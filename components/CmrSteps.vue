<script setup>
defineProps({ items: { type: Array, default: () => [] }, animated: Boolean })
</script>
<template>
  <ol class="cmr-steps">
    <template v-for="(item, i) in items" :key="i">
      <li v-if="animated" v-click="i + 1"><b>{{ String(i + 1).padStart(2, '0') }}</b><div><h3>{{ item.title }}</h3><p>{{ item.text }}</p></div></li>
      <li v-else><b>{{ String(i + 1).padStart(2, '0') }}</b><div><h3>{{ item.title }}</h3><p>{{ item.text }}</p></div></li>
    </template>
  </ol>
</template>
