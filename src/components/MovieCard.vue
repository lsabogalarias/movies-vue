<!-- eslint-disable-next-line no-return-assign, no-param-reassign -->
<template>
  <div>
    <h2>{{title}}</h2>
    <img width="100" v-bind:src="image" v-bind:alt="title"/>    
  </div>
</template>

<script>
export default {
  name: 'MovieCard',
  props: ['image', 'title'],
};
</script>