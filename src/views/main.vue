<template>
  <div>

    <article class="main">
      <span id="start-page"></span>
        <a href="#start-page" class="btn-flotante"
          ><i class="fas fa-chevron-up"></i></a>
      <section class="main--paragraph">
        <h1 id="desc"> {{ title }} </h1>
        <p> {{ description }}</p>

        <lp-button/>
      </section>

      <section class="main--image">
        <lp-drink/>
      </section>
    </article>

    <article class="products">
      <div id="prod">
        <h2>Most purchased products</h2>
      </div>

      <section class="products--items">
        <figure>
          <img class="items-img" src="../assets/donuts.jpg" alt="">
          <figcaption>Chocolate Donuts ~ $5.99 c/u</figcaption>
          <lp-button-p/>
        </figure>
        <figure>
          <img class="items-img" src="../assets/cookie.jpg" alt="">
          <figcaption>Cookies ~ $1.99 c/u</figcaption>
          <lp-button-p/>
        </figure>
        <figure>
          <img class="items-img" src="../assets/cupCake.jpg" alt="">
          <figcaption>Cup Cake ~ $3.99 c/u</figcaption>
          <lp-button-p/>
        </figure>
      </section>
    </article>

    <div class="decoration"></div>
    <article class="offers">
      
      <section class="offers--container">

        <div id="off">
          <h2>Offers of the month</h2>
        </div>

        <div class="container--options">

          <lp-Offers id="offers-logo"/>
          <div class="offers--items">

            <div class="item">
                <img class="item-logo" src="../assets/skull.png" alt="">
                <div class="item-desc">
                  <h5 class="item-title">Sugar skull set ~ <a href="#"><p class="item-price">$14.99</p></a></h5>
                  <p class="item-info">The Halloween game of the sugar skull is composed of a total of two dozen terrifying candies.</p>
                </div>
            </div>

            <div class="item">
                <img class="item-logo" src="../assets/halloween.png" alt="">
                <div class="item-desc">
                  <h5 class="item-title">Halloween bag ~ <a href="#"><p class="item-price two">$7.99</p></a></h5>
                  <p class="item-info">12 bags of Halloween candy, chocolates and marshmallows.</p>
                </div>
            </div>

            <div class="item">
                <img class="item-logo" src="../assets/fran.png" alt="">
                <div class="item-desc">
                  <h5 class="item-title">Frankenstein cake ~ <a href="#"><p class="item-price three">$24.99</p></a></h5>
                  <p class="item-info">Monstrous promotional chocolate cake with strawberries that will come to life to scare everyone on October 31st.</p>
                </div>
            </div>

          </div>

        </div>
        
      </section>

    </article>

  </div>
</template>

<script>
import Typewriter from 'typewriter-effect/dist/core';
import lpDrink from '@/components/lpDrink.vue'
import lpOffers from '@/components/lpOffers.vue'
import lpButton from '@/components/lpButton.vue'
import lpButtonP from '@/components/lpButtonP.vue'

export default {
  name: 'Main',
  data() {
    return {
      description: 'Sweets of all the colors and flavors you can imagine. Where you will find the greatest delights in the universe.',
      title: 'The best delicacies',
      options: [
        'Chocolate CAKES...', 
        'Gummy BEARS...',
        'Coffee and DONUTS...',
        'Vanilla MUFFIN...',
        'And more...'
        ],
      text:{
        name: 'Your name'
      }
    }
  },

  components: {
    lpDrink,
    lpButton,
    lpButtonP,
    lpOffers
  },

  mounted() {
    var app = document.getElementById('desc')
    var typewriter = new Typewriter(app, {
      loop: true,
      delay: 120,
      changeDeleteSpeed: 'natural'
    })
    typewriter
      .pauseFor(300)
      .typeString(this.title)
      .pauseFor(6000)
      .deleteAll()
      .typeString(this.options[0])
      .pauseFor(4000)
      .deleteAll()
      .typeString(this.options[1])
      .pauseFor(4000)
      .deleteAll()
      .typeString(this.options[2])
      .pauseFor(4000)
      .deleteAll()
      .typeString(this.options[3])
      .pauseFor(4000)
      .deleteAll()
      .typeString(this.options[4])
      .start()
  },
}
</script>
<style scoped>
@import '../styles/main.css';


.decoration {
  height: 54px;
  margin-top: 30px;
  background: linear-gradient(
    to bottom left,
    transparent 50%,
    var(--grey) 51%
  );
}
/* --- --- -- RESPONSIVE DESIGN -- --- --- */
@media only screen and (max-width: 1035px) {
  .decoration{
    display: none;
    background-color: transparent;
  }
}

</style>


