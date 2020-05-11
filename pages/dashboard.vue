<template>
  <div>
    <div class="navigation bg-black py-3 px-5 text-center">
      <button class="bg-primary text-white" v-if="$auth.loggedIn" @click="logout">Logout</button>
      <pre class="my-5 text-white">
        {{this.$auth.user}}
        </pre>
      <pre class="my-5 text-white">
        {{this.$auth.getToken("auth0")}}
        </pre>
    </div>
  </div>
</template>

<script>
export default {
  middleware: "auth",
  methods: {
    logout() {
      window.location.href = "/auth/logout";
    }
  }
};
</script>
