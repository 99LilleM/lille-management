<template>
  <select @change="onThemeChange">
    <option v-for="theme in daisyThemes" :key="theme" :value="theme" :data-theme="theme">
      {{ theme }}
    </option>
  </select>
</template>

<script setup lang="ts">



const daisyThemes = [
  'light',
  'dark',
  'cupcake',
  'bumblebee',
  'emerald',
  'corporate',
  'synthwave',
  'retro',
  'cyberpunk',
  'valentine',
  'halloween',
  'garden',
  'forest',
  'aqua',
  'lofi',
  'pastel',
  'fantasy',
  'wireframe',
  'black',
  'luxury',
  'dracula',
    'cmyk',
    'autumn',
    'business',
    'acid',
    'lemonade',
    'night',
    'coffee',
    'winter',
    'dim',
    'nord',
    'sunset',
    'caramellatte',
    'abyss',
    'silk'
]


const onThemeChange = (event) => {
  //apply to html data-theme-[theme]
  document.documentElement.setAttribute('data-theme', event.target.value)
}

</script>

<style scoped>

</style>