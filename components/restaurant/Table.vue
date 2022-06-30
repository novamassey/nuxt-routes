<template>
  <div class="table">
    <h1>Top 50: Restaunts</h1>
    <div class="table-container">
      <div class="table-col">
        <RestaurantRow :isHeader="true" />
        <RestaurantRow
          v-for="(restaurant, index) in restaurantsOrganized.first"
          :key="restaurant.id"
          :index="index"
          :name="restaurant.name"
          :rank="restaurant.rank"
        />
      </div>
      <div class="table-col">
        <RestaurantRow :isHeader="true" />
        <RestaurantRow
          v-for="(restaurant, index) in restaurantsOrganized.second"
          :key="restaurant.id"
          :index="index"
          :name="restaurant.name"
          :rank="restaurant.rank"
        />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import data from "@/data.json";

const restaurantsOrganized = {
  first: [...data].splice(0, 25),
  second: [...data].splice(25, 25),
};
</script>

<style scoped>
.table {
  margin: 3rem 0;
}
.table h1 {
  margin-bottom: 2rem;
}
.table-container {
  display: flex;
  justify-content: space-between;
}
.table-col {
  width: 48%;
}
</style>
