<script setup lang="ts">
import Layout from '../Layout/Layout.vue';
import Button from '../Button/Button.vue';
</script>

<template>
  <section class="pt-16 overflow-hidden relative">
    <Layout class="flex flex-col lg:flex-row justify-between relative">
      <div class="lg:max-w-[25rem] mt-72 mb-20 lg:my-36 block">
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
        class="z-[1] absolute lg:-top-[10rem] lg:-right-[13rem] xl:-right-[5rem]"
        src="../../assets/images/image-mockups.png"
        alt="mockups"
      />
      <img
        class="absolute lg:-top-[15rem] lg:-right-[25rem] xl:-right-[25rem]"
        src="../../assets/images/bg-intro-desktop.svg"
        alt="hero image"
      />
    </div>
  </section>
</template>
