<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-md-8">
        <div class="card">
          <div class="card-header">Example Component</div>

          <div class="card-body">I'm an example component.</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    getUserData() {
      axiosAdmin.get("api/user").then((r) => {
        console.log(r);
      });
    },
  },
  mounted() {
    console.log("Component mounted.");
  },
  created() {
    this.getUserData();
  },
};
</script>
