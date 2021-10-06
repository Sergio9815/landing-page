<template>
  <section class="container-buttons">
    <a type="button" class="btn btn-p" href="#">Buy now</a>
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

.btn-p {
  padding: 8px;
  margin-top: 10px;
  width: 200px;
}
</style>