<script setup>
import { computed } from 'vue'
const props = defineProps({ title:String, unit:{default:''}, max:Number, rows:{type:Array,default:()=>[]} })
const limit = computed(() => props.max || Math.max(1,...props.rows.map(r=>r.value)))
</script>
<template><figure class="cmr-bars"><figcaption>{{title}}<small>{{unit}}</small></figcaption><div v-for="(row,i) in rows" :key="i" class="cmr-bar-row"><span>{{row.label}}</span><div class="cmr-bar-track"><div class="cmr-bar-fill" :style="{width:Math.max(0,Math.min(100,row.value/limit*100))+'%'}" /></div><b>{{row.display ?? row.value}}</b></div></figure></template>
