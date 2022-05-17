<template>
  <section class="my-20">
    <SectionHeading
      title="Our Service"
      subtitle="When it comes to real estate and properties, we're very happy step of the way."
    />
    <div class="grid grid-cols-3 gap-14">
      <ServiceCard
        title="Property Insurance"
        subtitle="Property insurance provides protection against most risks to property, such as fire, theft."
      >
        <template #icon>
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
        </template>
      </ServiceCard>
      <ServiceCard
        title="Advantage"
        subtitle="All these properties have amazing prices, and you will find thousands of properties to choose from."
      >
        <template #icon>
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
        </template>
      </ServiceCard>
      <ServiceCard
        title="Low Commission"
        subtitle="We offer competitive sommission structure that are straightforward and fair, making it simple and affordable."
      >
        <template #icon>
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
        </template>
      </ServiceCard>
    </div>
  </section>
</template>

<script>
export default {
  name: 'OurService',
}
</script>

<style scoped></style>
