<script setup lang="ts">
import { pageTransition } from '~~/assets/scripts/transition'

definePageMeta({
  pageTransition,
})

const services = [
  {
    title: 'Brand',
    items: [
      'Strategy',
      'Art Direction',
      'Identity Systems',
      'Merchandise',
      'Campaigns',
    ],
  },
  {
    title: 'Fashion',
    items: [
      '3D Wearables',
      'Digital Fashion',
      'Material Libraries',
      'Virtual Stores',
      'AR Dressing',
    ],
  },
  {
    title: 'Product',
    items: [
      'UIX',
      'Motion Design',
      'Creative Front-end',
      '3D Content',
      'Web XR',
    ],
  },
  {
    title: 'Web3',
    items: [
      'Advisory',
      'Design Sprints',
      'NFT Co-creation',
      'Generative NFTs',
      'Metaverse',
    ],
  },
]

const radios = [
  {
    idNumber: 1,
    name: 'Simplified',
  },
  {
    idNumber: 2,
    name: 'Scalable',
  },
  {
    idNumber: 3,
    name: 'Growth',
  },
]

const itemsInfo = [
  {
    mainText:
      'Sophisticated solutions meticulously crafted around the needs of your audience.',
    subText:
      'Utilising the power of <span class="home-8__underline-text">design & narrative</span>, we turn complex concepts into meaningful digital experiences, from <span class="home-8__underline-text">vision to launch</span>.',
    blocks: [
      'Bespoke Strategies',
      'Engaging Creative',
      'Streamlined Process',
      'Technical Expertise',
    ],
  },
  {
    mainText:
      'Design thinking allows inherent scalability of your products from the core.',
    subText:
      'Establishing <span class="home-8__underline-text">practical & purpose driven</span> systems builds versatile asset libraries, whilst affording the <span class="home-8__underline-text">flexibility of modularity</span>.',
    blocks: [
      'Collaborative Workflows',
      'Design Systems',
      'Modular Assets',
      'Reusable Libraries',
    ],
  },
  {
    mainText:
      'Expert knowledge catalyses your path to the forefront of the digital world.',
    subText:
      'Working diligently to <span class="home-8__underline-text">accelerate & amplify</span> your digital journey, through transparent partnerships and <span class="home-8__underline-text">agile implementations</span>.',
    blocks: [
      'Authentic Partnerships',
      'Data Driven',
      'Dynamic Solutions',
      'Innovative Applications',
    ],
  },
]

const links = [
  {
    textLink: '1kx',
  },
  {
    textLink: 'Astrid Andersen',
  },
  {
    textLink: 'Aura',
  },
  {
    textLink: 'BrightID',
  },
  {
    textLink: 'Carteblock',
  },
  {
    textLink: 'Connext',
  },
  {
    textLink: 'Gitcoin',
  },
]
</script>

