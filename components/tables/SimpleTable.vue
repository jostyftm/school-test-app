<template>
  <table class="w-full">
    <thead>
      <tr>
        <th
          v-for="(heading, index) in headings"
          :key="index"
          class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
        >
          {{ heading }}
        </th>
        <th
          class="px-4 py-2 text-left text-gray-600 bg-gray-100 border-b border-t"
        ></th>
      </tr>
    </thead>
    <tbody>
      <tr v-if="loading">
        <td :colspan="columns">Cargando</td>
      </tr>
      <tr v-for="item in data" v-else :key="item.id">
        <td
          v-for="field in item"
          :key="`${field}.${item.id}`"
          class="px-4 py-4 text-gray-800 whitespace-no-wrap"
        >
          {{ field }}
        </td>
        <td class="px-4 py-4 text-gray-800 whitespace-no-wrap">
          <button
            class="text-center my-4 px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
            @click="editRecord(item)"
          >
            Editar
          </button>
          <button
            class="text-center my-4 px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
            @click="deleteRecord(item)"
          >
            Eliminar
          </button>
        </td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  props: {
    headings: {
      type: Array,
      required: true
    },
    data: {
      type: Array,
      required: true
    },
    loading: {
      type: Boolean,
      required: false,
      default: false
    }
  },
  computed: {
    columns() {
      return this.headings.lenghth + 1
    }
  },
  methods: {
    editRecord(record) {
      this.$emit("editRecord", record)
    },
    deleteRecord(record) {
      this.$emit("deleteRecord", record)
    }
  }
}
</script>
