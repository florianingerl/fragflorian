<script lang="ts">
import TheWelcome from '../components/TheWelcome.vue';
import VueWordOrder from './../components/vue-word-order.vue';
import VueWholeSentence from './../components/vue-whole-sentence.vue';
import Stupid from "./../components/Test.vue";
import { defineComponent } from "vue";

export default defineComponent(
  {
    components: { TheWelcome, Stupid, VueWordOrder, VueWholeSentence }
  }
);
</script>

<template>
  <main>
    <TheWelcome />
    <Stupid />
    <VueWordOrder lg="fr" :sentences="['Nenad is smart.', 'Florian is smart too.']" />
    <VueWholeSentence lg="en" :sentences="[{task: 'Florian is what?', solution: 'smart'}, { task: 'Nenad is what?', solution: 'smart' }]" />
  </main>
</template>
