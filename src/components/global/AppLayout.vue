<template>
  <div class="layout">
    <v-layout>
      <!-- Start::Cart Drawer Component -->
      <CartDrawer />
      <!-- End::Cart Drawer Component -->
      <!-- Start::Navigation Component -->
      <AppNavigation />
      <!-- End::Navigation Component -->
      <v-main>
        <slot></slot>
      </v-main>
      <!-- Start::Footer Component -->
      <AppFooter />
      <!-- End::Footer Component -->
    </v-layout>
  </div>
</template>

<script>
import AppNavigation from "@/components/global/AppNavigation.vue";
import AppFooter from "@/components/global/AppFooter.vue";
import CartDrawer from "@/components/global/CartDrawer.vue";

export default {
  data() {
    return {};
  },
  components: {
    AppNavigation,
    AppFooter,
    CartDrawer,
  },
};
</script>
