<template>
  <div class="signup-page">
    <Form @onSubmit="userSignup">
      <template #form-header>
        <h2>Create new account</h2>
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
        <FormLabel for="email">Email address</FormLabel>
        <FormInput
          v-model="email"
          required
          type="email"
          id="email"
          name="email"
          placeholder="Email"
        />
        <FormInputError>
          <p>Email is not correct.</p>
        </FormInputError>
      </FormControl>
      <FormControl>
        <FormLabel for="password">Password</FormLabel>
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
      <FormButton>Signup</FormButton>
      <template #form-footer>
        <p>
          Already have an account?
          <NuxtLink to="/login" class="text-blue-500">Login now</NuxtLink>
        </p>
      </template>
    </Form>
  </div>
</template>

<script>
export default {
  name: 'SignupPage',

  layout: 'fullscreen',

  middleware: ['isAuthenticated'],

  data() {
    return {
      username: '',
      email: '',
      password: '',
    }
  },

  methods: {
    async userSignup() {
      const { username, email, password } = this

      await this.$axios
        .post('auth/users/', {
          username,
          email,
          password,
        })
        .then((response) => {
          this.$auth.loginWith('local', {
            data: {
              username,
              password,
            },
          })

          this.$toast.success('Account successfully created')
          this.$router.push('/profile')
        })
        .catch(({ response }) => {
          const { data } = response

          if (data.username) {
            this.$toast.error(data.username[0])
          } else {
            this.$toast.error('Something went wrong when signup')
          }
        })
    },
  },
}
</script>

<style lang="css" scoped>
.signup-page {
  @apply flex min-h-screen items-center justify-center;
}
</style>
