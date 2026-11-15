<script setup>
import CmrDecor from './CmrDecor.vue'

defineProps({ kind: {default:'default'}, title:String, subtitle:String, number:String, quote:String, logo:String })
</script>
<template><div class="slidev-layout cmr" :class="'cmr-'+kind"><CmrDecor :kind="kind" /><img v-if="logo" class="cmr-logo" :src="logo"/><template v-if="kind==='section'"><div class="cmr-quote">{{quote}}</div><div class="cmr-section-name"><h1>{{title}}</h1><p>{{subtitle}}</p></div><div class="cmr-number">{{number}}</div></template><template v-else><header v-if="title"><h1>{{title}}</h1><p v-if="subtitle">{{subtitle}}</p></header><main><slot/></main></template></div></template>