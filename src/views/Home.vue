<template>
  <div class="home">
    <Stream />
  </div>
</template>

<script>
// @ is an alias to /src
import Stream from '@/components/Stream.vue'

export default {
  name: 'Home',
  components: {
    Stream
  }
}
</script>
