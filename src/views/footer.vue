<template>
  <div>
    <article class="about">
      <div id="abo">
          <h2 id="about--title">About our company</h2>
      </div>
      <div class="about--desc">
        <p class="about--desc-p">We are a company committed to the production and marketing of cakes, pastries, cookies and all kinds of delicious sweets.
        It is made up of a group of professional people dedicated to creating the most innovative delicacies you will find.
        Every day we strive to produce high-quality, homemade products that make the difference that our customers prefer in cakes and pastries.</p>

        <figure class="about--desc-img">
          <img class="img-ab" src="../assets/fondo.jpg" alt="">
          <figcaption class="img-desc">We offer cakes for all kinds of festivities</figcaption>
        </figure>
      </div>
    </article>

    <article class="contact">

        <div id="cont">
          <h2>Contact Us</h2>
          <p id="cont--p">Leave us a message, a comment, or just let us know what you think of your experience with our services.</p>
        </div>
        
        <div class="send-data">

          <div class="data--form">

            <form>

              <label for="fname"><i class="far fa-user"></i> First Name</label>
              <lp-Search-bar/>
              <label for="lname"><i class="far fa-envelope"></i> Your Email</label>
              <lp-Search-bar/> 
              <label for="subject"><i class="far fa-comments"></i> Subject (optional)</label>
              <textarea id="subject" name="subject" placeholder="  Write something.." style="height:170px"></textarea>
              <div class="btn-sub">
                <a href="#" id="btn-submit" >Send</a>
                <a href="#" id="btn-clear" >Clear</a>
              </div>

            </form>
            
          </div>

        </div>

    </article>

    <div class="reserved">
        <h6>My Candy Store © 2021 | All Rights Reserved |</h6>
        <h6>Web Design, Support, and Hosting by @GRAFIKE_</h6>
    </div>

  </div>
</template>

<script>
import lpSearchBar from '@/components/lpSearchBar.vue'

export default {
  name: 'Footer',
  components: {
    lpSearchBar
  }
}
</script>

<style scoped>
@import '../styles/footer.css';
</style>