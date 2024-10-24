<script setup>
import { useWebsiteStore } from '~/stores/websiteStore';

const store = useWebsiteStore()
const counter = useState("counter", () => 0);
</script>

<template>
  state test
  counter: {{ counter }}
  <button @click="counter++">Inc</button>

  store test:
    {{  store.name }}
</template>
