<template>
  <Page>
    <ActionBar title="Welcome to NativeScript-Vue!"/>
    <StackLayout columns="*" rows="*">
      <DateTextField/>
      <FloatText :eidtable="true"/>
      <DateTextField ref="txtDesc"/>
      <Button @tap="focusItem" text="focus last field"/>
    </StackLayout>
  </Page>
</template>

<script>
import SecondPage from "./SecondPage";
import FloatText from "./sub/FloatText";
import DateTextField from "./sub/DateTextField";

export default {
  data() {
    return {
      msg: "Hello World!"
    };
  },
  methods: {
    nav() {
      this.$navigateTo(SecondPage, {
        transition: { name: "slide", duration: 370 }
      });
    },
    focusItem() {
        console.log('foc');
      this.$refs.txtDesc.nativeView.focus();
    }
  },
  components: {
    DateTextField,
    FloatText
  }
};
</script>

<style scoped>
ActionBar {
  background-color: #53ba82;
  color: #ffffff;
}

.message {
  vertical-align: center;
  text-align: center;
  font-size: 20;
  color: #333333;
}
</style>
