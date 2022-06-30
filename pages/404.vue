<template>
  <div>
    <Navbar />
    <div class="container">
      <h2>Page Not Found</h2>
      <NuxtLink to="/">Go to Back</NuxtLink>
    </div>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
  margin-top: 5rem;
}
.link {
  text-decoration: underline;
  cursor: pointer;
}
</style>
