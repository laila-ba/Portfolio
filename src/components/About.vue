<template>
  <section id="about" class="about reveal">
    <div class="about-card text-container">
      <div class="w-full max-w-xl xl:max-w-none xl:flex-auto xl:px-16 text-box">
        <img class="w-32" src="../assets/img//01-new.png" alt="" />
        <!-- <svg
          xmlns="http://www.w3.org/2000/svg"
          width="131"
          height="107"
          fill="none"
        >
          <path
            stroke="white
"
            stroke-width="2"
            d="m10.266 88.302.005.008c7.704 11.4 19.03 17.09 33.829 17.09 14.897 0 26.274-5.687 33.979-17.09l.005-.008C83.927 79.487 86.8 67.823 86.8 53.4c0-4.884-.33-9.452-.992-13.7h17.931V103h25.55V3.65H107.2l-.146.826c-.847 4.8-3.572 8.886-8.297 12.26l-.008.006c-4.602 3.356-10.34 5.11-17.274 5.208l-.986.014v.646a43.086 43.086 0 0 0-2.405-4.111C70.576 7.083 59.191 1.4 44.1 1.4c-14.994 0-26.328 5.685-33.835 17.1C4.423 27.314 1.55 38.977 1.55 53.4c0 14.423 2.873 26.087 8.716 34.902ZM27.25 53.4c0-8.924 1.192-15.803 3.5-20.713 1.433-2.864 3.256-4.958 5.447-6.341 2.19-1.384 4.812-2.096 7.903-2.096 3.091 0 5.712.712 7.904 2.096 2.193 1.385 4.017 3.482 5.452 6.351 2.4 4.8 3.644 11.672 3.644 20.703 0 9.031-1.244 15.902-3.644 20.703-1.435 2.869-3.26 4.966-5.453 6.352-2.19 1.384-4.812 2.095-7.903 2.095-3.091 0-5.712-.711-7.904-2.096-2.19-1.383-4.013-3.477-5.446-6.34-2.308-4.91-3.5-11.79-3.5-20.714Z"
          />
        </svg>-->
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
              <a href="#about">
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
  </section>
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
