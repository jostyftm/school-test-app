<template>
  <div class="flex flex-col lg:flex-row">
    <sidebar />
    <div class="lg:w-10/12">
      <nuxt />
    </div>
  </div>
</template>

<script>
import Sidebar from "~/components/Dashboard/Sidebar"

export default {
  components: { Sidebar }
}
</script>
