<template>
<div class="container">
  <h1>Rick and Morty</h1>
  <FilterByStatus />
  <FilterByName />
  <ListCharacters />
</div>
</template>

<script>
import ListCharacters from '@/components/ListCharacters.vue'
import FilterByName from '@/components/FilterByName.vue'
import FilterByStatus from '@/components/FilterByStatus.vue'

export default {
  name: 'App',
  components: {
    ListCharacters,
    FilterByName,
    FilterByStatus
  } 
}
</script>

<style lang="scss">

:root {
  --background-body: #24282f;
  --background-card: #3C3E44;
  --text-white: #FFFFFF;
  --text-gray: #c0c0c0;
  --text-orange: #FF9800;
}
* {
  box-sizign: border-box;
  margin: 0;
  padding: 0;
}
body {
  background-color: var(--background-body);
  color: var(--text-white);
  font-family: 'Segoe UI', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
h1 {
  margin-bottom: 3rem;
  text-align: center;
}
.container {
  width: 980px;
  max-width: 90%;
  margin: 5rem auto;
}
img {
  width: 100%;
}

</style>
