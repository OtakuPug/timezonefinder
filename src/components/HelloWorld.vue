<template>
  <v-container class="fill-height" max-width="900">
    <div>


      <div class="mb-8 text-center">
        <h1 class="text-h2 font-weight-bold">Current IANA Timezone: {{ timezone }}</h1>
      </div>

    </div>
  </v-container>
</template>

<script setup lang="ts">

  const timezone = Intl.DateTimeFormat().resolvedOptions().timeZone
  const links = [
    {
      href: 'https://vuetifyjs.com/',
      icon: 'mdi-text-box-outline',
      subtitle: 'Learn about all things Vuetify in our documentation.',
      title: 'Documentation',
    },
    {
      href: 'https://vuetifyjs.com/introduction/why-vuetify/#feature-guides',
      icon: 'mdi-star-circle-outline',
      subtitle: 'Explore available framework Features.',
      title: 'Features',
    },
    {
      href: 'https://vuetifyjs.com/components/all',
      icon: 'mdi-widgets-outline',
      subtitle: 'Discover components in the API Explorer.',
      title: 'Components',
    },
    {
      href: 'https://discord.vuetifyjs.com',
      icon: 'mdi-account-group-outline',
      subtitle: 'Connect with Vuetify developers.',
      title: 'Community',
    },
  ]
</script>
