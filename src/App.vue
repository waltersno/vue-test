<script setup>
import SearchInputVue from './components/SearchInput.vue';
import PopularCities from './components/PopularCities.vue';
</script>

<template>
  <div class="app-container">
    <main class="main">
      <aside class="left-side">
        <header class="header">
          <img src="@/assets/images/logo.svg" />
          <h2>FastService</h2>
        </header>
        <section class="page-title">
          <h1 class="title">Delivery cost</h1>
          <h5 class="subtitle">
            Enter name of the city to count delivery cost
          </h5>
        </section>
        <div>
          <SearchInputVue />
        </div>
        <PopularCities />
        <footer class="footer">
          <div class="left-footer">
            <p>All rights reserved</p>
            <p>Fast service 2021</p>
          </div>
          <div class="right-footer">
            <img src="@/assets/images/visa-logo-icon-png_44632.svg" />
            <img src="@/assets/images/1280px-Mastercard-logo.svg" />
            <img src="@/assets/images/1200px-Maestro_2016.svg" />
            <img src="@/assets/images/proccessing.svg" />
          </div>
        </footer>
      </aside>
      <aside class="right-side">
        <div class="default-images">
          <img class="car" src="@/assets/images/car.png" alt="" />
          <img class="road" src="@/assets/images/road.png" alt="" />
          <img class="service" src="@/assets/images/serviceLogo.png" alt="" />
        </div>
      </aside>
    </main>
  </div>
</template>

<style scoped>
.default-images {
  position: relative;
  height: 100%;
}

.car {
  width: 50%;
}
.main {
  display: flex;
  gap: 144px;
}
.left-side {
  display: flex;
  flex-direction: column;
  gap: 4.5rem;
}

.app-container {
  display: flex;
  justify-content: end;
}

.page-title {
  font-size: 3rem;
  line-height: 3.5rem;
}

.section-title {
  font-size: 1.5rem;
}

.header {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  max-height: 100vh;
  margin-top: 1.5rem;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

.page-title {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.title {
  font-size: 3rem;
  line-height: 3.5rem;
}

.subtitle {
  font-weight: 400;
  color: #28304480;
  font-size: 1.5rem;
}

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 28px;
  font-size: 14px;
  color: rgba(40, 48, 68, 0.5);
}

.right-footer {
  display: flex;
  gap: 10px;
}

.right-side {
  height: 100vh;
  width: 50vw;
  background: #f7f7f7;
  border-radius: 40px 0px 0px 40px;
}
</style>
