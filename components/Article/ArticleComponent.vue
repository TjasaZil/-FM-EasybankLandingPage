<template>
  <div class="w-full mx-auto flex flex-col justify-center content-center mt-32">
    <div
      class="w-10/12 mx-auto text flex flex-col justify-center content-center text-center max-w-6xl lg:text-left"
    >
      <h2
        class="capitalize text-3xl lg:mx-0 lg:text-4xl text-primary-dark-blue font-normal"
      >
        latest articles
      </h2>
      <div
        class="flex flex-col justify-center items-center lg:flex-row lg:justify-between lg:mx-0 mx-auto"
      >
        <div
          v-for="text in texts"
          :key="text"
          class="flex flex-col justify-center items-start text-left mx-auto lg:w-1/5 lg:mx-0 max-w-[327px] lg:max-w-[255px] space-y-4 lg:space-y-0 mt-16 max-h-[395px]"
        >
          <img
            class="rounded-md lg:w-[255px]"
            :src="text.img"
            :alt="text.alt"
          />
          <div
            class="flex flex-col justify-center items-start text-left mx-auto max-w-[255px] lg:w-[207px] space-y-2"
          >
            <p class="capitalize text-neutral-grayish-blue text-xs mt-5">
              by {{ text.writer }}
            </p>
            <h3
              class="text-base font-medium text-primary-dark-blue hover:text-primary-bright-cyan hover:cursor-pointer lg:text-lg"
            >
              {{ text.heading }}
            </h3>
            <p
              class="text-neutral-grayish-blue text-[12px] lg:text-[12.5px] leading-snug"
            >
              {{ text.paragraph }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import Currency from '@/assets/images/image-currency-1.jpg';
import Restaurant from '@/assets/images/image-restaurant.jpg';
import Plane from '@/assets/images/image-plane.jpg';
import Confetti from '@/assets/images/image-confetti.jpg';

const texts = [
  {
    img: Currency,
    alt: 'Various paper currency',
    writer: 'Clare Robinson',
    heading: 'Recieve money in any currency with no fees',
    paragraph:
      'The world is getting smaller and we’re becoming more mobile. So why should you be forced to only receive money in a single …',
  },
  {
    img: Restaurant,
    alt: 'fine dining restaurant',
    writer: 'Wilson Hutton',
    heading: 'Treat yourself without worrying about money',
    paragraph:
      'Our simple budgeting feature allows you to separate out your spending and set realistic limits each month. That means you …',
  },
  {
    img: Plane,
    alt: 'a white wing of a plane',
    writer: 'Wilson Hutton',
    heading: 'take your Easybank card wherever you go',
    paragraph:
      'We want you to enjoy your travels. This is why we don’t charge any fees on purchases while you’re abroad. We’ll even show you …',
  },
  {
    img: Confetti,
    alt: 'colorfull confetti on a teal blue background',
    writer: 'Clare Robinson',
    heading: ' Our invite-only Beta accounts are now live',
    paragraph:
      'After a lot of hard work by the whole team, we’re excited to launch our closed beta. It’s easy to request an invite through the site ...',
  },
];
</script>
