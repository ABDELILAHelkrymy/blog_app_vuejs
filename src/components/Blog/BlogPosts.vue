<template>
  <div class="post-box">
    <span class="post-views">{{ views }}</span>
    <h1 class="post-title">{{ title }}</h1>
    <span class="post-date">{{ date }}</span>
    <p class="post-content">{{ content }}</p>
    <div class="row">
      <div class="col-md-6">
        <span class="post-author">{{ author }}</span>
      </div>
      <div class="col-md-6 text-end">
        <span class="post-category">{{ category | uppercase }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["views", "title", "date", "content", "author", "category"],
  name: "postView",
};
</script>

<style lang="scss" scoped>
.post-box {
  padding: 15px;
  background-color: #fff;
  box-shadow: 0 0 10px #ddd;
  position: relative;
  text-align: left;
  margin-bottom: 20px;
  .post-views {
    position: absolute;
    top: 5px;
    right: 5px;
    background-color: #4caf50;
    border-radius: 4px;
    padding: 1px 5px;
    color: #fff;
    text-align: center;
    font-weight: bold;
  }
  .post-title {
    font-weight: bold;
  }
  .post-date {
    display: block;
    padding: 0 0 5px;
    color: #888;
    font-size: 14px;
  }
  .post-content {
    line-height: 1.8;
    color: #666;
  }
  .post-author {
    background-color: #607d8b;
    padding: 6px 10px;
    border-radius: 4px;
    color: #fff;
  }
  .post-category {
    background-color: #e91e63;
    padding: 6px 10px;
    border-radius: 4px;
    color: #fff;
  }
}
</style>
