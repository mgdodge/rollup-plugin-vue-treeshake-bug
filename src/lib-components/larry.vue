<script>
import { hello } from './helpers';

export default {
  name: 'Larry', // vue component name
  data() {
    return {
      name: 'Larry, the best of the three stooges',
    };
  },
  computed: {
    greeting() {
      return hello(this.name);
    }
  },
};
</script>

<template>
  <div class="larry">
    <p>{{ greeting }}</p>
  </div>
</template>

<style scoped>
  .larry {
    display: block;
    width: 400px;
    margin: 25px auto;
    border: 1px solid #ccc;
    background: #eaeaea;
    text-align: center;
    padding: 25px;
  }
  .larry p {
    margin: 0 0 1em;
  }
</style>
