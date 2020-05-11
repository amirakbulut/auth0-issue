<template>
  <div>
    <pre></pre>
  </div>
</template>

<script>
export default {
  mounted() {
    // Try to get an access token using the 'code' parameter (returns 401 Unauthorized)
    this.$axios
      .$post(
        "https://" + process.env.AUTH0_DOMAIN + "/oauth/token",
        {
          grant_type: "authorization_code",
          client_id: process.env.AUTH0_CLIENT_ID,
          client_secret: process.env.AUTH0_CLIENT_SECRET,
          code: this.$route.query.code,
          redirect_uri: "http://mysalon.test/callback"
        },
        {
          headers: {
            "Content-Type": "application/x-www-form-urlencoded"
          }
        }
      )
      .then(response => {
        console.log(response);
      })
      .catch(error => {
        if (this.$axios.isCancel(error)) {
          console.log("Request canceled", error);
        } else {
          // handle error
        }
      });
  }
};
</script>
