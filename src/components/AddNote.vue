<template>
  <div
    class="bg-yellow-400 text-yellow-800 text-center p-2 rounded-xl flex justify-center items-center"
  >
    <button @click="showForm = !showForm">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        class="w-24 h-24 opacity-40"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
        />
      </svg>
    </button>
  </div>
</template>

<script setup>
import { showForm } from '../helpers/useNotes'
</script>
