<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  logoHeader: {
    type: String,
  },
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
})
</script>

<template>
  <div class="bg-main slidev-layout">
    <CornerCurves class="absolute transform bottom-0 right-0 flip-x" />
    <!-- <CornerCurves class="absolute flip-z left-0 bottom-0 transform rotate-0" /> -->
    <LayoutHeader :logo-header="logoHeader" />
    <div class="z-15">
      <slot />
    </div>
    <LayoutFooter
      :event-logo="eventLogo"
      :event-url="eventUrl"
      :twitter="twitter"
      :twitter-url="twitterUrl"
    />
  </div>
</template>
