<template>
    <div class="min-h-screen flex flex-col bg-base-200">
      <AppHeader />
      <main class="flex-1 w-full max-w-5xl mx-auto px-2 sm:px-4 py-4">
        <!-- slot cela va servir à injecter le contenu de la page dans le layout on utilise le layout dans app.vue (<NuxtLayout>, <NuxtPage /> pour faire le rendu des la page car dans Nuxt on a le router automatique) -->
        <slot />
      </main>
      <AppFooter />
    </div>
  </template>