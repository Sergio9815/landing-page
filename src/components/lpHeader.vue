<template>
  <div>
    <nav class="container">
      <section class="container-logo">
        <img id="ico" src="../assets/shop.png" alt="">
        <h3>My Business</h3>
      </section>
      <section class="container-menu">
				<ul>
					<li><a href="">Services <i class="fas fa-chevron-down"></i></a></li>
					<li><a href="">Offers <i class="fas fa-chevron-down"></i></a></li>
					<li><a href="">About us <i class="fas fa-chevron-down"></i></a></li>
					<li><a id="btn-about" onclick="hideContact()" href="#about-me">Contact <i class="fas fa-chevron-down"></i></a></li>
				</ul>
        <a class="btn" href="">Register</a>
      </section>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<style scoped>

.container {
  font-family: 'Lato', sans-serif;
  background-color: transparent;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 80px;
}

.container-logo {
  background-color: transparent;
  display: flex;
  align-items: center;
  justify-content: center;
}

h3 {
  font-weight: bold;
  color: #161616;
  margin: 0;
}

#ico {
  width: 30px;
  margin-right: 6px;
}

.container-menu {
  display: flex;
  align-items: center;
  justify-content: center;
}

.container-menu ul {
  list-style: none;
  padding-right: 50px; 
  margin: 0;
}

.container-menu ul li {
  float: left;
  padding-left: 40px; 
}
  
.container-menu ul li a {
  color: #161616;
  text-decoration: none;
  letter-spacing: 2px;
  font-size: 15px; 
  font-family: 'Roboto', sans-serif;
  font-weight: normal;
}

.container-menu ul li a:hover {
  border-bottom: solid 3px #c1b3ff6b; 
}

.btn {
  font-size: 13px;
  background-color: #c1b3ff6b;
  padding: 10px;
  width: 100px;
  letter-spacing: 3px;
  border-radius: 3px;
  color: #161616;
  text-transform: uppercase;
  text-decoration: none;
}

.btn:hover {
  background-color: #c1b3ff;
  color: white;
  transition: 0.6s;
}

</style>
