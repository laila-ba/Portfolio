<template>
  <section id="about" class="about reveal">
    <div class="overflow-hidden py-24 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div
          class="mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 sm:gap-y-20 lg:mx-0 lg:max-w-none lg:grid-cols-2"
        >
          <div class="lg:ml-auto lg:pl-4 lg:pt-4">
            <div class="lg:max-w-lg">
              <div class="">
                <h2
                  class="text-6xl font-semibold leading-7 text-white text-center"
                >
                  About me
                </h2>
              </div>
              <p class="mt-12 text-lg leading-8 text-gray-600">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Maiores impedit perferendis suscipit eaque, iste dolor
                cupiditate blanditiis ratione.
              </p>
            </div>
          </div>
          <div class="flex items-start lg:order-first">
            <img
              src="../assets/img/laila-avatar.png"
              alt="about-img"
              class="rounded-full w-3/4"
              width="2432"
              height="1442"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- <section id="about" class="about reveal">
    <div class="about-card text-container">
      <div class="w-full max-w-xl xl:max-w-none xl:flex-auto xl:px-16 text-box">
        <img class="w-32" src="../assets/img//01-new.png" alt="" />

        <h2
          class="text-7xl bg-white animate-text bg-gradient-to-r from-pink-500 via-purple-500 to-blue-500 bg-clip-text text-transparent font-black pt-6 text-center"
        >
          Hi, I'm Laila.
        </h2>

        <figure class="relative isolate pt-12">
          <blockquote
            class="text-lg text-white sm:leading-9 text-left space-y-4"
          >
            <p>
              I am a 22yr old front-end web developer, who loves turning lines
              of code into visually captivating and seamlessly functional
              websites :)
            </p>
            <p>
              I am based in London and currently working as a junior developer
              for
              <a href="https://tedbree.com/"
                ><span
                  class="bg-white animate-text bg-gradient-to-r from-pink-500 via-purple-500 to-blue-500 bg-clip-text text-transparent font-bold"
                  >Tedbree</span
                ></a
              >
              .
            </p>
          </blockquote>
        </figure>
      </div>
    </div>
  </section>
  <section id="about" class="about reveal">
    <div class="about-card text-container">
      <div class="w-full max-w-xl xl:max-w-none xl:flex-auto xl:px-16 text-box">
        <img class="w-36" src="../assets/img//02.png" alt="" />
        <h2
          class="text-7xl bg-white animate-text bg-gradient-to-r from-pink-500 via-purple-500 to-blue-500 bg-clip-text text-transparent font-black pt-6 text-center"
        >
          I love design.
        </h2>

        <figure class="relative isolate pt-12">
          <blockquote
            class="text-lg text-white sm:leading-9 text-left space-y-4"
          >
            <p>
              Im super passionate about bringing ideas to life in the browser
              and making things simply look good. Ive always had a sharp eye for
              design and dont stop until i achieve my goals!
            </p>
            <p>
              I have been coding for around 4 years now and
              <span
                class="bg-white animate-text bg-gradient-to-r from-pink-500 via-purple-500 to-blue-500 bg-clip-text text-transparent font-bold"
                >LOVEEEE</span
              >
              what i do.
            </p>
            <p>Here's a run down of my experince</p>
            <div class="cursor-pointer">
              <a href="#projects">
                <lottie-player
                  class="mx-auto -mt-12 cursor-pointer"
                  src="https://lottie.host/12d490c7-9b30-4ba9-af21-c10be56bd8b3/0wyQQs7Tli.json"
                  background="transparent"
                  speed="1"
                  style="width: 50px; height: 50px"
                  loop
                  autoplay
                ></lottie-player>
              </a>
            </div>
          </blockquote>
        </figure>
      </div>
    </div>
  </section> -->
</template>
<style>
.project {
  grid-column: 2/14;
  padding: 6rem;

  &-box__wrapper {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(25rem, 1fr));
    grid-gap: 4rem;
    color: #000;
    margin-top: 6rem;
  }

  &-box {
    padding: 2rem;
    height: 35rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    position: relative;

    &:hover {
      border: solid 2px #fff;
      color: #fff;
    }
  }
  .project-box:nth-child(1) {
    background: linear-gradient(to bottom, #f3cbab, #feedca);
  }
  .project-box:nth-child(2) {
    background: linear-gradient(to bottom, #b1e5f9, #f4d2fe);
  }
  .project-box:nth-child(3) {
    background: linear-gradient(to bottom, #dbb4f3, #efb7d7);
  }
  .project-box:nth-child(4) {
    background: linear-gradient(to bottom, #efa971, #e4cafe);
    .project-box__link {
      width: min-content;
    }
  }
  .project-box:nth-child(5) {
    background: linear-gradient(to right, #b1e5f9, #f4d2fe);
    .project-box__link {
      width: min-content;
    }
  }

  &-box__link {
    align-self: flex-end;
    width: 20%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    @media only screen and (max-width: 56.25em) {
      width: 30%;
    }
  }
  &-box__content {
    align-self: center;
  }
}

:hover state .project-box:nth-child(1),
.project-box:nth-child(2),
.project-box:nth-child(3),
.project-box:nth-child(4),
.project-box:nth-child(5) {
  background: linear-gradient(to bottom, #f3cbab, #feedca);
  &:after {
    content: "";
    position: absolute;
    width: 103%;
    height: 101%;
    top: 1rem;
    right: 0;
    z-index: -1;
  }
  &:hover {
    background: none;
    background-color: #000;
  }
  &:hover img {
    filter: invert(1);
  }
  &:hover:after {
    outline: 2px solid #fff;
  }
}
</style>
<script></script>
