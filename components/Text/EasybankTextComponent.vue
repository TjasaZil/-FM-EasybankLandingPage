<template>
  <div class="w-full flex flex-col justify-center items-center mt-20 mx-auto">
    <div
      class="w-10/12 mx-auto text flex flex-col justify-center content-center text-center max-w-7xl"
    >
      <h2
        class="text-center capitalize text-3xl text-primary-dark-blue lg:text-left"
      >
        Why Choose Easybank?
      </h2>
      <p
        class="max-w-[635px] mx-auto lg:text-left lg:mx-0 text-neutral-grayish-blue text-base leading-5 mt-6 lg:text-[17px]"
      >
        We leverage Open Banking to turn your bank account into your financial
        hub. Control your finances like never before.
      </p>
      <div
        class="flex flex-col mx-auto text-center justify-center content-center lg:flex-row lg:text-left lg:justify-between lg:mx-0 max-w-7xl"
      >
        <div
          v-for="render in renders"
          :key="render"
          class="max-w-[255px] lg:w-1/5 xl:w-1/4 flex flex-col mx-auto text-center justify-center content-center space-y-5 lg:space-y-6 lg:mx-0 mt-8"
        >
          <img
            :src="render.img"
            alt="green circular icons"
            class="w-[72px] h-[72px] mx-auto lg:mx-0"
          />
          <h3 class="capitalize text-2xl text-primary-dark-blue lg:text-left">
            {{ render.heading }}
          </h3>
          <p
            class="text-neutral-grayish-blue text-base leading-5 lg:text-left lg:leading-6"
          >
            {{ render.text }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Budgeting from '@/assets/images/icon-budgeting.svg';
import Onboarding from '@/assets/images/icon-onboarding.svg';
import Banking from '@/assets/images/icon-online.svg';
import API from '@/assets/images/icon-api.svg';

export default {
  name: 'EasybankTextComponent',
  data() {
    return {
      renders: [
        {
          img: Banking,
          heading: 'online banking',
          text: 'Our modern web and mobile applications allow you to keep track of your finances wherever you are in the world.',
        },
        {
          img: Budgeting,
          heading: 'simple budgeting',
          text: 'See exactly where your money goes each month. Receive notifications when you’re close to hitting your limits.',
        },
        {
          img: Onboarding,
          heading: 'fast onboarding',
          text: 'We don’t do branches. Open your account in minutes online and start taking control of your finances right away.',
        },
        {
          img: API,
          heading: 'open API',
          text: 'Manage your savings, investments, pension, and much more from one account. Tracking your money has never been easier.',
        },
      ],
    };
  },
};
</script>
