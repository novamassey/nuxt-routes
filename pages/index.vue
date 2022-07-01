<template>
  <div>
    <Html :lang="dynamic > 50 ? 'en-GB' : 'en-US'">
      <Head>
        <Title>Restuarant Site</Title>
        <Meta name="description" content="My page is awesome socks!"></Meta>
        <Link
          rel="preload"
          href="https://www.iconpacks.net/icons/2/free-sad-face-icon-2691-thumb.png"
          as="script"
        />
      </Head>
    </Html>
    <div class="container">
      <h2>Welcome to Restaurants</h2>
      <NuxtLink to="/restaurants">Go to restaurants</NuxtLink>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.container {
  text-align: center;
  margin-top: 5rem;
}
</style>
