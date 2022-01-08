<template>
  <div class="featured">
    <h2>Featured In</h2>
    <div class="featured_grid">
      <div class="forbes">
        <img src="../assets/images/forbes.png" alt="" />
      </div>
      <div class="guardian">
        <img src="../assets/images/theguardian.png" alt="" />
      </div>
      <div class="techradar">
        <img src="../assets/images/techradar.png" alt="" />
      </div>
    </div>
    <div class="featured_gif">
      <img src="../assets/images/dog-gif.png" alt="" />
    </div>
    <div class="featured_details">
      <div class="featured_details_item">
        <div class="count">273k</div>
        <div class="title">Clients served</div>
      </div>
      <div class="featured_details_item">
        <div class="count">300k</div>
        <div class="title">Downloads</div>
      </div>
      <div class="featured_details_item">
        <div class="count">16k</div>
        <div class="title">Care givers</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Featured",
};
</script>

<style lang="scss" src="../styles/featured.scss"></style>
