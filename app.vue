<template>
  <div>
    <NavBar />
    <div class="">
      <div class="">
        <HeroComponent
          data-aos="fade-in-right"
          data-aos-duration="2000"
          data-aos-easing="linear"
        />
      </div>
      <ServicesComponent
        data-aos="zoom-in"
        data-aos-duration="1000"
        data-aos-easing="linear"
      />
      <TestimonialComponent
        data-aos="zoom-in"
        data-aos-duration="1000"
        data-aos-easing="linear"
      />
      <FaqComponent data-aos="zoom-in" data-aos-duration="1000" />
      <ContactComponent
        data-aos="zoom-in"
        data-aos-easing="linear"
        data-aos-duration="1000"
      />
      <FooterComponent data-aos="zoom-in" data-aos-duration="1000" />
    </div>
  </div>
</template>
<script setup>
import "aos/dist/aos.css";
import AOS from "aos";
onMounted(() => {
  AOS.init();
});
</script>
