<template>
  <div class="bg-white lg:h-screen lg:w-2/12 lg:border-r border-gray-500">
    <div class="my-8">
      <div class="mx-auto h-16 w-16 bg-gray-500"></div>
    </div>
    <ul>
      <li>
        <nuxt-link
          :to="{ name: 'dashboard' }"
          class="px-4 py-2 block hover:bg-gray-200 border-l-2 border-gray-500"
        >
          Inicio
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          :to="{ name: 'dashboard-institution' }"
          class="px-4 py-2 block hover:bg-gray-200"
        >
          Institución
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          :to="{ name: 'dashboard-area' }"
          class="px-4 py-2 block hover:bg-gray-200"
        >
          Areas
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          :to="{ name: 'dashboard-question' }"
          class="px-4 py-2 block hover:bg-gray-200"
        >
          Preguntas
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>
