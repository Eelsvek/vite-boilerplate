<template>
  <div>
    <button @click="changeName(1)"></button>
    <div>{{ name }}</div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'App',
  components: {},

  setup() {
    const name = ref('Kevin')

    const changeName = (newName: string) => {
      name.value = newName
    }

    return {
      changeName,
      name,
    }
  },
})
</script>

<style></style>
