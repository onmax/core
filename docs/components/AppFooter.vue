<script setup lang="ts">
const links = [
  {
    label: 'Terms',
    to: 'https://admin.hub.nuxt.com/terms',
    target: '_blank'
  }, {
    label: 'Privacy',
    to: 'https://admin.hub.nuxt.com/privacy',
    target: '_blank'
  }, {
    label: 'Status',
    to: 'https://status.hub.nuxt.com',
    target: '_blank'
  }
]
</script>

<template>
  <UFooter :links="links">
    <template #left>
      <span class="inline text-sm">© {{ new Date().getFullYear() }} <a href="https://nuxtlabs.com" target="_blank" class="text-gray-900 dark:text-gray-50 hover:underline underline-offset-4">NuxtLabs</a></span>
    </template>

    <template #right>
      <ColorScheme><UColorModeSelect /></ColorScheme>
      <UButton
        icon="i-simple-icons-discord"
        color="gray"
        variant="ghost"
        to="https://discord.gg/vW89dsVqBF"
        target="_blank"
        aria-label="Go to NuxtHub Discord server"
      />
      <UButton
        icon="i-simple-icons-x"
        color="gray"
        variant="ghost"
        to="https://x.com/nuxt_hub"
        target="_blank"
        aria-label="Go to NuxtHub X account"
      />
      <UButton
        icon="i-simple-icons-github"
        color="gray"
        variant="ghost"
        to="https://github.com/nuxt-hub/core"
        target="_blank"
        aria-label="Go to NuxtHub GitHub repository"
      />
    </template>
  </UFooter>
</template>
