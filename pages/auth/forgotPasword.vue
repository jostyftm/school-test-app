<template>
  <div class="mx-auto w-4/12 shadow bg-white rounded py-4 mt-10">
    <h1 class="font-semibold text-center text-xl">Recuperar contraseña</h1>

    <div class="bg-gray-400 p-4 my-4 border-l-4 border-gray-600">
      <span>
        Se ha enviado las instrucciones al correo asas*****@gmail.com, siga los
        pasos para restablecer su contraseña
      </span>
    </div>

    <form action="" class="w-full p-4">
      <div
        class="mb-6 rounded focus-within:border-teal-500 flex justify-between w-full border-b-2 border-gray-200"
      >
        <input
          type="email"
          name="email"
          class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
          placeholder="tucorreo@mail.com"
          required
        />
        <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
      </div>
      <div class="my-4">
        <button
          class="px-4 py-2 rounded-full w-full bg-gray-300 active:bg-gray-500 focus:outline-none"
        >
          Recuperar contraseña
        </button>
      </div>
      <div class="text-center my-4">
        <span>¿Ya tienes una cuenta? ingresa </span>
        <nuxt-link :to="{ name: 'auth-login' }">
          aqui
        </nuxt-link>
      </div>
    </form>
  </div>
</template>
