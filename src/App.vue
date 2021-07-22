<template>
  <img alt="Vue logo" src="./assets/logo.png" />
</template>

<script lang="ts">
import { defineComponent, Ref, ref } from 'vue';

export default defineComponent({
  name: 'App',
  setup() {
    const card = ref<HTMLElement | string>('');
    const logCardInfo = (card: Ref<HTMLElement | string>) => {
      console.log(card.value);
    };
    logCardInfo(card);
  },
});
</script>
