<template>
  <div>
    <NavBar />
    <div class="">
      <div class="">
        <HeroComponent data-aos="fade-up" />
      </div>
      <ServicesComponent
        data-aos="zoom-in"
        data-aos-duration="3000"
        data-aos-easing="linear"
      />
      <TestimonialComponent data-aos="fade-in" />
      <FaqComponent data-aos="fade-out" />
      <ContactComponent data-aos="fade-down" data-aos-easing="linear" />
      <FooterComponent data-aos="zoom-in" />
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
