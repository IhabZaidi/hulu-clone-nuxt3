<template>
  <div>
    <nav className="relative pt-12">
      <div
        className="flex flex-row  px-10 sm:px-20 text-2xl whitespace-nowrap space-x-10 sm:space-x-20 overflow-x-scroll scrollbar-hide text-white"
      >
        <div
          v-for="navItem in navList"
          :key="navItem"
          class="group hover:text-teal-400 hover:scale-105 duration-200"
        >
          {{ navItem }}
          <div
            class="
              h-1
              rounded-full
              mt-0.5
              group-hover:scale-x-100 group-hover:bg-teal-400 group-hover:block
              w-[100%]
              transition-all
              duration-300
            "
          ></div>
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
  "Arabic",
  "Hindi",
  "Bluray"
];
</script>