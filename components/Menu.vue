<template>
  <v-list>
    <v-list-item v-for="page in pages" :to="page.path">
      <v-list-item-title v-text="page.title" />
    </v-list-item>
  </v-list>
</template>

<script setup lang="ts">
const pages = [
  {
    title: 'メイン',
    path: '/'
  },
  {
    title: '検索',
    path: '/search'
  }
]
</script>