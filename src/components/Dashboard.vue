<template>
  <div class="d-flex" id="wrapper">
    <Sidebar msg="Welcome to Your Vue.js App" />
    <div id="page-content-wrapper">
      <Navbar />
      <div class="container-fluid">
        <router-view />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Sidebar from "@/components/dashboard/Sidebar.vue";
import Navbar from "@/components/dashboard/Navbar.vue";

export default {
  name: "Dashboard",
  components: {
    Sidebar,
    Navbar,
  },
  mounted: function(){
    
  }
};

</script>
<style scoped>
.container-fluid {
  padding: 20px;
}
</style>
