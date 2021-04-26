<template>
  <section class="hero is-white is-fullheight">
    <div class="hero-body">
      <div class="inner-container">
        <div class="columns is-vcentered" style="width: 100%;">

          <div data-aos="fade-down" class="column
          is-10-mobile is-offset-1-mobile
          is-10-tablet is-offset-1-tablet
          is-5-desktop is-offset-1-desktop
          is-5-widescreen is-offset-1-widescreen
          is-5-fullhd is-offset-1-fullhd has-text-right">
            <h1 class="title is-2 mb-6 rtl">
              {{ title }}
            </h1>
            <h2 class="subtitle is-5">
              {{ description }}
            </h2>
          </div>

          <div data-aos="fade-left" class="column
          is-10-mobile is-offset-1-mobile
          is-10-tablet is-offset-1-tablet
          is-4-desktop is-offset-1-desktop
          is-4-widescreen is-offset-1-widescreen
          is-4-fullhd is-offset-1-fullhd">
            <figure class="image is-square">
              <img :src="imageSrc">
            </figure>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  props: {
    title: {
      required: true,
      type: String
    },
    description: {
      required: true,
      type: String
    },
    imageSrc: {
      required: true,
      type: String
    }
  }
}
</script>