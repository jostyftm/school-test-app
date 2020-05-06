<template>
  <div class="p-4">
    <!-- Header -->
    <div class="mb-8">
      <div class="flex justify-between items-center border-b border-gray-500">
        <h1 class="font-semibold text-lg md:text-2xl">Instituciones</h1>
        <nuxt-link
          :to="{ name: 'auth-login' }"
          class="text-center my-4 px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
        >
          Crear institución
        </nuxt-link>
      </div>
    </div>
    <!-- Content -->
    <div
      class="bg-white border border-gray-300 shadow-sm rounded-lg py-2 overflow-auto"
    >
      <simple-table
        :headings="headings"
        :data="institutions"
        :loading="loading"
      />
    </div>
  </div>
</template>

<script>
import institutionsQuery from "~/graphql/institutions/institutions.graphql"
import simpleTable from "~/components/tables/SimpleTable"
export default {
  layout: "dashboard",
  components: { simpleTable },
  data() {
    return {
      headings: ["ID", "Nombre", "Avatar"],
      institutions: [],
      loading: true
    }
  },
  mounted() {
    this.getInstitutions()
  },
  methods: {
    async getInstitutions() {
      const response = await this.$apollo.query({
        query: institutionsQuery,
        variables: {
          first: 10,
          page: 1
        }
      })
      this.institutions = response.data.institutions.data
      this.loading = this.$apollo.loading
    }
  }
}
</script>
