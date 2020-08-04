<!--  -->
<template>
  <div>
    <div>
      <v-alert type="success" width="800pX" elevation="20">alert.</v-alert>
    </div>
    <div style="height:80px;width:800px">
      <v-card>
        <v-responsive :aspect-ratio="16/9">
          <v-card-text>This card will always be 16:9 (unless you put more stuff in it)</v-card-text>
        </v-responsive>
      </v-card>
    </div>
    <v-row justify="center">
      <v-avatar color="indigo">
        <v-icon dark>mdi-account-circle</v-icon>
      </v-avatar>

      <v-avatar>
        <img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John" />
      </v-avatar>

      <v-avatar color="red">
        <span class="white--text headline">CJ</span>
      </v-avatar>
    </v-row>

    <v-toolbar>
      <v-tabs dark background-color="primary" grow>
        <v-tab>
          <v-badge color="pink" dot>Item One</v-badge>
        </v-tab>

        <v-tab>
          <v-badge color="green" content="6">Item Two</v-badge>
        </v-tab>

        <v-tab>
          <v-badge color="deep-purple accent-4" icon="mdi-vuetify">Item Three</v-badge>
        </v-tab>
      </v-tabs>
    </v-toolbar>

    <v-banner two-line>
      <v-avatar slot="icon" color="deep-purple accent-4" size="40">
        <v-icon icon="mdi-lock" color="white">mdi-lock</v-icon>
      </v-avatar>
Three line text string example with two actions. One to two lines is preferable. Three lines should be considered the maximum string length on desktop in order to keep messages short and actionable.
      <template
        v-slot:actions
      >
        <v-btn text color="deep-purple accent-4">Action</v-btn>
        <v-btn text color="deep-purple accent-4">Action</v-btn>
      </template>
    </v-banner>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  //生命周期 - 创建完成（访问当前this实例）
  created() {},
  //生命周期 - 挂载完成（访问DOM元素）
  mounted() {},
};
</script>
<style scoped>
/* @import url(); 引入css类 */
</style>