<template>
  <section class="section section--nm home-1">
    <img class="home-1__bg" src="/images/main.jpg" alt="Background" />
    <div class="container home-1__wrapper">
      <h1 class="home-1__title">
        A multidisciplinary creative consultancy shaping
        <span class="home-1__underline-text"> digital culture </span>
      </h1>
    </div>
  </section>
  <section class="section home-2">
    <div class="container home-2__wrapper">
      <AboutInfo class="home-2__about-text"
        >Empowering brands at the forefront of digital
      </AboutInfo>
      <p class="home-2__text">
        Integral is a multi-disciplinary design studio, catalysing insights with
        technology to build thoughtful
        <span class="home-2__underline-text">design-led solutions</span> for
        dynamic global clients. <br /><br />
        From strategy, to creative direction and production, we deliver
        innovative and engaging experiences that
        <span class="home-2__underline-text"
          >connect brands with their audiences.</span
        >
      </p>
    </div>
  </section>
  <section class="section section--nm home-3">
    <HomeVideo class="home-3__bg" />
  </section>
  <section id="about" class="section home-4">
    <div class="container home-4__wrapper">
      <AboutInfo>About </AboutInfo>
      <div class="grid home-4__content">
        <div class="home-4__left-block">
          <h2 class="home-4__title">
            Redefining brand dimensionalities
            <span class="home-4__title-arrow">
              <IconsAngleArrow />
            </span>
          </h2>
          <img class="home-4__mobile-img" src="/images/1.jpg" alt="" />
          <div class="home-4__text-wrapper">
            <p class="home-4__med-desc">
              Operating at the intersection of physical & digital, specialising
              in; <span class="home-4__underline-text">brand</span>,
              <span class="home-4__underline-text">fashion</span>,
              <span class="home-4__underline-text">product</span> &
              <span class="home-4__underline-text">web3</span>.
            </p>
            <p class="home-4__small-desc">
              With deep knowledge broadly spanning design, fashion & web3, we
              help our partners grow through our innate understanding of the
              drivers behind tomorrow’s trends and opportunities.
            </p>
          </div>
          <div class="home-4__btn-wrapper">
            <TheButton> Studio </TheButton>
          </div>
        </div>
        <div class="home-4__right-block">
          <img class="home-4__img" src="/images/1.jpg" alt="" />
        </div>
      </div>
    </div>
  </section>
  <section class="section section--nm home-5">
    <div class="container home-5__wrapper">
      <img class="home-5__img" src="/images/2.jpg" alt="" />
    </div>
  </section>
  <section id="services" class="section section--nm home-6">
    <div class="container home-6__wrapper">
      <AboutInfo>Services </AboutInfo>
      <div class="grid home-6__info-wrapper">
        <div
          v-for="(el, idx) in services"
          :key="idx"
          class="home-6__info"
          :class="idx === 0 && 'home-6__info--active'"
        >
          <h3 class="home-6__title">
            {{ el.title }}
            <span class="home-6__info-arrow">
              <IconsAngleArrow />
            </span>
          </h3>
          <ul class="home-6__text-list">
            <li
              v-for="(elem, index) in el.items"
              :key="index"
              class="home-6__text-li"
            >
              <p class="home-6__text">
                <span class="home-6__symbol">¬ </span>{{ elem }}
              </p>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
  <section class="section section--nm home-7">
    <div class="grid container home-7__wrapper">
      <p class="home-7__text">
        We tailor each experience around your story, to create strategically
        aligned solutions
        <span class="home-7__underline-text"> as unique as your vision.</span>
      </p>
      <TheButton class="home-7__btn"> What’s your story </TheButton>
    </div>
  </section>
  <section id="approach" class="section section--nm home-8">
    <div class="container home-8__wrapper">
      <AboutInfo>Approach </AboutInfo>
      <div class="grid home-8__content">
        <div class="home-8__left-block">
          <img class="home-8__img" src="/images/3.jpg" alt="" />
        </div>
        <div class="home-8__right-block">
          <ul class="home-8__menu">
            <li
              v-for="(radio, id) in radios"
              :key="id"
              class="home-8__menu-btn"
            >
              <input
                :id="`home-8__input-radio${radio.idNumber}`"
                class="home-8__radio"
                type="radio"
                name="home-8__radios"
                checked
              />
              <label
                class="home-8__text"
                :for="`home-8__input-radio${radio.idNumber}`"
              >
                {{ radio.name }}
              </label>
            </li>
          </ul>
          <img class="home-8__mobile-img" src="/images/3.jpg" alt="" />
          <ul class="home-8__text-list">
            <li
              v-for="(item, idx) in itemsInfo"
              :key="idx"
              class="home-8__info"
              :class="idx === 0 && 'home-8__info--active'"
            >
              <div class="home-8__text-wrapper">
                <p class="home-8__main-text">
                  {{ item.mainText }}
                </p>
                <p class="home-8__subtext" v-html="item.subText" />
              </div>
              <div class="home-8__blocks-wrapper">
                <p
                  v-for="(block, id) in item.blocks"
                  :key="id"
                  class="home-8__block-name"
                >
                  {{ block }}
                </p>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
  <section class="section section--nm home-9">
    <div class="container home-9__wrapper">
      <AboutInfo>Trusted by </AboutInfo>
      <ul class="home-9__links-wrapper">
        <li v-for="(link, idx) in links" :key="idx" class="home-9__item">
          <a
            href="/"
            class="home-9__link"
            rel="noopener noreferrer"
            target="_blank"
          >
            {{ link.textLink }}
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>
