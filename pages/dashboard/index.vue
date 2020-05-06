<template>
  <div class="p-4">
    <!-- Header -->
    <div class="mb-8">
      <div class="flex justify-between items-center border-b border-gray-500">
        <h1 class="font-semibold text-lg md:text-2xl">Titulo de la pagina</h1>
        <nuxt-link
          :to="{ name: 'auth-login' }"
          class="text-center my-4 px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
        >
          Acción rapida
        </nuxt-link>
      </div>
    </div>
    <!-- Content -->
    <div
      class="bg-white border border-gray-300 shadow-sm rounded-lg py-2 overflow-auto"
    >
      <div class="p-4 font-semibold text-gray-900">
        <h3>Titulo del panel</h3>
      </div>
      <table class="w-full">
        <thead>
          <tr>
            <th
              class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
            >
              ID
            </th>
            <th
              class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
            >
              Name
            </th>
            <th
              class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
            >
              Last name
            </th>
            <th
              class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
            >
              email
            </th>
            <th
              class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
            >
              created at
            </th>
            <th
              class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
            ></th>
          </tr>
        </thead>

        <tbody>
          <tr>
            <td class="px-4 py-4 text-gray-800 whitespace-no-wrap">
              1
            </td>
            <td class="px-4 py-4 text-gray-800 whitespace-no-wrap">
              Joe William
            </td>
            <td class="px-4 py-4 text-gray-800 whitespace-no-wrap">
              Doe Smith
            </td>
            <td class="px-4 py-4 text-gray-800 whitespace-no-wrap">
              jw@mail.com
            </td>
            <td class="px-4 py-4 text-gray-800 whitespace-no-wrap">
              3 days ago
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  layout: "dashboard"
}
</script>
