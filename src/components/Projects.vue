<template>
  <div class="mx-auto max-w-7xl px-6 lg:px-8">
    <h2
      class="text-7xl bg-white animate-text bg-gradient-to-r from-pink-500 via-purple-500 to-blue-500 bg-clip-text text-transparent font-black pt-6 text-center"
    >
      Projects
    </h2>
    <div
      class="mx-auto mt-16 grid auto-rows-fr grid-cols-1 sm:mt-20 lg:mx-0 lg:max-w-none lg:grid-cols-2 gap-12"
    >
      <div class="nft w-full">
        <div class="main">
          <img
            class="tokenImage"
            src="https://images.unsplash.com/photo-1621075160523-b936ad96132a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
            alt="NFT"
          />
        </div>
      </div>
      <div class="nft w-full">
        <div class="main">
          <img
            class="tokenImage"
            src="https://images.unsplash.com/photo-1621075160523-b936ad96132a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
            alt="NFT"
          />
        </div>
      </div>
      <div class="nft w-full">
        <div class="main">
          <img
            class="tokenImage"
            src="https://images.unsplash.com/photo-1621075160523-b936ad96132a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
            alt="NFT"
          />
        </div>
      </div>
      <div class="nft w-full">
        <div class="main">
          <img
            class="tokenImage"
            src="https://images.unsplash.com/photo-1621075160523-b936ad96132a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
            alt="NFT"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "vue3-carousel/dist/carousel.css";

export default {
  components: {},
};
</script>
<style scoped>
.nft {
  user-select: none;
  margin: 5rem auto;
  border: 1px solid #ffffff22;
  background-color: #282c34;
  background: linear-gradient(
    0deg,
    rgba(40, 44, 52, 1) 0%,
    rgba(17, 0, 32, 0.5) 100%
  );
  box-shadow: 0 7px 20px 5px #00000088;
  border-radius: 0.7rem;
  backdrop-filter: blur(7px);
  -webkit-backdrop-filter: blur(7px);
  overflow: hidden;
  transition: 0.5s all;
  hr {
    width: 100%;
    border: none;
    border-bottom: 1px solid #88888855;
    margin-top: 0;
  }
  ins {
    text-decoration: none;
  }
  .main {
    display: flex;
    flex-direction: column;

    padding: 1rem;
    .tokenImage {
      border-radius: 0.5rem;
      max-width: 100%;

      object-fit: cover;
    }
    .description {
      margin: 0.5rem 0;
      color: #a89ec9;
    }
    .tokenInfo {
      display: flex;
      justify-content: space-between;
      align-items: center;
      .price {
        display: flex;
        align-items: center;
        color: #ee83e5;
        font-weight: 700;
        ins {
          margin-left: -0.3rem;
          margin-right: 0.5rem;
        }
      }
      .duration {
        display: flex;
        align-items: center;
        color: #a89ec9;
        margin-right: 0.2rem;
        ins {
          margin: 0.5rem;
          margin-bottom: 0.4rem;
        }
      }
    }
    .creator {
      display: flex;
      align-items: center;
      margin-top: 0.2rem;
      margin-bottom: -0.3rem;
      ins {
        color: #a89ec9;
        text-decoration: none;
      }
      .wrapper {
        display: flex;
        align-items: center;
        border: 1px solid #ffffff22;
        padding: 0.3rem;
        margin: 0;
        margin-right: 0.5rem;
        border-radius: 100%;
        box-shadow: inset 0 0 0 4px #000000aa;
        img {
          border-radius: 100%;
          border: 1px solid #ffffff22;
          width: 2rem;
          height: 2rem;
          object-fit: cover;
          margin: 0;
        }
      }
    }
  }
  ::before {
    position: fixed;
    content: "";
    box-shadow: 0 0 100px 40px #ffffff08;
    top: -10%;
    left: -100%;
    transform: rotate(-45deg);
    height: 60rem;
    transition: 0.7s all;
  }
  &:hover {
    border: 1px solid #ffffff44;
    box-shadow: 0 7px 50px 10px #000000aa;
    transform: scale(1.015);
    filter: brightness(1.3);
    ::before {
      filter: brightness(0.5);
      top: -100%;
      left: 200%;
    }
  }
}

.bg {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  h1 {
    font-size: 20rem;
    filter: opacity(0.5);
  }
}
</style>
