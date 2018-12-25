<template>
    <FloatTextField v-model="value" :hint="hint" @focus="getDate" :editable="false"></FloatTextField>
</template>

<script>
import Vue from "vue";
import DateService from "../../utils/DateService.js";
import FloatTextField from "./FloatText";
const Service = new DateService();
export default Vue.extend({
  props: ["value", "hint"],
  data() {
    return {
      isActive: false,
    }
  },
  methods: {
    async getDate() {
      if (this.isActive == false) {
        this.isActive = true;
        this.value = await Service.getDate();
        this.isActive = false;
      }
      this.$emit("input", this.value);
    }
  },
  components: {
    FloatTextField
  }
});
</script>

<style scoped lang="scss">
</style>