<template>
  <section class="my-20">
    <SectionHeading title="Our best blog" />
    <div class="flex items-center space-x-8">
      <div class="w-1/2">
        <div class="flex flex-col space-y-12">
          <PostCard
            title="This best kept secret helps new real estate agents find client"
            subtitle="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum impedit distinctio rerum sunt, praesentium nemo?"
            date="April 28, 2022"
          />
          <PostCard
            title="This best kept secret helps new real estate agents find client"
            subtitle="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum impedit distinctio rerum sunt, praesentium nemo?"
            date="April 28, 2022"
          />
          <PostCard
            title="This best kept secret helps new real estate agents find client"
            subtitle="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum impedit distinctio rerum sunt, praesentium nemo?"
            date="April 28, 2022"
          />
        </div>
      </div>
      <div class="w-1/2">
        <img src="~/assets/images/home01.jpg" alt="" class="rounded-2xl" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BlogPosts',
}
</script>

<style scoped></style>
