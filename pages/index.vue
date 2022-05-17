<template>
  <div>
    <section class="my-20">
      <div class="mx-auto mb-20 max-w-2xl text-center">
        <h1 class="mb-6 text-7xl font-black leading-[80px]">
          Your perfect home is waiting for you
        </h1>
        <p class="mb-8 text-lg font-medium">
          We have more than 200k properties around to world to show you
        </p>
        <div>
          <NuxtLink
            to="/explore"
            class="inline-block rounded-lg bg-rose-400 py-2 px-4 text-lg font-semibold text-white"
          >
            Explore more
          </NuxtLink>
        </div>
      </div>
      <div class="mx-auto max-w-4xl rounded-lg bg-slate-50 p-6 shadow-md">
        <form class="search-form">
          <div>
            <label for="location">Location</label>
            <input
              type="text"
              id="location"
              name="location"
              placeholder="Toronto"
            />
          </div>
          <div>
            <label for="type">Type</label>
            <input type="text" id="type" name="type" placeholder="Apartment" />
          </div>
          <div>
            <label for="price">Price range</label>
            <input type="number" id="price" name="price" placeholder="300k" />
          </div>
          <div class="flex-grow">
            <button type="search">Search</button>
          </div>
        </form>
      </div>
    </section>
    <section class="my-20">
      <div class="flex items-center space-x-8">
        <div class="w-1/2">
          <img src="~/assets/images/home01.jpg" alt="" class="rounded-2xl" />
        </div>
        <div class="w-1/2">
          <h2 class="mb-4 text-5xl font-semibold leading-[60px]">
            We are the best and most trusted
            <span class="text-blue-500">Real estate agent</span>
          </h2>
          <p class="mb-8 text-lg font-medium">
            We've helped a lot of people to find their dream homes
          </p>
          <ul class="flex flex-col space-y-6">
            <li class="flex items-center space-x-4">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-10 w-10 rounded-full bg-blue-50 p-1 text-blue-500"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                stroke-width="2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M5 13l4 4L19 7"
                />
              </svg>
              <span class="text-xl font-medium">
                678k buys have worked with us
              </span>
            </li>
            <li class="flex items-center space-x-4">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-10 w-10 rounded-full bg-blue-50 p-1 text-blue-500"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                stroke-width="2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M5 13l4 4L19 7"
                />
              </svg>
              <span class="text-xl font-medium">
                Professional and experienced resources
              </span>
            </li>
            <li class="flex items-center space-x-4">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-10 w-10 rounded-full bg-blue-50 p-1 text-blue-500"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                stroke-width="2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M5 13l4 4L19 7"
                />
              </svg>
              <span class="text-xl font-medium">
                Provide the best service for users
              </span>
            </li>
          </ul>
        </div>
      </div>
    </section>
    <SpecialHomes />
    <OurService />
    <BlogPosts />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style scoped>
.search-form {
  @apply flex items-center space-x-4;
}

.search-form label {
  @apply mb-2 block text-lg font-medium;
}

.search-form input {
  @apply rounded-md border-none;
}

.search-form button {
  @apply block w-full rounded-md border-none bg-blue-500 py-2 text-lg font-semibold text-white shadow-md;
}
</style>
