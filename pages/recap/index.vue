<template>
  <main>
    <section v-if="posts" class="w-full max-w-5xl mx-auto">
      <h1 class="title">Recaps from 21</h1>
      <posts post-type="recap" :amount="10" />
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, error }) {
    let posts;
    try {
      posts = await $content("recap").fetch();
    } catch (e) {
      error({ message: "Recap posts not found" });
    }
    return { posts };
  },
}
</script>
