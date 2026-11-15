<script setup>
defineProps({ items: { type: Array, default: () => [] }, snake: Boolean })
</script>
<template><ol class="cmr-flow" :class="{snake}"><li v-for="(item,i) in items" :key="i"><span>{{String(i+1).padStart(2,'0')}}</span><div>{{item}}</div><small v-if="i < items.length-1" aria-hidden="true">↓</small></li></ol></template>
