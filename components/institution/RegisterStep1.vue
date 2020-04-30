<template>
  <div>
    <div class="px-4 my-4">
      <h2 class="text-center font-semibold text-xl">
        Datos de la institución
      </h2>
      <p class="text-gray-600">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci iusto
        ullam porro dolor, recusandae minus cupiditate cum enim!
      </p>
    </div>
    <div class="px-4 w-2/3 mx-auto">
      <div
        class="mb-6 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
      >
        <label for="" class="text-gray-700">Nombre de la institución*</label>
        <input
          type="email"
          name="email"
          class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
          placeholder="tucorreo@mail.com"
          required
        />
        <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
      </div>
      <div
        class="mb-6 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
      >
        <label for="" class="text-gray-700">
          Correo electronico de la institución*
        </label>
        <input
          type="email"
          name="email"
          class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
          placeholder="tucorreo@mail.com"
          required
        />
        <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
      </div>
    </div>
  </div>
</template>
