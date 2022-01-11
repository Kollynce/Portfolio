<template>
  <div
    class="container mx-auto md:mt-28 mt-10 px-4 space-y-16 md:px-56 2xl:px-80"
  >
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 place-items-center">
      <template v-for="thumbnail in thumbnails" :key="thumbnail.title">
        <div
          class="
            md:w-96
            h-96
            thumb
            rounded-2xl
            flex flex-col
            items-center
            justify-center
          "
        >
          <p class="text-center text-white font-bold text-xl">
            {{ thumbnail.title }}
          </p>
          <p class="text-center text-white leading-relaxed px-4">
            {{ thumbnail.description }}
          </p>
        </div>
      </template>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      thumbnails: [
        {
          title: "Homely",
          description:
            "It is a long established fact that a reader will be distracted by the readable content",
          image:
            "https://res.cloudinary.com/collinskreation/image/upload/v1641320549/IMG_1947_ksmjda.jpg",
        },
        {
          title: "Homely",
          description:
            "It is a long established fact that a reader will be distracted by the readable content",
          image:
            "https://res.cloudinary.com/collinskreation/image/upload/v1641320549/IMG_1947_ksmjda.jpg",
        },
        {
          title: "Homely",
          description:
            "It is a long established fact that a reader will be distracted by the readable content",
          image:
            "https://res.cloudinary.com/collinskreation/image/upload/v1641320549/IMG_1947_ksmjda.jpg",
        },
        {
          title: "Homely",
          description:
            "It is a long established fact that a reader will be distracted by the readable content",
          image:
            "https://res.cloudinary.com/collinskreation/image/upload/v1641320549/IMG_1947_ksmjda.jpg",
        },
      ],
    };
  },
};
</script>

<style>
</style>