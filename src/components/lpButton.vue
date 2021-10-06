<template>
  <section class="container-buttons">
    <a type="button" class="btn" href="#">Buy now</a>
  </section>
</template>
<style scoped>
.btn {
  font-size: 13px;
  background-color: var(--brownLg);
  padding: 15px 50px;
  width: 100px;
  letter-spacing: 3px;
  border-radius: 3px;
  color: var(--white);
  text-decoration: none;
  text-transform: uppercase;
}

.btn:hover {
  background-color: var(--brown);
  color: var(--white);
  transition: 0.6s;
}
</style>