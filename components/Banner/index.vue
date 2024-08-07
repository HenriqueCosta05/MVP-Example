<template>
  <div class="bg-[url('/assets/images/banner.jpg')] bg-fixed min-w-full w-[calc('100vw' -'1vw')] min-h-screen h-screen bg-no-repeat drop-shadow-md ">
    <div class="flex flex-col justify-center items-center h-full">
      <BannerHeading text="Welcome to our website" highlighted-text="BooleanTech"></BannerHeading>
      <BannerDescription text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."></BannerDescription>
      <div class="flex gap-4">
        <Button text="Get Started" :icon="RocketIcon"/>
        <ButtonOutlined :icon="InfoIcon" text="Learn More" />
      </div>
  </div>
  </div>
</template>

<script lang="ts" setup>
import RocketIcon from '~/assets/icons/rocket.svg'
import InfoIcon from '~/assets/icons/info.svg'
</script>

