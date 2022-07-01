<template>
  <div>
    <div class="container">
      <NuxtLayout name="error">
        <template #header>
          <h1>Page Not Found</h1>
        </template>

        <template #redirectEl>
          <NuxtLink to="/">Go Back</NuxtLink>
        </template>
      </NuxtLayout>
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
img {
  width: 10rem;
}
</style>
