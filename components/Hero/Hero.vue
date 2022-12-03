<script setup lang="ts">
import Layout from '../Layout/Layout.vue';
import Button from '../Button/Button.vue';
</script>

<template>
  <section class="pt-16 overflow-hidden relative mx-auto">
    <Layout
      class="flex flex-col lg:flex-row justify-between relative bg-[url('../../assets/images/bg-intro-mobile.svg')] bg-cover bg-center"
    >
      <div class="lg:max-w-[25rem] mt-80 md:mt-96 mb-20 lg:my-36 block">
        <h1
          class="text-primary-dark-blue font-medium text-4xl lg:text-5xl text-center lg:text-start"
        >
          Next generation digital banking
        </h1>
        <p
          class="text-center lg:text-start text-neutral-grayish-blue mt-5 text-base"
        >
          Take yout financial life online. Your Easybank account will be a
          one-stop-shop for spending, saving, budgeting, investing, and much
          more
        </p>
        <div class="flex justify-center lg:justify-start">
          <Button text="Request invite" class="mt-9" />
        </div>
      </div>
    </Layout>
    <div class="">
      <img
        class="z-[1] w-[20rem] md:w-[27rem] left-1/2 -translate-x-1/2 -top-20 absolute lg:left-auto lg:w-auto lg:max-w-fit lg:-translate-x-0 lg:-top-[10rem] lg:-right-[13rem] xl:-right-[5rem]"
        src="../../assets/images/image-mockups.png"
        alt="mockups"
      />
      <!-- <img
        class="z-[1] absolute lg:-top-[10rem] lg:-right-[13rem] xl:-right-[5rem]"
        src="../../assets/images/image-mockups.png"
        alt="mockups"
      /> -->
      <img
        class="lg:hidden absolute w-full h-[20rem] md:h-[26rem] top-[64px] left-0 right-0"
        src="../../assets/images/bg-intro-mobile.svg"
        alt="hero image"
      />
      <img
        class="hidden lg:block absolute lg:-top-[15rem] lg:-right-[25rem] xl:-right-[25rem]"
        src="../../assets/images/bg-intro-desktop.svg"
        alt="hero image"
      />
    </div>
  </section>
</template>
