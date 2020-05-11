<template>
  <div>
    <div class="navigation bg-primary py-3 px-5 text-center">
      <button class="bg-white text-black" v-if="$auth.loggedIn" @click="logout">Logout</button>
      <button class="bg-white text-black" v-if="!$auth.loggedIn" @click="login">Login</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    login() {
      window.location.href = "/auth/login";
    },
    logout() {
      window.location.href = "/auth/logout";
    }
  }
};
</script>