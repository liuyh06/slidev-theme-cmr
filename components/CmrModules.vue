<script setup>
defineProps({ items: { type: Array, default: () => [] } })
</script>
<template><div class="cmr-module-grid"><section v-for="(item,i) in items" :key="i"><h3>{{ item.title }}</h3><ul><li v-for="line in item.lines" :key="line">{{line}}</li></ul></section></div></template>
