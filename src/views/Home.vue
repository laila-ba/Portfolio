<template>
  <body>
    <div class="relative isolate">
      <div class="px-6 pt-6 lg:px-8">
        <nav
          class="flex items-center justify-between mx-96 py-4 px-12"
          aria-label="Global"
        >
          <div class="flex lg:flex-1">
            <a href="#" class="-m-1.5 p-1.5">
              <span class="sr-only">Laila B</span>
              <img class="w-32" src="../assets/img/laays2.png" alt="" />
            </a>
          </div>
          <div class="flex lg:hidden">
            <button
              type="button"
              class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-white"
              @click="mobileMenuOpen = true"
            >
              <span class="sr-only">Open main menu</span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                />
              </svg>
            </button>
          </div>
          <div class="hidden lg:flex lg:gap-x-12">
            <a
              v-for="item in navigation"
              :key="item.name"
              :href="item.href"
              class="text-sm font-semibold text-white"
              >{{ item.name }}</a
            >
          </div>
        </nav>

        <Dialog as="div" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
          <DialogPanel
            focus="true"
            class="fixed inset-0 z-10 overflow-y-auto bg-white px-6 py-6 lg:hidden"
          >
            <div class="flex items-center justify-between">
              <a href="#" class="-m-1.5 p-1.5">
                <span class="sr-only">Your Company</span>
                <img class="w-40" src="../assets/img/logo.png" alt="" />
              </a>
              <button
                type="button"
                class="-m-2.5 rounded-md p-2.5 text-gray-700"
                @click="mobileMenuOpen = false"
              >
                <span class="sr-only">Close menu</span>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M6 18L18 6M6 6l12 12"
                  />
                </svg>
              </button>
            </div>
            <div class="mt-6 flow-root">
              <div class="-my-6 divide-y divide-gray-500/10">
                <div class="space-y-2 py-6">
                  <a
                    v-for="item in navigation"
                    :key="item.name"
                    :href="item.href"
                    class="-mx-3 block rounded-lg py-2 px-3 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-400/10"
                    >{{ item.name }}</a
                  >
                </div>
                <div class="py-6">
                  <a
                    href="#"
                    class="-mx-3 block rounded-lg py-2.5 px-3 text-base font-semibold leading-6 text-gray-900 hover:bg-gray-400/10"
                    >Log in</a
                  >
                </div>
              </div>
            </div>
          </DialogPanel>
        </Dialog>
      </div>
      <div class="flex">
        <img
          class="absolute z-0 image-height"
          src="../assets/img/shapes.png"
          alt=""
        />
      </div>
      <div
        class="mx-auto pr-6 lg:flex lg:items-center xl:ml-72 pl-12 text-left z-10 relative"
      >
        <div class="mx-auto max-w-2xl lg:mx-0 lg:flex-auto">
          <h1
            class="mt-24 max-w-lg text-4xl font-bold tracking-tight text-white sm:text-8xl"
          >
            Frontend <br />
            <span
              class="animate-text bg-gradient-to-r from-pink-500 via-purple-500 to-blue-500 bg-clip-text text-transparent text-8xl font-black"
              >Developer</span
            >
          </h1>

          <p class="mt-6 text-lg leading-8 text-white">
            Motivated young developer with a drive to combine creative design
            with the power of code.
          </p>
          <!-- <div class="mt-10 flex items-center gap-x-6">
            <a
              href="#about"
              class="animate-bounce rounded-md bg-indigo-600 px-3.5 py-1.5 text-lg text-white shadow-sm"
              >Tell me more</a
            >
          </div> -->
        </div>
        <div class="mt-16 sm:mt-24">
          <img
            class="mx-auto w-3/4 drop-shadow-xl rounded-full"
            src="../assets/img/laila3.png"
            alt=""
          />
        </div>
      </div>

      <div class="cursor-pointer">
        <a href="#about">
          <lottie-player
            class="mx-auto -mt-12 cursor-pointer"
            src="https://lottie.host/12d490c7-9b30-4ba9-af21-c10be56bd8b3/0wyQQs7Tli.json"
            background="transparent"
            speed="1"
            style="width: 90px; height: 90px"
            loop
            autoplay
          ></lottie-player>
        </a>
      </div>

      <About></About>
      <Projects></Projects>
    </div>
  </body>
</template>
<style>
.image-height {
  height: 50rem;
}
</style>
<script setup>
import { ref } from "vue";
import { Dialog, DialogPanel } from "@headlessui/vue";
import About from "../components/About.vue";
import Projects from "../components/Projects.vue";

const navigation = [
  { name: "h o m e", href: "#home" },
  { name: "a b o u t", href: "#about" },
  { name: "p r o j e c t s", href: "#" },
  { name: "c o n t a c t", href: "#" },
];

const mobileMenuOpen = ref(false);
</script>
