<template lang="">
  <div class="input-wrapper">
    <div class="search">
      <input placeholder="Enter name of the city" class="input" />
      <button class="search-btn" type="button">Enter</button>
    </div>

    <!-- <ul class="search-hints">
      <li class="hints-item">Almaty</li>
      <li class="hints-item">Astana</li>
      <li class="hints-item">Almarasan</li>
      <li class="hints-item">Almaty</li>
    </ul> -->
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.input-wrapper {
  max-width: 523px;
  box-shadow: 0px 0px 20px rgba(120, 161, 187, 0.3);
  border-radius: 30px;
  overflow: hidden;
}

.search {
  position: relative;
  padding: 1rem 2rem;
  border: 1px solid #e9f0eb;
  border-radius: 31px;
  max-width: 523px;
  height: 63px;
  display: flex;
  align-items: center;
}

.input-wrapper.active {
  box-shadow: 0px 0px 20px rgba(120, 161, 187, 0.3);
  overflow: hidden;
}

.search-hints {
  left: 0;
  right: 0;
  top: 100%;
  display: flex;
  flex-direction: column;
  list-style: none;
  gap: 0.5rem;
  padding: 0;
  margin: 0;
  padding: 0 1.5rem 1rem;
  background-color: #fff;
}

.hints-item {
  padding: 1.5rem 0.5rem 0.7rem;
  border-bottom: 1px solid #E9F0EB;
}

.hints-item:last-of-type {
  border-bottom: none;
}

.input {
  display: block;
  width: 100%;
  height: 50;
  border: none;
  outline: none;
  font-size: 1.5rem;
}

.input::placeholder {
  color: #d9e4dc;
}

.search-btn {
  background: linear-gradient(279.56deg,
      #65b3e4 15.15%,
      rgba(120, 161, 187, 0) 171.55%);
  border: none;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  right: 0;
  height: 63px;
  color: #fff;
  cursor: pointer;
  width: 170px;
  border-radius: 50px;
  font-size: 1.5rem;
}
</style>
