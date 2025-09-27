<!-- An example of using a title followed by a section that uses tabs
 for navigation combined with a div for displaying content.  -->
<script setup lang="ts">
import TopBanner from '../components/TopBanner.vue';
import TabBar from '../components/TabBar.vue';
import HelloWorld from '../components/HelloWorld.vue';
</script>

<template>
  <TopBanner />
  <TabBar :button-labels="['one', 'two', 'three', 'four']" :selected="2" />
  <HelloWorld />
</template>