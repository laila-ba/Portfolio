<template>
  <body>
    <!--practice-->
    <div class="container1">
      <div class="px-6 pt-6 lg:px-8 absolute top-0">
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
      <!--nav end-->
      <!--main hero start-->

      <div
        class="mx-auto pr-6 lg:flex lg:items-center xl:ml-72 pl-12 text-left z-10 relative"
      >
        <div class="mx-auto max-w-2xl lg:mx-0 lg:flex-auto">
          <h1
            class="mt-24 max-w-lg text-4xl font-bold tracking-tight text-white sm:text-8xl"
          >
            Frontend <br />
            <span
              class="animate-text bg-gradient-to-r from-yellow-500 to-purple-500 bg-clip-text text-transparent text-8xl font-black"
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
        <div
          class="absolute -left-80 -top-56 transform-gpu blur-3xl"
          aria-hidden="true"
        >
          <div
            class="aspect-[1097/845] w-[68.5625rem] bg-gradient-to-r from-[#ff4694] to-[#776fff] opacity-[0.45]"
            style="
              clip-path: polygon(
                74.1% 44.1%,
                100% 61.6%,
                97.5% 26.9%,
                85.5% 0.1%,
                80.7% 2%,
                72.5% 32.5%,
                60.2% 62.4%,
                52.4% 68.1%,
                47.5% 58.3%,
                45.2% 34.5%,
                27.5% 76.7%,
                0.1% 64.9%,
                17.9% 100%,
                27.6% 76.8%,
                76.1% 97.7%,
                74.1% 44.1%
              );
            "
          ></div>
        </div>
        <div
          class="hidden md:absolute md:bottom-16 md:left-[50rem] md:block md:transform-gpu md:blur-3xl"
          aria-hidden="true"
        >
          <div
            class="aspect-[1097/845] w-[68.5625rem] bg-gradient-to-r from-[#ff4694] to-[#776fff] opacity-25"
            style="
              clip-path: polygon(
                74.1% 44.1%,
                100% 61.6%,
                97.5% 26.9%,
                85.5% 0.1%,
                80.7% 2%,
                72.5% 32.5%,
                60.2% 62.4%,
                52.4% 68.1%,
                47.5% 58.3%,
                45.2% 34.5%,
                27.5% 76.7%,
                0.1% 64.9%,
                17.9% 100%,
                27.6% 76.8%,
                76.1% 97.7%,
                74.1% 44.1%
              );
            "
          ></div>
        </div>
        <div class="mt-16 sm:mt-24">
          <img
            class="mx-auto w-3/4 drop-shadow-xl rounded-full"
            src="../assets/img/laila3.png"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="blank">
      <About></About>
    </div>
    <div class="container1 second">
      <div class="item">
        <div class="img img-first"></div>
        <div class="card">
          <h3>Rock climbing</h3>
          <p>
            The goal is to reach the summit of a formation or the endpoint of a
            usually pre-defined route without falling
          </p>
          <a href="#">Learn more</a>
        </div>
      </div>
      <div class="item">
        <div class="img img-second"></div>
        <div class="card">
          <h3>Caving</h3>
          <p>
            Exploring underground through networks of tunnels and passageways,
            which can be natural or artificial.
          </p>
          <a href="#">Learn more</a>
        </div>
      </div>
      <div class="item">
        <div class="img img-third"></div>
        <div class="card">
          <h3>Parachuting</h3>
          <p>
            Jumping from an aeroplane and falling through the air before opening
            your parachute.
          </p>
          <a href="#">Learn more</a>
        </div>
      </div>
    </div>

    <div class="blank"></div>
    <div class="">
      <svg
        class="absolute w-full bg-cover"
        xmlns="http://www.w3.org/2000/svg"
        version="1.1"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        xmlns:svgjs="http://svgjs.dev/svgjs"
        viewBox="0 0 800 800"
      >
        <defs>
          <filter
            id="bbblurry-filter"
            x="-100%"
            y="-100%"
            width="400%"
            height="400%"
            filterUnits="objectBoundingBox"
            primitiveUnits="userSpaceOnUse"
            color-interpolation-filters="sRGB"
          >
            <feGaussianBlur
              stdDeviation="130"
              x="0%"
              y="0%"
              width="100%"
              height="100%"
              in="SourceGraphic"
              edgeMode="none"
              result="blur"
            ></feGaussianBlur>
          </filter>
        </defs>
        <g filter="url(#bbblurry-filter)">
          <ellipse
            rx="150"
            ry="150"
            cx="185.69611654231676"
            cy="614.0045897798389"
            fill="hsl(37, 99%, 67%)"
          ></ellipse>
          <ellipse
            rx="150"
            ry="150"
            cx="864.0801801431866"
            cy="-87.974101121513"
            fill="hsl(38, 99%, 67%)"
          ></ellipse>
        </g>
      </svg>
    </div>

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
          Motivated young developer with a drive to combine creative design with
          the power of code.
        </p>
        <!-- <div class="mt-10 flex items-center gap-x-6">
            <a
              href="#about"
              class="animate-bounce rounded-md bg-indigo-600 px-3.5 py-1.5 text-lg text-white shadow-sm"
              >Tell me more</a
            >
          </div> -->
      </div>
      <div
        class="absolute -left-80 -top-56 transform-gpu blur-3xl"
        aria-hidden="true"
      >
        <div
          class="aspect-[1097/845] w-[68.5625rem] bg-gradient-to-r from-[#ff4694] to-[#776fff] opacity-[0.45]"
          style="
            clip-path: polygon(
              74.1% 44.1%,
              100% 61.6%,
              97.5% 26.9%,
              85.5% 0.1%,
              80.7% 2%,
              72.5% 32.5%,
              60.2% 62.4%,
              52.4% 68.1%,
              47.5% 58.3%,
              45.2% 34.5%,
              27.5% 76.7%,
              0.1% 64.9%,
              17.9% 100%,
              27.6% 76.8%,
              76.1% 97.7%,
              74.1% 44.1%
            );
          "
        ></div>
      </div>
      <div
        class="hidden md:absolute md:bottom-16 md:left-[50rem] md:block md:transform-gpu md:blur-3xl"
        aria-hidden="true"
      >
        <div
          class="aspect-[1097/845] w-[68.5625rem] bg-gradient-to-r from-[#ff4694] to-[#776fff] opacity-25"
          style="
            clip-path: polygon(
              74.1% 44.1%,
              100% 61.6%,
              97.5% 26.9%,
              85.5% 0.1%,
              80.7% 2%,
              72.5% 32.5%,
              60.2% 62.4%,
              52.4% 68.1%,
              47.5% 58.3%,
              45.2% 34.5%,
              27.5% 76.7%,
              0.1% 64.9%,
              17.9% 100%,
              27.6% 76.8%,
              76.1% 97.7%,
              74.1% 44.1%
            );
          "
        ></div>
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
  </body>
