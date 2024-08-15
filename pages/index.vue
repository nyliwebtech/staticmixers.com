<template>
  <div class="container">
    <section class="hero">
      <div class="media">
        <div ref="player" class="player">
          <video
            preload="metadata"
            webkit-playsinline
            playsinline
            muted
            loop
            autoplay
            @canplay="videoFadeIn"
          >
            <source
              src="https://cms.mixers.com/assets/881E5694-4D8A-45C9-A9AA-72F9852D4792"
              type="video/mp4"
            >
          </video>
        </div>
      </div>
      <div class="mediaHero flex">
        <div class="flex flex-nowrap flex-justify-center wrapper">
          <div class="heroText">
            <h1>ROSS is a leader in Motionless Mixers for turbulent and laminar flow.
            </h1>
            <uiButton href="/how-it-works/">
              How to Select a Static Mixer

            </uiButton>
          </div>
          <div class="photoBox flex50">
            <img
              src="https://cms.mixers.com/assets/84F13387-43D5-4B15-8EE1-FDC0C070949A?width=1000&height=1000&format=webp"
              class="photo"
              alt="ROSS Inline High Shear Mixer"
              width="800"
            >
          </div>
        </div>
      </div>
    </section>
    <section class="flex flex-justify wrapper py-3 mobile-col-reverse bb-light">
      <div data-aos="fade-right" class="photo flex40">
        <img
          src="https://cms.mixers.com/assets/72E23C43-0AC9-4A66-BE8C-D4D55F7A05A9?width=800&height=1000&format=webp"
          alt="Static Mixer"
          width="800"
          height="1000"
        >
      </div>
      <div data-aos="fade-up" class="content py-3 flex55">
        <h4>Industrial Mixing Equipment</h4>
        <h2>Static Mixers</h2>
        <p><b>Ross is a leader in the design of Motionless Mixing Systems.</b> Our Static Mixers are well proven for wide ranging uses in turbulent and laminar flow applications, supplied as complete plug-in modules or as mixer inserts for installation into an existing pipe. Popular options include jacket for heating or cooling, injection ports with removable quill and special materials of construction. </p>

<p><b>Ross offers two basic designs:</b></p>
<ul class="txtList">
	<li>ISG - Interfacial Surface Generator for high viscosity, laminar flow mixing. </li>
	<li>LPD or LLPD - Low Pressure Drop for low viscosity, turbulent flow mixing. </li>
</ul>

<p>For many decades, Ross has supplied Static Mixers for installation in refineries and oil sampling pipelines, water and wastewater treatment plants, R&D and manufacturing facilities for chemicals, food, plastics, composites, adhesives, sealants, pharmaceuticals, pulp & paper, biodiesel, industrial gases, and many other applications. </p>


        <uiButton href="/how-it-works/">
          How it Works
        </uiButton>
      </div>
    </section>
    <section data-aos="fade-up" class="py-3 bgwave">
      <div class="wrapper">
        <h4>Design Options</h4>

        <div class="flex flex-justify">
          <div class="flex47" style="text-align:center;">
            <img
              src="https://cms.mixers.com/assets/A54D4CFE-789F-4197-8E12-DA556F850C89?height=700&format=webp"
              alt="ISG Motionless Mixers"
              width="400"
              height="400"
            >
            <h3>Interfacial Surface Generator</h3>
            <p>Ideal solution for high viscosity, laminar flow mixing.</p>
          </div>
          <div class="flex47" style="text-align:center;">
            <img
              src="https://cms.mixers.com/assets/B1CEBC7A-BC18-4FAF-84BE-6D0224CD8661?width=700&format=webp"
              alt="LPD Motionless Mixers"
              width="400"
              height="400"
            >
            <h3>Low Pressure Drop</h3>
            <p>Ideal for low viscosity, turbulent flow mixing.</p>
          </div>

        </div>
      </div>
    </section>
    <section data-aos="fade-up" class="slideIndustries py-3">
      <div class="wrapper flex flex-justify mobile-col-reverse">
        <div class="flex40 highlightPhoto">
          <img
            src="https://cms.mixers.com/assets/2315BA47-7197-4D70-839F-E6B6CF555AD0?width=1000&height=1200&format=webp"
            alt="Industries Served"
            width="500"
            height="600"
          >
        </div>
        <div class="flex50 z10">
          <h4>Industries Served</h4>
          <h2>Recommended Mixing Equipment for Water and Wastewater Treatment</h2>
          <p>Static Mixers allow for continuous dosing and blending of treatment chemicals into water and wastewater. Flocculants, disinfectants, neutralizing agents, pH conditioners and other chemicals are conveniently added into a flowing water stream and completely mixed within a relatively short length of pipe.</p>

            <p>Used in conjunction with automated instrumentation, Ross Low Pressure Drop Static Mixers deliver predictable quality control based on a virtually maintenance-free operation.
          </p>

        <p>
          <uiButton href="/resources/">
            Tech Reports
          </uiButton>
        </p>
          <br><br>
          <div class="infobox">
            <p>
              Ross Low Pressure Drop (LPD) Static Mixers are typical installations in water and wastewater treatment facilities around the world. These mixers consist of a series of baffles or "elements" discriminately positioned in series.
            </p>
            <div class="arrowpipe" />
          </div>
          <br><br><br><br>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import appConfig from '~/app.config';


