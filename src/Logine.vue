<template>
  <div>
    <h1>Login Page</h1>
    <form @submit.prevent="login">
      <label for="username">Username:</label>
      <input type="text" v-model="username" required />
      <label for="password">Password:</label>
      <input type="password" v-model="password" required />
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: ''
    };
  },
  methods: {
    login() {
      // Ajoutez ici la logique d'authentification
      console.log('Login:', this.username);
    }
  }
};
</script>

<style scoped>
/* Ajoutez vos styles ici */
</style>
