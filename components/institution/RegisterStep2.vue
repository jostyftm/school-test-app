<template>
  <div>
    <div class="px-4 my-4">
      <h2 class="text-center font-semibold text-xl">
        Datos del representante
      </h2>
      <p class="text-gray-600">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci iusto
        ullam porro dolor, recusandae minus cupiditate cum enim!
      </p>
    </div>
    <div class="px-4 w-2/3 mx-auto">
      <!-- First row -->
      <div class="flex justify-between">
        <div
          class="mb-6 mx-2 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
        >
          <label for="" class="text-gray-700">Nombres*</label>
          <input
            type="text"
            name="name"
            class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
            placeholder="Jhon joe"
            required
          />
          <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
        </div>
        <div
          class="mb-6 mx-2 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
        >
          <label for="" class="text-gray-700">
            Apellidos*
          </label>
          <input
            type="text"
            name="last_name"
            class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
            placeholder="Doe Smith"
            required
          />
          <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
        </div>
      </div>
      <!-- Second row -->
      <div class="flex justify-between">
        <div
          class="mb-6 mx-2 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
        >
          <label for="" class="text-gray-700">Tipo de identificación*</label>
          <select
            name="identification_type_id"
            class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
          >
            <option>Seleccione un tipo de documento</option>
          </select>
          <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
        </div>
        <div
          class="mb-6 mx-2 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
        >
          <label for="" class="text-gray-700">
            Número de documneto*
          </label>
          <input
            type="text"
            name="document_number"
            class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
            placeholder="1234567895"
            required
          />
          <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
        </div>
      </div>
      <!-- Third row -->
      <div class="flex justify-between">
        <div
          class="mb-6 mx-2 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
        >
          <label for="" class="text-gray-700">
            Correo electronico*
          </label>
          <input
            type="email"
            name="email"
            class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
            placeholder="jhondoe@mail.com"
            required
          />
          <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
        </div>
        <div
          class="mb-6 mx-2 rounded focus-within:border-gray-500 flex flex-col justify-between w-full border-b-2 border-gray-200"
        >
          <label for="" class="text-gray-700">
            Contraseña*
          </label>
          <input
            type="password"
            name="password"
            class="p-2 rounded-none rounded-t flex-1 focus:outline-none bg-gray-100"
            placeholder="1234567895"
            required
          />
          <!-- <div class="h-4 w-4 bg-gray-200"></div> -->
        </div>
      </div>
    </div>
  </div>
</template>
