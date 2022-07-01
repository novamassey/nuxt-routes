<template>
  <div>
    <Html :lang="dynamic > 50 ? 'en-GB' : 'en-US'">
      <Head>
        <Title>Top 50 Restaurants</Title>
        <Meta name="description" content="My page is awesome socks!"></Meta>
        <Link
          rel="preload"
          href="https://www.iconpacks.net/icons/2/free-sad-face-icon-2691-thumb.png"
          as="script"
        />
      </Head>
    </Html>
    <NuxtLayout name="custom">
      <div class="table">
        <RestaurantTable />
      </div>
    </NuxtLayout>
  </div>
</template>
