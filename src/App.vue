<template>
  <div id="app" class="p-48 antialiased font-sans text-gray-900">
    <div class="max-w-xs mx-auto">
      <select name="wrestler" id="wrestler" v-model="selectedWrestler">
        <option v-for="wrestler in wrestlers" :key="wrestler">
          {{ wrestler }}
        </option>
      </select>
    </div>  
  </div>
</template>

<script>
export default {
  name: 'App',
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
