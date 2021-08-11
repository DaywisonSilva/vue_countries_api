<template>
  <header class="header">
    <h1>Where in the World?</h1>
    <label>
      <i class="fas fa-sun" v-if="isDarkOn"></i>
      <i class="fas fa-moon" v-else></i>
      <input
        @input="$emit('onDarkMode', isDarkOn)"
        type="checkbox"
        class="header__checkbox"
        v-model="isDarkOn"
      />
      Dark Mode
    </label>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isDarkOn: false,
    }
  },
}
</script>

<style scoped>
.header {
  width: 100%;
  height: 60px;

  background-color: var(--dark-blue);
  color: var(--white);

  display: flex;
  align-items: center;
  justify-content: space-between;

  padding: 0 35px;
}

.header h1 {
  font-size: 22px;
}

.header label {
  font-weight: 600;
}

.header__checkbox {
  display: none;
}

.hidden {
  display: none;
}
</style>
