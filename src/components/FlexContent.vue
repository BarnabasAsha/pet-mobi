<template>
  <div
    class="flex_content"
    :style="reversed ? { flexDirection: 'row-reverse' } : ''"
  >
    <div
      class="flex_content_text"
      :style="reversed ? { marginLeft: '0', marginRight: '5%' } : ''"
    >
      <h3>{{ title }}</h3>
      <p>{{ content }}</p>
    </div>
    <div
      class="flex_content_img"
      :style="imgGutter ? { marginRight: '5%' } : ''"
    >
      <img :src="require(`../assets/images/${img}.png`)" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "FlexContent",
  props: {
    title: String,
    content: String,
    img: String,
    reversed: Boolean,
    imgGutter: Boolean,
  },
};
</script>

<style lang="scss" src="../styles/flexContent.scss"></style>
