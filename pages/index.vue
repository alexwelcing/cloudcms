<template>
  <main>
    <section class="mt-8 self-center flex flex-col flex-1 items-center justify-center">
      <h1 class="title text-center">20 — 22 projects — 22</h1>
      <h2 class="subtitle text-center">Interactive project planning.</h2>
    </section>

    <section class="mt-8">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-5xl mx-auto">Latest projects</h3>
      <posts post-type="projects" :amount="3" />
    </section>
  </main>
</template>