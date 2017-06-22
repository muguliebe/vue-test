<template>
  <div class="counter">
    <span class="count">{{count}}</span>
    <button class="btn btn-info" @click="add">add</button>
    <button class="btn btn-warning" @click="minus">minus</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  computed: {
    count() {
      return this.$store.state.count
    }
  },
  methods: {
    add() {
      return ++this.$store.state.count
    },
    minus() {
      return --this.$store.state.count
    }
  }
}
</script>

<style>
.count{
  font-size: 2rem;
  display: block;
}
</style>
