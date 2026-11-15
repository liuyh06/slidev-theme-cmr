<script setup>
import CmrFrame from '../components/CmrFrame.vue'
defineProps({title:String,subtitle:String,number:String,quote:String,logo:String})
</script>
<template><CmrFrame kind="default" v-bind="$frontmatter"><div class="cmr-body"><slot/></div><div class="cmr-side"><slot name="right"/></div></CmrFrame></template>