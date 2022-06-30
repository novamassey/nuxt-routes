<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="/">Restaunts Home</a>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              activeClass="active"
              aria-current="page"
              to="/"
              >Home</NuxtLink
            >
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link" activeClass="active" to="/restaurants"
              >Restaurants</NuxtLink
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script></script>

<style>
.ml-auto {
  margin-left: auto;
}
</style>
