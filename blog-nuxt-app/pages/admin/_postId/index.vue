<template>
  <div class="admin-post-pag">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";

export default {
  layout: "admin",
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        auth: "Javier",
        title: "My awesome Post",
        content: "Super amazing, thanks for that!",
        thumbnailLink:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRbRgucQ5ANNoAXfK8VZgiNb46V9C0D8xL-UA&usqp=CAU",
      },
    };
  },
};
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>