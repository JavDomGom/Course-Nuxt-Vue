<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRbRgucQ5ANNoAXfK8VZgiNb46V9C0D8xL-UA&usqp=CAU"
      title="Hello there!"
      previewText="This is my first post!"
    />
    <PostPreview
      id="2"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRbRgucQ5ANNoAXfK8VZgiNb46V9C0D8xL-UA&usqp=CAU"
      title="Hello there - the second time!"
      previewText="This is my second post!"
    />
    <PostPreview
      id="3"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRbRgucQ5ANNoAXfK8VZgiNb46V9C0D8xL-UA&usqp=CAU"
      title="Hi!"
      previewText="This is my third post!"
    />
  </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";

export default {
  components: {
    PostPreview,
  },
  props: {
    isAdmin: Boolean,
    default: false,
  },
};
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>