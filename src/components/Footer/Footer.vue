<template>
  <div class="footer">
    <FooterItem
      v-for="item in myitems"
      :key="item.title"
      :title="item.title"
      :list="item.list"
    />
  </div>
</template>

<script>
import { ref } from "vue";
import FooterItem from "./FooterItem.vue";

export default {
  name: "Footer",
  components: {
    FooterItem,
  },
  setup() {
    const myitems = ref([
      {
        title: "Services",
        list: ["Dog Grooming", "Dog Walking", "Dog Watching"],
      },
      {
        title: "About Us",
        list: ["The Team", "Partners"],
      },
      {
        title: "Learn More",
        list: ["How it works", "Terms and conditions"],
      },
      {
        title: "App",
        list: ["Download app"],
      },
      {
        title: "Community",
        list: ["Join Community"],
      },
    ]);
    return { myitems };
  },
};
</script>
