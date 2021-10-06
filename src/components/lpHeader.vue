<template>
  <div>
    <nav class="container">
      <section class="container-logo">
        <img id="ico" src="../assets/candy.png" alt="">
        <h3> {{name}} </h3>
      </section>
      <section class="container-menu">
				<ul>
					<li><a href="#prod">Products</a></li>
					<li><a href="#off">Offers</a></li>
					<li><a href="#ab">About us</a></li>
					<li><a href="#cont">Contact</a></li>
				</ul>
      </section>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      name: 'My Candy Store',
    }
  }
}
</script>

<style scoped>
@import '../styles/header.css';
</style>
