<template lang="">
  <section>
    <h3 class="section-title">Most popular cities</h3>
    <ul class="cities">
      <li class="city" v-for="city in CITIES" :key="city">{{ city }}</li>
    </ul>
  </section>
</template>
<script>
import { CITIES } from '../data';

export default {
  data: function () {
    return {
      CITIES,
    };
  },
};
</script>
<style scoped>
.cities {
  display: flex;
  flex-direction: column;
  list-style: none;
  padding: 0;
  display: grid;
  grid-template-columns: 1fr 1fr;
  column-gap: 75px;
  margin-top: 2.5rem;
}

.city {
  padding: 0.8rem 1rem;
  border-bottom: 1px solid #e9f0eb;
  color: rgba(40, 48, 68, 0.5);
  font-size: 1.4rem;
}
</style>
