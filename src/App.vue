<template>
  <NavBar />
  <Notes />
  <FormNote v-if="showForm" />
</template>

<script setup>
import { showForm } from './helpers/useNotes'
</script>
