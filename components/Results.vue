<template>
  <div className="px-5 my-10 sm:grid md:grid-cols-2 xl:grid-cols-3 gap-x-8">
    <div v-for="anime in myAnimeList" :key="anime.id">
      <Thumbnail :anime=anime />
    </div>
  </div>
</template>

<script setup>
const {data: myAnimeList} = useFetch("/api/myData");
console.log(myAnimeList);
</script>