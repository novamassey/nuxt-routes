<template>
  <div>
    <slot name="header" />
    <div class="img-container">
      <img
        src="https://www.iconpacks.net/icons/2/free-sad-face-icon-2691-thumb.png"
        alt=""
      />
    </div>
    <slot name="redirectEl" />
  </div>
</template>

<script></script>

<style scoped>
.img-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
img {
  width: 10rem;
}
</style>
