<script setup lang="ts">
import ModulesBarLink from "~/components/docs/ModulesBarLink.vue";
const props = defineProps({
  currentPageId: String,
})
</script>

<template>
  <div
      class="fixed z-10 bg-gray-100 dark:bg-pickled-bluewood-800/80 w-full pt-2 pb-2.5 grid place-items-center"
      style="backdrop-filter: var(--elements-backdrop-filter)"
  >
    <div class="flex items-center gap-2">
      <ModulesBarLink
          title="nuxt-auth"
          icon="heroicons-outline:lock-closed"
          href="/nuxt-auth"
          :current-page-id="currentPageId"
      />
      <ModulesBarLink
          title="nuxt-session"
          icon="heroicons-outline:clock"
          href="/nuxt-session"
          :current-page-id="currentPageId"
      />
      <ModulesBarLink
          title="nuxt-parse"
          icon="heroicons-outline:funnel"
          href="/nuxt-parse"
          :current-page-id="currentPageId"
      />
      <ModulesBarLink
          title="nuxt-pdf"
          icon="heroicons-outline:document"
          href="/nuxt-pdf"
          :current-page-id="currentPageId"
      />
    </div>
  </div>
</template>
