<script setup>
import CmrFrame from '../components/CmrFrame.vue'
</script>
<template>
  <CmrFrame kind="flow-snake" v-bind="$frontmatter">
    <div class="cmr-body"><slot /></div>
    <div class="cmr-side"><slot name="right" /></div>
    <div class="cmr-caption"><slot name="caption" /></div>
  </CmrFrame>
</template>
