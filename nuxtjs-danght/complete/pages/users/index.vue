<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="onLoadUsers">Load User</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: '',
    }
  },
  methods: {
    onLoadUsers: function () {
      this.$route.push('/users/' + this.userId)
    },
  },
}
</script>

<style></style>
