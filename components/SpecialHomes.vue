<template>
  <section class="my-20">
    <SectionHeading
      title="Special Homes"
      subtitle="Find your place with an immersive photo experience and the most listings, including things you won't find anywhere else."
    />
    <p v-if="$fetchState.pending">Fetching houses...</p>
    <p v-else-if="$fetchState.error">An error occurred :(</p>
    <div v-else class="grid grid-cols-3 gap-10">
      <HomeCard
        v-for="house in houses"
        :key="house.id"
        :price="house.price"
        :address="house.address"
        :city="house.city"
        :saleType="house.sale_type"
      />
    </div>
  </section>
</template>

<script>
export default {
  name: 'SpecialHomes',
  data: () => ({
    houses: [],
  }),
  async fetch() {
    this.houses = await this.$axios.$get(`listings/`)
  },
}
</script>

<style scoped></style>
