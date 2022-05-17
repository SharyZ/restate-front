<template>
  <section class="my-20">
    <SectionHeading
      title="Special Homes"
      subtitle="Find your place with an immersive photo experience and the most listings, including things you won't find anywhere else."
    />
    <div class="grid grid-cols-3 gap-10">
      <HomeCard
        :price="4600000"
        address="Alatau, #99"
        city="Nukus"
        saleType="For sale"
      />
      <HomeCard
        :price="200000"
        address="Alatau, #99"
        city="Tashkent"
        saleType="For rent"
      />
      <HomeCard
        :price="4600000"
        address="Alatau, #99"
        city="Nukus"
        saleType="For sale"
      />
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped></style>
