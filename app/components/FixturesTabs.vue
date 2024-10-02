<script setup lang="ts">
const items = [{
  label: 'Fixtures',
  icon: 'i-heroicons-information-circle',
  content: 'This is the content shown for Tab1'
}, {
  label: 'Round of 18',
  icon: 'i-heroicons-arrow-down-tray',
  content: 'And, this is the content for Tab2'
}, {
  label: 'Round of 16',
  icon: 'i-heroicons-eye-dropper',
  content: 'Finally, this is the content for Tab3'
},
{
  label: 'Round of 16',
  icon: 'i-heroicons-eye-dropper',
  content: 'Finally, this is the content for Tab3'
}]

function onChange (index) {
  const item = items[index]

  alert(`${item.label} was clicked!`)
}
</script>

<template>
  <UTabs :items="items" @change="onChange" />
</template>

