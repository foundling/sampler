<template>
  <div class="pad">
  </div>
</template>

<script>
export default {
  name: 'Pad',
  data () {
    return {
      lastPressed: false
    }
  }
}
</script>

<style scoped lang="scss">
  .pad {
    list-style-type: none;
    margin: 15px;
    border: 3px solid transparent;
    border-radius: 10%; 
    background: #383d40;
    height: 80px;
    width: 80px;
    transition: background 0.5s ease-in;
 
    &:hover:active {
      background: #afff00;
      transition: background 0.01s ease-in;
    }
 
    &.last-pressed {
      border: 3px solid red;
    }
 
  }
</style>
