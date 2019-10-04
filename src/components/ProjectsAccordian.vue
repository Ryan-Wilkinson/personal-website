<template>
  <div class="accordian-container">
    <h1 class="title">
      Personal Projects
    </h1>
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <div class="container-general">
            <div class="gallery-wrap wrap-effect-1">
              <div class="item" />
              <div class="item" />
              <div class="item" />
              <div class="item" />
              <div class="item" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper'

export default {
  name: 'ProjectsAccordian',
  data() {
    return {}
  },
  created() {
    Swiper('.swiper-container', {
      direction: 'vertical',
      mousewheel: {},
      effect: 'cube',
      keyboard: {
        enabled: true,
        onlyInViewport: false,
      },
    })
  },
}
</script>
<style lang="scss" scoped>
.accordian-container {
  display: flex;
  flex-direction: column;
  color: #fff;
  width: 100%;
  padding-bottom: 30px;
}

.title {
  color: black;
  align-self: center;
  font-size: 3em;
  margin-top: 0;
}

.swiper-container {
  width: 100%;
  height: 90%;
}

.swiper-slide {
  text-align: center;
  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

// Image Accordions General
.container-general {
  margin: 0 auto;
  width: 800px;
  .gallery-wrap {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: 70vh;
    .item {
      flex: 1;
      height: 100%;
      background-position: center;
      background-size: cover;
      background-repeat: none;
      transition: all 0.8s ease;
      &:hover {
        flex: 7;
      }
    }
  }
}

// Image Accordions Effect 1
.wrap-effect-1 {
  .item {
    &:first-of-type {
      background-image: url('../../public/images/hangman.jpg');
    }
    &:nth-of-type(2) {
      background-image: url('../../public/images/mountacular.jpg');
    }
    &:nth-of-type(3) {
      background-image: url('../../public/images/playbillify.jpg');
    }
    &:nth-of-type(4) {
      background-image: url('../../public/images/goldfish.jpg');
    }
    &:last-of-type {
      background-image: url('../../public/images/citi2citi.jpg');
    }
  }
}

.inspire {
  border: 1px solid rgba(22, 76, 167, 0.6);
  border-radius: 10px;
  cursor: pointer;
  overflow: hidden;
  position: relative;
  text-decoration: none;
  margin: 10px;
  padding: 10px;
  &:after {
    background: #38ef7d;
    content: '';
    height: 155px;
    left: -75px;
    opacity: 0.4;
    position: absolute;
    top: -50px;
    transform: rotate(35deg);
    transition: all 550ms cubic-bezier(0.19, 1, 0.22, 1);
    width: 50px;
    z-index: -10;
  }
  &:hover {
    &:after {
      left: 120%;
      transition: all 550ms cubic-bezier(0.19, 1, 0.22, 1);
    }
  }
}

@keyframes rotate {
  0% {
    transform: rotate(0deg) translate3d(0, 0, 0);
  }
  25% {
    transform: rotate(10deg) translate3d(0, 0, 0);
  }
  50% {
    transform: rotate(-10deg) translate3d(0, 0, 0);
  }
  75% {
    transform: rotate(5deg) translate3d(0, 0, 0);
  }
  100% {
    transform: rotate(0deg) translate3d(0, 0, 0);
  }
}
</style>
