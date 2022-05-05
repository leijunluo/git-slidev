<script setup lang="ts">
import { defineProps, defineComponent } from 'vue'

import Default from './default.vue'

const components = defineComponent({ Default })
const props = defineProps({
  eventLogo: {
    type: String,
  },
  eventUrl: {
    type: String,
  },
  twitter: {
    type: String,
  },
  twitterUrl: {
    type: String,
  },
  media: {
    type: String,
  },
  reverse: {
    type: Boolean
  }
})


</script>

<template>
  <default
    class="presenter"
    :logo-header="logoHeader"
    :event-logo="eventLogo"
    :event-url="eventUrl"
    :twitter="twitter"
    :twitter-url="twitterUrl"
  >
    <div class="grid grid-cols-2 gap-1" :class="{ 'gap-16': reverse}">
     
      <div class="prose pr-16 " :class="{ 'order-1 text-right': reverse}">
        <slot />
      </div>
       <figure class="relative flex flex-col justify-center">
        <img
          :src="media"
          class="rounded-lg shadow-lg object-cover z-10 mt-18"
        />
      </figure>
    </div>
  </default>
</template>
