<template>
  <div id="app" class="p-48 antialiased font-sans text-gray-900">
    <div class="max-w-xs mx-auto">
      <VueSelect :data="wrestlers" v-model="selectedWrestler" v-on:valueSelect="onValueSelect">
        <template v-slot:SelectLabel>Wrestlers</template>
      </VueSelect>
    </div>  
  </div>
</template>

<script>
import VueSelect from './components/VueSelect';

export default {
  name: 'App',
  components: {
    VueSelect
  },
  methods: {
    onValueSelect(value) {
      this.selectedWrestler = value;
    }
  },
  data() {
    return {
      selectedWrestler: 'Hulk Hogan',
      wrestlers: [
        'Stone Cold Steve Austin',
        'Bret Hart',
        'Ric Flair',
        'Macho Man Randy Savage',
        'Jake The Snake Roberts',
        'The Undertaker',
        'Hulk Hogan',
        'Rikishi',
        'John Cena',
        'Shawn Michaels',
        'British Bulldog',
        'Superfly Jimmy Snuka',
        'The Ultimate Warrior',
        'Andre The Giant',
        'Doink The Clown',
      ]
    }
  }
}
</script>

<style>

</style>
