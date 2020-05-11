<template>
  <div></div>
</template>

<script>
export default {
  beforeMount() {
    this.logout();
  },
  methods: {
    async logout() {
      await this.$auth.logout();

      window.location.href =
        "https://" +
        process.env.AUTH0_DOMAIN +
        "/v2/logout?returnTo=localhost%3A3000&client_id=" +
        process.env.AUTH0_CLIENT_ID;
    }
  }
};
</script>
