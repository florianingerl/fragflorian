<script lang="ts">
import TheWelcome from '../components/TheWelcome.vue';
import VueWordOrder from './../components/vue-word-order.vue';
import Stupid from "./../components/Test.vue";
import { defineComponent } from "vue";

export default defineComponent(
  {
    components: { TheWelcome, Stupid, VueWordOrder }
  }
);
</script>

<template>
  <main>
    <TheWelcome />
    <Stupid />
    <VueWordOrder lg="fr" :sentences="['Nenad is smart.', 'Florian is smart too.']" />
  </main>
</template>
