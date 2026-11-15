<script setup>
defineProps({ items:{type:Array,default:()=>[]} })
</script>
<template><ol class="cmr-icon-steps"><li v-for="(item,i) in items" :key="i"><b>{{item.icon || String(i+1).padStart(2,'0')}}</b><div><h3>{{item.title}}</h3><p>{{item.text}}</p></div></li></ol></template>
