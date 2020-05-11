<template>
  <div></div>
</template>

<script>
export default {
  beforeMount() {
    this.$auth.loginWith("auth0");
  }
};
</script>
