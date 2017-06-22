<template>
  <div class="hello">
    I'm Test and.. {{msg}}
    <counter></counter>
    <counter></counter>
  </div>
</template>

<script>
import Counter from './Counter'

export default {
  data () {
    return {
      msg: 'shit'
    }
  },
  components: {
    'counter': Counter
  }
}
</script>