useSeoMeta({
  title: 'Ross High Shear Mixers: Ross High Shear Mixer homogenizers are used for a wide range of Process Applications in the adhesive, cosmetic, pharmaceutical, food and chemical markets',
  description: 'Ross designs and manufactures industrial high shear mixers, dispersers,  for the process industries. Our high shear batch and inline mixers, sanitary mixers and blenders, vacuum homogenizers and other industrial mixing equipment are used for liquid/solid – liquid/liquid and solid/solid mixing and blending applications in the adhesive, battery, chemical, cosmetic, electronics, food, pharmaceutical and plastic industries.',
  ogImage: 'https://cms.mixers.com/assets/F9F0DE78-24AE-418B-8310-D40B1A93236C?width=1200&format=webp'
})

const player = ref(null)

const videoFadeIn = () => {
  player.value.classList.add('playable')
}

</script>

<style scoped>
section {
  position: relative;
}

section.hero {
  width: 100%;
}

.bgwave:before {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  opacity: 0.2;
  background: url('https://cms.mixers.com/assets/19A0383E-5208-452F-9C9F-5BB2E091BA07?format=webp')
    no-repeat;
  background-size: contain;
  background-position: center center;
}

.player {
  position: absolute;
  width: 100%;
  top: 0;
  left: 0;
  height: 630px;
  overflow: hidden;
  opacity: 0;
  transition: 0.3s all;
}

.player.playable {
  opacity: 0.2;
}

