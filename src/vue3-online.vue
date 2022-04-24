<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "Vue3Online",
  data() {
    return {
      onlineStatus: navigator.onLine,
    };
  },
  mounted() {
    this.addHandler();
  },
  unmounted() {
    this.remveHanlder();
  },
  methods: {
    addHandler() {
      window.addEventListener("online", () => {
        this.onlineStatus = true;
      });
      window.addEventListener("offline", () => {
        this.onlineStatus = false;
      });
    },
    remveHanlder() {
      window.removeEventListener("online", () => {});
      window.removeEventListener("offline", () => {});
    },
  },
  computed: {
    isOnline() {
      return this.onlineStatus;
    },
  },
});
</script>

<template>
  <div>
    <slot v-if="isOnline"></slot>
    <slot v-else name="offline"></slot>
  </div>
</template>
