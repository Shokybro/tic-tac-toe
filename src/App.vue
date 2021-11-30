<template>
  <div id="app">
      <div class="container">
         <button @click="start" class="container--btn" type="button">Start game</button>
      </div>
      <GameSingle v-if="current === 'Game'"></GameSingle>
  </div>
</template>

<script>

import GameSingle from '@/components/GameSingle'
export default {
  components: {GameSingle},
  name: 'App',
  data () {
    return {
      current: "Menu"
    }
  },
  methods: {
    start () {
      this.current = 'Game'
      document.querySelector('.container').style.display = 'none'
    }
  }
}
</script>

<style lang="scss" scoped>
  .container {
    display: inline-block;
    position: relative;
    left: 50%;
    top: 10rem;
    transform: translate(-50%, -50%);

    &--btn {
      border: none;
      background-color: aqua;
      padding: 1rem 2rem;
      font-weight: 500;
      cursor: pointer;
    }
  }
</style>
