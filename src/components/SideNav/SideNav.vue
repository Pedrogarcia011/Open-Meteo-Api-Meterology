<template>
  <div class="body">
    <v-app-bar-nav-icon class="mobile_menu" ></v-app-bar-nav-icon >
    <v-main>
      <router-view></router-view>
    </v-main>
  </div>
</template>

<script>
import { routesList } from "@/router/routesList";

export default {
  data: () => {
    return {
      // data
      routesList,
    };
  },

  props: {},
  component: {},
};
</script>

<style scoped>
.body {
  display: flex;
  flex-direction: row;
}
.mobile_menu{
  display: none;
}

@media (max-width: 850px) {
  .mobile_menu{
  display: flex;
}
.desktop_menu{
  display: none;
}
}
</style>
