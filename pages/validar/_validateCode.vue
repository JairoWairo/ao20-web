<template>
  <div></div>
</template>

<script>
export default {
  async asyncData({ redirect, $axios, params }) {
    try {
      await $axios.post(`/accounts/validate/${params.validateCode}`);
      return redirect("/?validada=1");
    } catch (e) {
      return redirect("/");
    }
  },
};
</script>
