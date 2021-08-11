<template>
  <div class="select">
      <h1>Componente select do daywison</h1>
      <span class="material-icons-outlined">
check_circle
</span>
    <div class="select__input">
        <div class="select__selected">Filter By Region</div>
        <div class="select__options">
            <ul>
                <li>Africa</li>
                <li>America</li>
                <li>Asia</li>
                <li>Europe</li>
                <li>Oceania</li>
            </ul>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    
    .select{}

    .select__input {
        width: 200px;
        height: 40px;
        background-color: var(--white);
        box-shadow: 0px 0px 5px #9595956b;
        border-radius: var(--border-radius);
    }
</style>