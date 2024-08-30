<script setup lang="ts">
interface ILink {
  label: string
  href: string
}

interface IMenu {
  title: string
  links: ILink[]
}

const menus: IMenu[] = [
  {
    title: 'More on The Blog',
    links: [
      {
        label: 'About MNTN',
        href: '/'
      },
      {
        label: 'Contributors & Writers',
        href: '/'
      },
      {
        label: 'Write For Us',
        href: '/'
      },
      {
        label: 'Contact us',
        href: '/'
      },
      {
        label: 'Privacy Policy',
        href: '/'
      }
    ]
  },
  {
    title: 'More on MNTN',
    links: [
      { label: 'The Team', href: '/' },
      { label: 'Jobs', href: '/' },
      { label: 'Press', href: '/' }
    ]
  }
]
</script>

<template>
  <div class="w-full h-full">
    <header class="w-full flex justify-between items-center px-4 py-5 z-50 family-zilla">
      <div>
        <img src="./assets/logo.svg" alt="" srcset="" />
      </div>
      <nav class="hidden sm:block">
        <ul class="flex text-lg text-white gap-6 font-semibold">
          <li class="cursor-pointer transition p-2 hover:text-[#FBD784] hover:-translate-y-1">
            Equipment
          </li>
          <li class="cursor-pointer transition p-2 hover:text-[#FBD784] hover:-translate-y-1">
            About us
          </li>
          <li class="cursor-pointer transition p-2 hover:text-[#FBD784] hover:-translate-y-1">
            Blog
          </li>
        </ul>
      </nav>
      <div>
        <a
          href="https://github.com/Miguel-Domingos/MNTN"
          class="cursor-pointer text-lg font-bold opacity-50 hover:opacity-100 text-gray-950 transition"
        >
          <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24">
            <path
              fill="currentColor"
              d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5c.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34c-.46-1.16-1.11-1.47-1.11-1.47c-.91-.62.07-.6.07-.6c1 .07 1.53 1.03 1.53 1.03c.87 1.52 2.34 1.07 2.91.83c.09-.65.35-1.09.63-1.34c-2.22-.25-4.55-1.11-4.55-4.92c0-1.11.38-2 1.03-2.71c-.1-.25-.45-1.29.1-2.64c0 0 .84-.27 2.75 1.02c.79-.22 1.65-.33 2.5-.33s1.71.11 2.5.33c1.91-1.29 2.75-1.02 2.75-1.02c.55 1.35.2 2.39.1 2.64c.65.71 1.03 1.6 1.03 2.71c0 3.82-2.34 4.66-4.57 4.91c.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2"
            />
          </svg>
        </a>
      </div>
    </header>
    <div class="relative w-full h-full">
      <img
        class="w-full h-full absolute object-cover -top-[20%] -z-10 custom-animation"
        src="./assets/HG.png"
        alt=""
        srcset=""
      />
      <img
        class="w-full h-full absolute object-cover -top-[20%] -z-10"
        src="./assets/BG%20Hero.png"
        alt=""
        srcset=""
      />
      <img
        class="w-full h-full object-top object-cover absolute top-[30%] -z-10 custom-animation-2"
        src="./assets/MG.png"
        alt=""
        srcset=""
      />
      <div class="fixed -top-[10%] -z-10 w-full h-full">
        <div class="w-full h-full flex justify-center items-center custom-animation-3">
          <div class="flex flex-col justify-center start gap-7">
            <div
              class="text-[#FBD784] flex gap-4 items-center w-full justify-center md:justify-start"
            >
              <div class="bg-[#FBD784] h-0.5 w-14 md:block hidden"></div>
              <span class="text-lg font-semibold uppercase">A Hiking guide</span>
            </div>

            <h1
              class="flex text-center md:text-left text-4xl md:text-5xl lg:text-7xl font-light text-white flex-col family-zilla"
            >
              <span> Be prepared for the </span>
              <span> Mountains and beyond! </span>
            </h1>

            <div class="text-white flex justify-center md:justify-start gap-2 text-lg font-bold">
              <span>scroll down </span>
              <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 20 20">
                <path
                  fill="currentColor"
                  fill-rule="evenodd"
                  d="M10 2a.75.75 0 0 1 .75.75v12.59l1.95-2.1a.75.75 0 1 1 1.1 1.02l-3.25 3.5a.75.75 0 0 1-1.1 0l-3.25-3.5a.75.75 0 1 1 1.1-1.02l1.95 2.1V2.75A.75.75 0 0 1 10 2"
                  clip-rule="evenodd"
                />
              </svg>
            </div>
          </div>
        </div>
      </div>

      <img
        class="w-full h-full custom-position sm:object-left-top object-cover absolute top-[50%] sm:left-0 -z-10"
        src="./assets/VG.png"
        alt=""
        srcset=""
      />
      <div
        class="w-full h-full absolute top-[60%] -z-10 bg-[linear-gradient(180deg,_rgba(11,_29,_38,_0)_0%,_#0B1D26_61.38%)] aspect-video"
      ></div>
    </div>

    <main class="w-full bg-[#0b1d26] flex flex-col px-4 relative z-50 gap-48 lg:gap-64 my-40">
      <div
        class="flex flex-col-reverse items-center lg:items-start justify-between lg:gap-20 lg:flex-row mx-10 lg:mx-20"
      >
        <div class="relative w-full max-w-xl mt-32 flex flex-col gap-7 items-center md:items-start">
          <div class="absolute md:-top-[10%] md:-left-[15%] -top-[15%] left-0">
            <span class="text-white text-9xl font-bold opacity-10">01</span>
          </div>
          <div class="text-[#FBD784] flex gap-4 justify-center md:justify-start items-center">
            <div class="bg-[#FBD784] h-0.5 w-14 md:block hidden"></div>
            <span class="text-lg font-semibold uppercase">Get Started</span>
          </div>
          <h2
            class="font-semibold text-white md:text-left text-center text-3xl md:text-4xl lg:text-6xl"
          >
            What level of hiker are you?
          </h2>

          <span class="text-white text-lg text-center md:text-left">
            Determining what level of hiker you are can be an important tool when planning future
            hikes. This hiking level guide will help you plan hikes according to different hike
            ratings set by various websites like All Trails and Modern Hiker. What type of hiker are
            you – novice, moderate, advanced moderate, expert, or expert backpacker?
          </span>

          <div class="flex gap-2 font-semibold text-lg text-[#FBD784] cursor-pointer">
            <span class="">read more</span>

            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 20 20">
              <path
                fill="currentColor"
                fill-rule="evenodd"
                d="M2 10a.75.75 0 0 1 .75-.75h12.59l-2.1-1.95a.75.75 0 1 1 1.02-1.1l3.5 3.25a.75.75 0 0 1 0 1.1l-3.5 3.25a.75.75 0 1 1-1.02-1.1l2.1-1.95H2.75A.75.75 0 0 1 2 10"
                clip-rule="evenodd"
              />
            </svg>
          </div>
        </div>
        <div class="w-full max-w-lg">
          <img class="w-full object-cover" src="./assets/01.png" alt="" srcset="" />
        </div>
      </div>

      <div
        class="flex flex-col-reverse items-center lg:items-start justify-between lg:gap-20 lg:flex-row-reverse mx-10"
      >
        <div class="relative w-full max-w-xl mt-32 flex flex-col gap-7 items-center md:items-start">
          <div class="absolute md:-top-[10%] md:-left-[15%] left-0 -top-[15%]">
            <span class="text-white text-9xl font-bold opacity-10">02</span>
          </div>
          <div class="text-[#FBD784] flex gap-4 justify-center md:justify-start items-center">
            <div class="bg-[#FBD784] h-0.5 w-14 md:block hidden"></div>
            <span class="text-lg font-semibold uppercase">Hiking </span>
          </div>
          <h2
            class="font-semibold md:text-left text-center text-3xl md:text-4xl lg:text-6xl text-white"
          >
            Picking the right Hiking Gear!
          </h2>

          <span class="text-white text-lg text-center md:text-left">
            The nice thing about beginning hiking is that you don’t really need any special gear,
            you can probably get away with things you already have. Let’s start with clothing. A
            typical mistake hiking beginners make is wearing jeans and regular clothes, which will
            get heavy and chafe wif they get sweaty or wet.</span
          >

          <div class="flex gap-2 font-semibold text-lg text-[#FBD784] cursor-pointer">
            <span class="">read more</span>

            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 20 20">
              <path
                fill="currentColor"
                fill-rule="evenodd"
                d="M2 10a.75.75 0 0 1 .75-.75h12.59l-2.1-1.95a.75.75 0 1 1 1.02-1.1l3.5 3.25a.75.75 0 0 1 0 1.1l-3.5 3.25a.75.75 0 1 1-1.02-1.1l2.1-1.95H2.75A.75.75 0 0 1 2 10"
                clip-rule="evenodd"
              />
            </svg>
          </div>
        </div>
        <div class="w-full max-w-lg">
          <img class="w-full object-cover" src="./assets/02.png" alt="" srcset="" />
        </div>
      </div>

      <div
        class="flex flex-col-reverse items-center lg:items-start justify-between lg:gap-20 lg:flex-row mx-10 lg:mx-20"
      >
        <div class="relative w-full max-w-xl mt-32 flex flex-col gap-7 items-center md:items-start">
          <div class="absolute md:-top-[10%] md:-left-[15%] left-0 -top-[15%]">
            <span class="text-white text-9xl font-bold opacity-10">03</span>
          </div>
          <div class="text-[#FBD784] flex gap-4 justify-center md:justify-start items-center">
            <div class="bg-[#FBD784] h-0.5 w-14 md:block hidden"></div>
            <span class="text-lg font-semibold uppercase">where you go is the key</span>
          </div>
          <h2
            class="md:text-left text-center font-semibold text-3xl md:text-4xl lg:text-6xl text-white"
          >
            Understand Your Map & Timing
          </h2>

          <span class="text-white text-lg text-center md:text-left">
            To start, print out the hiking guide and map. If it’s raining, throw them in a Zip-Lock
            bag. Read over the guide, study the map, and have a good idea of what to expect. I like
            to know what my next landmark is as I hike. For example, I’ll read the guide and know
            that say, in a mile, I make a right turn at the junction..</span
          >

          <div class="flex gap-2 font-semibold text-lg text-[#FBD784] cursor-pointer">
            <span class="">read more</span>

            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 20 20">
              <path
                fill="currentColor"
                fill-rule="evenodd"
                d="M2 10a.75.75 0 0 1 .75-.75h12.59l-2.1-1.95a.75.75 0 1 1 1.02-1.1l3.5 3.25a.75.75 0 0 1 0 1.1l-3.5 3.25a.75.75 0 1 1-1.02-1.1l2.1-1.95H2.75A.75.75 0 0 1 2 10"
                clip-rule="evenodd"
              />
            </svg>
          </div>
        </div>
        <div class="w-full max-w-lg">
          <img class="w-full object-cover" src="./assets/03.png" alt="" srcset="" />
        </div>
      </div>
    </main>
    <footer class="w-full bg-[#0b1d26]">
      <div class="w-full bg-[#0b1d26] container mx-auto px-4 pb-32">
        <div
          class="w-full flex justify-between md:flex-row flex-col gap-16 items-center text-center md:text-left md:items-start"
        >
          <div class="flex h-full flex-col justify-between md:gap-8">
            <div class="flex flex-col gap-6 items-center md:items-start">
              <img src="./assets/logo.svg" alt="" srcset="" />
              <span class="text-white font-bold"
                >Get out there & discover your next <br />
                slope, mountain & destination!</span
              >
            </div>
            <div>
              <span class="text-white hidden md:block text-sm font-light opacity-50">
                Copyright 2023 MNTN, Inc. Terms & Privacy
              </span>
            </div>
          </div>

          <div
            class="flex gap-16 lg:gap-28 md:flex-row flex-col items-center text-center md:text-left md:items-start"
          >
            <div v-for="menu in menus" :key="menu.title" class="flex flex-col gap-6">
              <span class="text-[#FBD784] text-lg font-bold">{{ menu.title }}</span>

              <div class="flex flex-col gap-4">
                <span v-for="link in menu.links" :key="link.label" class="text-white">{{
                  link.label
                }}</span>
              </div>
            </div>
          </div>

          <span class="text-white block md:hidden text-sm text-center font-light opacity-50">
            Copyright 2023 MNTN, Inc. Terms & Privacy
          </span>
        </div>
      </div>
    </footer>
  </div>
</template>

<style>
.custom-animation {
  animation-name: customAnimation;
  animation-duration: 1ms; /* Firefox requires this to apply the animation */
  animation-timeline: --customTimeline;
}

@keyframes customAnimation {
  20% {
    top: -50%;
  }

  100% {
    top: -80%;
  }
}

.custom-animation-2 {
  animation-name: customAnimation2;
  animation-duration: 1ms; /* Firefox requires this to apply the animation */
  animation-timeline: --customTimeline;
}

@keyframes customAnimation2 {
  15% {
    top: 20%;
  }
  100% {
    top: 25%;
  }
}

.custom-animation-3 {
  animation-name: customAnimation3;
  animation-duration: 1ms; /* Firefox requires this to apply the animation */
  animation-timeline: --customTimeline;
}

@keyframes customAnimation3 {
  0% {
    opacity: 1;
  }

  20% {
    opacity: 0;
    color: #0b1d26;
  }

  100% {
    opacity: 0;
    color: #0b1d26;
  }
}

.custom-position {
  object-position: 20% 0;
}
</style>
