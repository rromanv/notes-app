<template>
  <div
    v-motion
    :initial="{
      y: 100,
    }"
    :enter="{
      y: 0,
    }"
    class="absolute inset-0 w-screen h-screen flex justify-center items-center bg-purple-900 overflow-hidden"
  >
    <button @click="showForm = false">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        class="w-16 absolute inset-1"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M10 14l2-2m0 0l2-2m-2 2l-2-2m2 2l2 2m7-2a9 9 0 11-18 0 9 9 0 0118 0z"
        />
      </svg>
    </button>
    <form @submit.prevent class="space-y-4">
      <div class="flex flex-col">
        <label for="title">Title</label>
        <input type="text" name="title" class="rounded" placeholder="Title" />
      </div>
      <div class="flex flex-col">
        <label for="content">Content</label>
        <textarea name="content" class="rounded" placeholder="Note Content" />
      </div>
      <div>
        <button
          class="w-full bg-yellow-500 text-yellow-800 p-2 rounded mt-4 hover:bg-yellow-600 hover:text-yellow-900"
        >
          Add
        </button>
      </div>
    </form>
  </div>
</template>

<script setup>
import { showForm } from '../helpers/useNotes'
</script>
