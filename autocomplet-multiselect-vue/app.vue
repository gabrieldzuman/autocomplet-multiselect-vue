<template>
  <div>
    <VueMultiselect
      v-model="multiValue"
      :options="source"
      :multiple="true"
      :close-on-select="true"
      placeholder="Autocomplete Funciona!"
      label="name"
      track-by="name" />
  </div>
</template>

<script setup>
import { ref } from "vue";
import VueMultiselect from "vue-multiselect";
const multiValue = ref(null);
const source = ref([
  { name: "Gabriel!" },
  { name: "Leonardo!" },
  { name: "Dzuman!" },
]);
</script>

<style src="vue-multiselect/dist/vue-multiselect.css"></style>
