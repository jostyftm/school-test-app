<template>
  <div class="p-4 w-2/3 mx-auto">
    <div class="h-32 w-32 mx-auto bg-gray-500"></div>
    <h1 class="my-4 text-center font-bold text-xl">
      La cuenta ha sido creada exietosamente
    </h1>
    <p>
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tempore
      aspernatur fugit corrupti velit harum dolore impedit molestias est?
    </p>
    <nuxt-link
      :to="{ name: 'auth-login' }"
      class="block text-center my-4 w-full px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
    >
      Iniciar sesión
    </nuxt-link>
  </div>
</template>
