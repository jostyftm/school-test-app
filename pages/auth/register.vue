<template>
  <div class="mx-auto w-2/3 shadow bg-white py-4 rounded mt-10">
    <!-- Steps -->
    <register-step1 v-show="step == 1" />
    <register-step2 v-show="step == 2" />
    <terms-and-conditions v-show="step == 3" />
    <register-step-finish v-show="step == 4" />

    <!-- Step controls -->
    <div class="w-full flex justify-between px-4">
      <button
        v-if="step > 1 && step < 4"
        class="px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
        @click="goPrevStep"
      >
        Atras
      </button>
      <button
        v-if="step < 4"
        class="px-4 py-2 rounded-full bg-gray-300 active:bg-gray-500 focus:outline-none"
        @click="goNextStep"
      >
        Continuar
      </button>
    </div>
  </div>
</template>

<script>
import RegisterStep1 from "~/components/institution/RegisterStep1"
import RegisterStep2 from "~/components/institution/RegisterStep2"
import RegisterStepFinish from "~/components/institution/RegisterStepFinish"
import TermsAndConditions from "~/components/institution/TermsAndConditions"

export default {
  components: {
    RegisterStep1,
    RegisterStep2,
    TermsAndConditions,
    RegisterStepFinish
  },
  data() {
    return {
      step: 1
    }
  },
  methods: {
    goNextStep() {
      this.step++
    },
    goPrevStep() {
      this.step--
    }
  }
}
</script>
