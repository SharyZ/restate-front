<template>
  <div class="login-page">
    <Form @onSubmit="userLogin">
      <template #form-header>
        <h2>Login to your account</h2>
      </template>
      <FormControl>
        <FormLabel for="username">Username</FormLabel>
        <FormInput
          v-model="username"
          required
          type="text"
          id="username"
          name="username"
          placeholder="Username"
        />
        <FormInputError>
          <p>Username is not correct.</p>
        </FormInputError>
      </FormControl>
      <FormControl>
        <div class="flex items-center justify-between">
          <FormLabel for="password">Password</FormLabel>
          <NuxtLink class="mb-2" to="/forgot-password">
            Forgot your password?
          </NuxtLink>
        </div>
        <FormInput
          v-model="password"
          required
          type="password"
          id="password"
          name="password"
          placeholder="Password"
        />
        <FormInputError>
          <p>Password must be more than 6 characters.</p>
        </FormInputError>
      </FormControl>
      <FormButton>Login</FormButton>
      <template #form-footer>
        <p>
          Don't have an account?
          <NuxtLink to="/signup" class="text-blue-500">Signup now</NuxtLink>
        </p>
      </template>
    </Form>
  </div>
</template>

<script>
export default {
  name: 'LoginPage',

  layout: 'fullscreen',

  middleware: ['isAuthenticated'],

  data() {
    return {
      username: '',
      password: '',
    }
  },

  methods: {
    async userLogin() {
      const { username, password } = this

      await this.$auth
        .loginWith('local', {
          data: {
            username,
            password,
          },
        })
        .then((response) => {
          const token = response.data.auth_token

          this.$auth.setUserToken(token)
          this.$toast.success('Successfully loggedin')
        })
        .catch((error) => {
          this.$toast.error('Incorrect login or password!')
        })
    },
  },
}
</script>

<style lang="css" scoped>
.login-page {
  @apply flex min-h-screen items-center justify-center;
}
</style>
