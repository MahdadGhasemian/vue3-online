<script>
import { defineComponent } from 'vue';
import Vue3Online from '@/vue3-online.vue';

export default defineComponent({
  name: 'ServeDev',
  components: {
    Vue3Online
  }
});
</script>

<template>
  <div id="app">
    <vue3-online />
  </div>
</template>
