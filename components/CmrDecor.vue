<script setup>
import { computed } from 'vue'
const props = defineProps({ kind: { default: 'default' } })
const variants = {
  "cover": [
    {
      "left": 725.612,
      "top": -115.485,
      "width": 218.513,
      "height": 218.513,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 864.921,
      "top": -35.446,
      "width": 218.513,
      "height": 218.513,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 886.411,
      "top": 163.87,
      "width": 102.132,
      "height": 102.132,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 15.875,
      "top": 436.971,
      "width": 218.513,
      "height": 218.513,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -123.434,
      "top": 356.933,
      "width": 218.513,
      "height": 218.513,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -28.543,
      "top": 273.998,
      "width": 102.132,
      "height": 102.132,
      "angle": 135.0,
      "opacity": 0.89804
    }
  ],
  "contents": [
    {
      "left": 25.284,
      "top": 391.234,
      "width": 333.522,
      "height": 333.522,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -145.748,
      "top": 294.653,
      "width": 293.123,
      "height": 293.123,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -56.861,
      "top": 151.826,
      "width": 113.723,
      "height": 113.723,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": 853.445,
      "top": -74.314,
      "width": 140.94,
      "height": 140.94,
      "angle": 135.0,
      "opacity": 0.89804
    }
  ],
  "section": [
    {
      "left": 690.649,
      "top": -122.34,
      "width": 242.192,
      "height": 242.192,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 845.053,
      "top": -33.628,
      "width": 242.192,
      "height": 242.192,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 868.872,
      "top": 187.286,
      "width": 113.199,
      "height": 113.199,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": -7.961,
      "top": 478.538,
      "width": 218.513,
      "height": 218.513,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -147.269,
      "top": 398.499,
      "width": 218.513,
      "height": 218.513,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -52.379,
      "top": 315.564,
      "width": 102.132,
      "height": 102.132,
      "angle": 135.0,
      "opacity": 0.89804
    }
  ],
  "default": [
    {
      "left": -48.689,
      "top": 6.404,
      "width": 86.097,
      "height": 86.097,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -15.275,
      "top": -34.439,
      "width": 69.498,
      "height": 69.498,
      "angle": 135.0,
      "opacity": 0.89804
    }
  ],
  "end": [
    {
      "left": 725.612,
      "top": -115.485,
      "width": 218.513,
      "height": 218.513,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 864.921,
      "top": -35.446,
      "width": 218.513,
      "height": 218.513,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 886.411,
      "top": 163.87,
      "width": 102.132,
      "height": 102.132,
      "angle": -45.0,
      "opacity": 0.89804
    },
    {
      "left": 15.875,
      "top": 436.971,
      "width": 218.513,
      "height": 218.513,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -123.434,
      "top": 356.933,
      "width": 218.513,
      "height": 218.513,
      "angle": 135.0,
      "opacity": 0.89804
    },
    {
      "left": -28.543,
      "top": 273.998,
      "width": 102.132,
      "height": 102.132,
      "angle": 135.0,
      "opacity": 0.89804
    }
  ]
}
const squares = computed(() => variants[props.kind] || variants.default)
</script>
<template><div class="cmr-geometry" aria-hidden="true"><i v-for="(s,i) in squares" :key="i" :style="{left:s.left+'px',top:s.top+'px',width:s.width+'px',height:s.height+'px',transform:'rotate('+s.angle+'deg)',opacity:s.opacity}" /></div></template>
<style>
.cmr-geometry{position:absolute;inset:0;pointer-events:none;overflow:hidden}
.cmr-geometry i{position:absolute;display:block;background:var(--cmr-primary);transform-origin:center}
.slidev-layout.cmr:after{display:none}
.cmr header{position:relative;z-index:1}
</style>
