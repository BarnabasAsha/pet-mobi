<template>
  <div class="flex_wrapper">
    <FlexContent
      v-for="content in contents"
      :key="content.title"
      :title="content.title"
      :img="content.img"
      :content="content.content"
      :reversed="content.reversed"
      :imgGutter="content.imgGutter"
    />
  </div>
</template>

<script>
import FlexContent from "./FlexContent.vue";
import { ref } from "vue";

export default {
  name: "FlexWrapper",
  components: {
    FlexContent,
  },
  setup() {
    const contents = ref([
      {
        title: "Dog Grooming",
        content:
          "We use cage-free drying techniques with industrial dryers and our groomers are both qualified on all breeds of dogs and cats as well as all the cuts and styles.",
        img: "dog-grooming",
        reversed: false,
      },
      {
        title: "Dog Walkers",
        content:
          "We  provide dog walking when you are unable to, and we pick them up and drop them off in our fully equipped pet taxi.",
        img: "dog-walkers",
        reversed: true,
      },
      {
        title: "Dog Sitters",
        content:
          "We provide certified sitters to come and stay in your home in a guest room to care for your dog while you’re away.",
        img: "dog-sitters",
        reversed: false,
        imgGutter: true,
      },
    ]);
    return { contents };
  },
};
</script>

<style lang="scss" style="../styles/flexContent.scss"></style>
