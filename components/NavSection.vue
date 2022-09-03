<template>
  <div>
    <nav className="relative pt-12">
      <div
        className="flex flex-row px-10 sm:px-20 text-2xl whitespace-nowrap space-x-10 sm:space-x-20 overflow-x-scroll scrollbar-hide text-white"
      >
        <div v-for="navItem in navList" :key="navItem">
          {{ navItem }}
        </div>
      </div>
      <div
        className="absolute top-0 right-0 bg-gradient-to-l from-[#06202A] h-10 w-1/12"
      />
    </nav>
  </div>
</template>

<script setup>
const navList = [
  "Trending",
  "TopRated",
  "Action",
  "Comedy",
  "Horror",
  "Romance",
  "Mystery",
  "Sci-Fi",
  "Western",
  "Animation",
];
</script>