</template>
<style>
.image-height {
  height: 50rem;
}
.container1 {
  text-align: center;
  color: var(--color);
  width: 100%;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-image: url(../assets/img/hero-background2.png);
  background-size: cover;
  background-position: center;

  /*  this is where the magic happens:  */
  background-attachment: fixed;
}

h1 {
  font-weight: 700;
  font-size: 3rem;
}

p {
  max-width: 52ch;
  line-height: 1.5;
  padding: 1em;
}

a {
  display: inline-block;
  padding: 1em 3.5em;
  background-color: var(--color);
  color: white;
  text-decoration: none;
  text-transform: uppercase;
  border-radius: 0.3em;
  font-weight: 700;
  letter-spacing: 0.5px;
  font-size: 0.875rem;
}

.blank,
.other {
  width: 100%;
  min-height: 80vh;
  background-color: #fff;
}

.second {
  background-image: url(https://images.unsplash.com/photo-1514496959998-c01c40915c5f?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1740&q=80);
  background-attachment: fixed;
  height: 1200px;
}

h3 {
  font-weight: 700;
  font-size: 1.6rem;
  margin-top: 1em;
}

.card > a {
  margin-bottom: 2em;
}

.item {
  display: flex;
  max-width: 320px;
  background-color: white;
  flex-direction: column;
  align-items: center;
  border-radius: 0.5em;
  -webkit-box-shadow: 0px 29px 38px -15px rgba(0, 0, 0, 0.43);
  -moz-box-shadow: 0px 29px 38px -15px rgba(0, 0, 0, 0.43);
  box-shadow: 0px 29px 38px -15px rgba(0, 0, 0, 0.43);
}

.img {
  width: 90%;
  height: 200px;
  background-color: lightgrey;
  background-size: cover;
  background-position: center;
  margin-top: 20px;
  border-radius: 0.3em;
}

.img-first {
  background-image: url(https://images.unsplash.com/photo-1522163182402-834f871fd851?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1606&q=80);
}

.img-second {
  background-image: url(https://images.unsplash.com/photo-1628746404106-4d3843b231b3?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NHx8Y2F2aW5nfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=900&q=60);
}

.img-third {
  background-image: url(https://images.unsplash.com/photo-1632853073412-782bf0279d65?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80);
}

.second {
  flex-direction: row;
  gap: 1.6em;
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
