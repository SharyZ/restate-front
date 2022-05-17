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
    <section class="my-20">
      <div class="mb-8 text-center">
        <h2 class="mb-4 text-5xl font-semibold leading-[60px]">
          Special Homes
        </h2>
        <p class="mb-8 text-lg font-medium">
          Find your place with an immersive photo experience and the most
          listings, including things you won't find anywhere else.
        </p>
      </div>
      <div class="grid grid-cols-3 gap-10">
        <div class="overflow-hidden rounded-2xl">
          <img src="~/assets/images/home02.jpg" alt="" />
          <div class="mb-4 p-4">
            <div class="flex items-center space-x-4">
              <div class="flex-grow">
                <h3 class="mb-2 text-4xl font-semibold">$4,600,000</h3>
                <p>50 Canary Cres, Toronto</p>
              </div>
              <div
                class="rounded-md bg-blue-200 px-2 py-1 font-semibold text-blue-900"
              >
                For sale
              </div>
            </div>
          </div>
          <NuxtLink
            to="/"
            class="block w-full bg-rose-400 p-2 text-center font-semibold text-white"
          >
            View details
          </NuxtLink>
        </div>
        <div class="overflow-hidden rounded-2xl">
          <img src="~/assets/images/home02.jpg" alt="" />
          <div class="mb-4 p-4">
            <div class="flex items-center space-x-4">
              <div class="flex-grow">
                <h3 class="mb-2 text-4xl font-semibold">$4,600,000</h3>
                <p>50 Canary Cres, Toronto</p>
              </div>
              <div
                class="rounded-md bg-blue-200 px-2 py-1 font-semibold text-blue-900"
              >
                For sale
              </div>
            </div>
          </div>
          <NuxtLink
            to="/"
            class="block w-full bg-rose-400 p-2 text-center font-semibold text-white"
          >
            View details
          </NuxtLink>
        </div>
        <div class="overflow-hidden rounded-2xl">
          <img src="~/assets/images/home02.jpg" alt="" />
          <div class="mb-4 p-4">
            <div class="flex items-center space-x-4">
              <div class="flex-grow">
                <h3 class="mb-2 text-4xl font-semibold">$4,600,000</h3>
                <p>50 Canary Cres, Toronto</p>
              </div>
              <div
                class="rounded-md bg-blue-200 px-2 py-1 font-semibold text-blue-900"
              >
                For sale
              </div>
            </div>
          </div>
          <NuxtLink
            to="/"
            class="block w-full bg-rose-400 p-2 text-center font-semibold text-white"
          >
            View details
          </NuxtLink>
        </div>
      </div>
    </section>
    <section class="my-20">
      <div class="mb-8 text-center">
        <h2 class="mb-4 text-5xl font-semibold leading-[60px]">Our Service</h2>
        <p class="mb-8 text-lg font-medium">
          When it comes to real estate and properties, we're very happy step of
          the way
        </p>
      </div>
      <div class="grid grid-cols-3 gap-14">
        <div class="text-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="mx-auto h-14 w-14 rounded-full bg-blue-50 p-4 text-blue-500"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
            />
          </svg>
          <div class="mb-4 p-4">
            <h3 class="mb-2 text-3xl font-semibold">Property Insurance</h3>
            <p>
              Property insurance provides protection against most risks to
              property, such as fire, theft.
            </p>
          </div>
        </div>
        <div class="text-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="mx-auto h-14 w-14 rounded-full bg-blue-50 p-4 text-blue-500"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M20 13V6a2 2 0 00-2-2H6a2 2 0 00-2 2v7m16 0v5a2 2 0 01-2 2H6a2 2 0 01-2-2v-5m16 0h-2.586a1 1 0 00-.707.293l-2.414 2.414a1 1 0 01-.707.293h-3.172a1 1 0 01-.707-.293l-2.414-2.414A1 1 0 006.586 13H4"
            />
          </svg>
          <div class="mb-4 p-4">
            <h3 class="mb-2 text-3xl font-semibold">Advantage</h3>
            <p>
              All these properties have amazing prices, and you will find
              thousands of properties to choose from.
            </p>
          </div>
        </div>
        <div class="text-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="mx-auto h-14 w-14 rounded-full bg-blue-50 p-4 text-blue-500"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M3 10h18M7 15h1m4 0h1m-7 4h12a3 3 0 003-3V8a3 3 0 00-3-3H6a3 3 0 00-3 3v8a3 3 0 003 3z"
            />
          </svg>
          <div class="mb-4 p-4">
            <h3 class="mb-2 text-3xl font-semibold">Low Commission</h3>
            <p>
              We offer competitive sommission structure that are straightforward
              and fair, making it simple and affordable.
            </p>
          </div>
        </div>
      </div>
    </section>
    <section class="my-20">
      <div class="mb-8 text-center">
        <h2 class="mb-4 text-5xl font-semibold leading-[60px]">
          Our best blog
        </h2>
      </div>
      <div class="flex items-center space-x-8">
        <div class="w-1/2">
          <div class="flex flex-col space-y-12">
            <NuxtLink to="/" class="flex space-x-4">
              <img
                src="~/assets/images/home02.jpg"
                alt=""
                class="h-40 w-40 rounded-2xl"
              />
              <div>
                <h4 class="mb-4 text-2xl font-semibold">
                  This best kept secret helps new real estate agents find client
                </h4>
                <p class="mb-2">
                  Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                  Nostrum impedit distinctio rerum sunt, praesentium nemo?
                </p>
                <p class="text-rose-500">April 28, 2022</p>
              </div>
            </NuxtLink>
            <NuxtLink to="/" class="flex space-x-4">
              <img
                src="~/assets/images/home02.jpg"
                alt=""
                class="h-40 w-40 rounded-2xl"
              />
              <div>
                <h4 class="mb-4 text-2xl font-semibold">
                  This best kept secret helps new real estate agents find client
                </h4>
                <p class="mb-2">
                  Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                  Nostrum impedit distinctio rerum sunt, praesentium nemo?
                </p>
                <p class="text-rose-500">April 28, 2022</p>
              </div>
            </NuxtLink>
            <NuxtLink to="/" class="flex space-x-4">
              <img
                src="~/assets/images/home02.jpg"
                alt=""
                class="h-40 w-40 rounded-2xl"
              />
              <div>
                <h4 class="mb-4 text-2xl font-semibold">
                  This best kept secret helps new real estate agents find client
                </h4>
                <p class="mb-2">
                  Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                  Nostrum impedit distinctio rerum sunt, praesentium nemo?
                </p>
                <p class="text-rose-500">April 28, 2022</p>
              </div>
            </NuxtLink>
          </div>
        </div>
        <div class="w-1/2">
          <img src="~/assets/images/home01.jpg" alt="" class="rounded-2xl" />
        </div>
      </div>
    </section>
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