.player video {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.mediaHero {
  height: 630px;
  box-sizing: border-box;
  background: var(--navy-gray);
}

.mediaHero .wrapper {
  padding: 3rem;
  box-sizing: border-box;
}

.mediaHero .photoBox {
  z-index: 5;
  position: relative;
  transform:translateY(0rem);
  text-align:right;
}

.mediaHero .photoBox img {
  max-width:600px;
}

.mediaHero .photoBox-vmc {
  min-width: 500px;
  max-width: 600px;
  flex-grow: 2;
  flex-basis: 50%;
}

.mediaHero .photoBox .opener {
  position: absolute;
  bottom: 340px;
  right: 0px;
  width: 100px;
  padding-right: 0.6rem;
  height: 70px;
  background: #58eb93;
  z-index: -1;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  cursor: pointer;
  transition: 0.3s all;
}

.mediaHero .photoBox .opener.active {
  right: -10px;
  transition: 0.3s all;
}

.mediaHero .photoBox .clickopener {
  position: absolute;
  bottom: 340px;
  right: 0px;
  width: 100px;
  padding-right: 0.6rem;
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  cursor: pointer;
}

.mediaHero .photoBox .opener svg {
  width: 50px;
  height: auto;
}

.mediaHero img.photo {
  object-fit: cover;
  width: 100%;
  height: auto;
}

.heroText {
  flex-grow: 1;
  flex-basis: 40%;
}

.heroText h1 {
  font-size: 3rem;
  line-height: 4rem;
  color: #fff;
}

.bgtriangle:before {
  content: '';
  border-right: 40rem solid transparent;
  border-top: 40rem solid rgba(231, 244, 255, 0.54);
  position: absolute;
  width: 0;
  height: 0;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 0;
}

.light h2 {
  color: #fff;
}

.light p {
  color: #6d809b;
}

.slideIndustries {
  background: #e0ebf4;
}

.slideIndustries .highlightPhoto img {
  object-fit: cover;
  height: calc(100% + 6rem);
}

.slideIndustries .highlightPhoto {
  transform: translateY(-3rem);
  transition: 0.3s all;
  position: relative;
  z-index: 0;
}

.slideIndustries .highlightPhoto::before {
  content: '';
  position: absolute;
  width: 7.07rem;
  height: 7.07rem;
  background: #6d809b;
  box-sizing: border-box;
  transform: rotate(0deg);
  transform-origin: top left;
  z-index: -5;
  transition: 0.3s all;
  top: 0rem;
  right: -5rem;
}

.slideIndustries .highlightPhoto::after {
  content: '';
  position: absolute;
  width: 8rem;
  height: 8rem;
  background: #e0ebf4;
  transition: 0.3s all;
  z-index: -1;
  top: 0rem;
}

.slideProducts p {
  font-size: 1.1rem;
}

.slideProducts .highlight {
  align-items: flex-end;
  margin-top: -7rem;
  transform: translateY(8rem);
}

.slideProducts .highlightPhoto {
}

.slideProducts .highlightPhoto img {
  margin: 0;
  padding: 0;
  float: left;
}

.slideProducts .highlightContent {
  background: var(--bright-blue);
  padding: 3rem;
  box-sizing: border-box;
  position: relative;
  margin-bottom: 8rem;
}

.slideProducts .highlightContent p {
  color: #fff;
  font-size: 1.1rem;
}

.slideProducts .highlightContent::before {
  content: '';
  position: absolute;
  border-top: 8rem solid var(--bright-blue);
  border-left: 8rem solid transparent;
  right: 0;
  bottom: -8rem;
}

.arrowpipe {
  bottom: -4rem;
  right: -6rem;
  z-index: 5;
  position: absolute;
  width: 25rem;
  height: 0.6rem;
  background: #fff;
}

.arrowpipe::before {
  content: '';
  width: 2.5rem;
  height: 2.5rem;
  background: #fff;
  display: block;
  transform: rotate(225deg);
  position: absolute;
  right: 0;
  bottom: -0.95rem;
}

.infobox {
  background: #fff;
  box-shadow: 10px 10px 0px #bbcfe0;
  padding: 2rem;
  position: relative;
  z-index: 1;
  transform: translateX(-3rem);
}

.infobox p {
  font-size: 0.9rem;
  margin-bottom: 0;
}

.infobox .arrowpipe {
  transform: rotate(180deg);
  bottom: 50%;
  left: -20em;
  z-index: -1;
}

.highlightContent a {
  color: #fff;
}


@media screen and (max-width: 768px) {
  .player,
  .mediaHero {
    height: 400px;
  }

  .mediaHero .wrapper {
    padding: 1.5rem;
  }

  .heroText {
    width: 100%;
    margin: 0;
  }

  .heroText h1 {
    font-size: 2rem;
    line-height: 2.4rem;
  }

  .mediaHero .photoBox {
    min-width: 0;
    display: none;
  }

  .arrowpipe {
    width: 10rem;
  }

  .underHead {
    padding-bottom: 0px;
  }

  .underHead .wrapper {
    padding: 1rem 2rem;
    transform: translateY(-3rem);
  }

  .underHead .wrapper section {
    margin-right: 0rem;
  }

  .bgwave:before {
    background-position: top center;
  }

  .bynumbers-list div {
    border-right: 0;
    padding: 0rem;
  }

  .infobox {
    transform: translateX(0rem);
  }

  .slideProducts .arrowpipe {
    display: none;
  }

  .slideProducts .highlightContent {
    margin-bottom: 0;
  }

  .slideProducts .highlightContent::before {
    content: none;
  }

  .slideIndustries {
    margin-top: 0rem;
  }
}
</style>
