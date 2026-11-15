<script setup>
defineProps({ center: String, items: { type: Array, default: () => [] } })
</script>
<template>
  <div class="cmr-radial-map" role="group" :aria-label="center">
    <svg viewBox="0 0 864 340" aria-hidden="true"><path d="M432 170L200 70 M432 170L664 70 M432 170L200 270 M432 170L664 270" /></svg>
    <div class="cmr-radial-center">{{ center }}</div>
    <div v-for="(item, i) in items.slice(0,4)" :key="i" class="cmr-radial-node" :class="'node-'+i"><h3>{{ item.title }}</h3><p>{{ item.text }}</p></div>
  </div>
</template>
