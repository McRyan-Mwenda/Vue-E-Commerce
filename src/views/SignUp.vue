<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="my-16">
    <p class="text-2xl text-center mb-4">Create account</p>
    <form class="bg-blue-400 px-8 py-4 rounded-md">
      <div class="form-field">
        <label for="username" class="form-label">Username</label>
        <input
          type="text"
          name="username"
          class="form-input"
          placeholder="your username"
        />
      </div>
      <div class="form-field">
        <label for="email" class="form-label">Email</label>
        <input
          type="email"
          name="email"
          class="form-input"
          placeholder="your email address"
        />
      </div>
      <div class="form-field">
        <label for="password" class="form-label">Password</label>
        <input
          type="password"
          name="password"
          class="form-input"
          placeholder="**********"
        />
      </div>
      <div class="form-field">
        <label for="password-2" class="form-label">Confirm password</label>
        <input
          type="password"
          name="password-2"
          class="form-input"
          placeholder="**********"
        />
      </div>
      <button type="submit" class="form-submit">Sign Up</button>
    </form>
    <p class="text-center my-4 text-lg">
      Already have an account?
      <RouterLink
        to="/sign-in"
        class="text-blue-500 hover:text-blue-600 underline"
        >Go to log in</RouterLink
      >.
    </p>
  </div>
</template>

<script></script>

<style scoped>
form {
  width: 40%;
  margin: auto;
}
</style>
