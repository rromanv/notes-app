<template>
  <div class="container mx-auto mt-8 grid grid-cols-3 gap-4">
    <Note v-for="n in 5" :key="n" />
    <AddNote />
  </div>
</template>
