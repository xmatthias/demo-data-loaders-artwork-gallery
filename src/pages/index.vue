<script lang="ts">
import { useArtworkList } from '@/loaders/artwork-list'
export { useArtworkList }
</script>

<script setup lang="ts">
const { data: artworkList } = useArtworkList()
</script>

<template>
  <main>Home</main>

  <div class="masonry">
    <ArtworkCard
      v-for="artwork in artworkList.data"
      :key="artwork.id"
      :artwork="artwork"
    />
  </div>
</template>
