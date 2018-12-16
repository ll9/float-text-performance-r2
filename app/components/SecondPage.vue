<template>
  <Page>
    <ScrollView>
      <StackLayout>
        <StackLayout class="form-group">
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
        </StackLayout>
        <StackLayout class="form-group">
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
        </StackLayout>
        <StackLayout class="form-group">
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
        </StackLayout>
        <StackLayout class="form-group">
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
        </StackLayout>
        <StackLayout class="form-group">
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
        </StackLayout>
        <StackLayout class="form-group">
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
          <FloatTextField hint="hint" v-model="msg"/>
        </StackLayout>
      </StackLayout>
    </ScrollView>
  </Page>
</template>

<script>
import FloatTextField from "./sub/FloatText";

export default {
  data() {
    return {
      msg: "Hello World!"
    };
  },
  components: {
    FloatTextField
  }
};
</script>

<style scoped>

.form-group {
    border-color: black;
    border-width: 2;
    border-radius: 5;
    margin: 10;
}

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
