<template>
  <div class="flex w-full">
    <main class="bg-primary-700">
      <nav class="m-6" aria-label="go back">
        <router-back class="block" />
      </nav>
      <article v-if="post" class="w-full py-10">
        <h1>{{ post.title }}</h1>
        <h6>
          {{ post.subtitle }} • <span v-if="post.createdAt">{{ formatDate(post.createdAt) }}</span>
        </h6>
        <p class="mt-1 mb-4">
          {{ post.description }}
        </p>
        <nuxt-content :document="post" />
      </article>
    </main>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params, error }) {
    let post
    try {
      post = await $content('work', params.work).fetch()
    } catch (e) {
      error({ message: 'Work post not found' })
    }
    return { post }
  },
  methods: {
    formatDate(dateString) {
      const date = new Date(dateString)
      return date.toLocaleDateString(process.env.lang) || ''
    },
  },
}
</script>