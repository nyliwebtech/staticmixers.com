<template>
  <div class="container">
    <main>
    <section class="wrapper py-3 bb-light">
        <h1>Static Mixer Resources</h1>
        <p>
          Providing the most insight and information towards our line of static mixers, our Resources section is designed to help customers make the right choices when selecting the proper blender in their next application.
        </p>
      </section>
      <section class="wrapper flex flex-justify py-3 bb-light">
        <div class="highlightReport flex60 mb-2">
          <a href="https://www.mixers.com/resources/mixing-technology-reports/continuous-static-mixing-of-multiple-process-streams/" target="_blank"><img src="https://cdn.mixers.com/images/mti/mti_45-static-mixer-large.jpg" style="width:100%; object-fit:cover; aspect-ratio:16/9;"></a>
          <h2>Continuous static mixing of multiple process streams</h2>
          <p class="excerpt">
            In many processes, mixing in pipelines is simpler and more economical than in vessels. In particular, continuous large-scale mixing of multiple liquid streams is easily accomplished in a static mixer arrangement. Advantages include fast blending, low maintenance, easy installation, and low energy requirement.
          </p>
        </div>
        <div class="featuredReports flex35">
          <h2 class="secondary">
            Featured Reports
          </h2>
          <ul>
            <li v-for="freport in data.mixing_technology_reports" :key="freport.id" class="bb-light">
              <nuxtLink target="_blank" :to="'https://www.mixers.com/resources/mixing-technology-reports/' + freport.slug + '/'">
                <h3>
                  {{ freport.title }}
                </h3>
              </nuxtLink>
            </li>
          </ul>
          <UiButtonExternal href="https://www.mixers.com/resources/mixing-technology-reports/">
            View ALl Tech Reports
          </UiButtonExternal>
        </div>
      </section>
      <section class="wrapper py-3 bb-light">
        <h2>White Papers and Articles</h2>
        <div class="flex flex-justify">
          <UiCard class="flex30"
            href="https://www.mixers.com/resources/whitepapers/static-mixer-designs-and-applications/"
            :image="{
              id: '334bf234-e0e5-4d5d-9b84-cac17a66076c.png',
              filename_disk : '334bf234-e0e5-4d5d-9b84-cac17a66076c.png'
            }"
            title="Static Mixer Designs and Applications"
          >
          Originally developed for niche markets, static mixers today serve a broader user base and have become more widespread throughout the process industries. Their high performance, low operating and maintenance cost, durability and continuous operation make them very appealing tools for improving mixing, emulsification, reaction and heat transfer.
          </UiCard>
          <UiCard class="flex30"
            href="https://cdn.mixers.com/articles/hsm_biomas_article.pdf"
            :image="{
              id: '334bf234-e0e5-4d5d-9b84-cac17a66076c.png',
              filename_disk : '334bf234-e0e5-4d5d-9b84-cac17a66076c.png'
            }"
            title="Shear Business for Biodiesel"
          >
          As demand for renewable fuels increase, inline high shear and static mixers get the nod.
          </UiCard>
          <div class="flex30"></div>
        </div>
      </section>
    </main>
  </div>
</template>

<script setup>
import appConfig from '~/app.config'

useSeoMeta({
  title: 'High Shear Mixers - Mixing Technical Articles and White Papers',
  description: 'Providing the most insight and information towards our high shear mixers, our Resources section is designed to help customers make the right choices when selecting the proper blender in their next application.',
  ogImage: 'https://cms.mixers.com/assets/F9F0DE78-24AE-418B-8310-D40B1A93236C?width=1200&format=webp'
})

const { data } = await useAsyncGql({
  operation: 'TechReports',
  variables: { limit: 5, cat: 'Static Mixers' }
});
</script>

<style scoped>
.highlightReport h2 {
  font-size: 2rem;
  line-height: 1.4;
  margin-top:2rem;
}

.highlightReport .media {
  width: 100%;
  padding-top: 66%;
  position: relative;
}

.highlightReport .media img {
  position: absolute;
  top: 0;
  width: 100%;
}

.featuredReports ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.featuredReports h2 {
  font-size: 2rem;
}

h3.resultHeader {
  font-size: 2rem;
  color: var(--text-highlight-secondary);
  border-bottom: 3px solid var(--text-highlight-secondary);
}

.featuredReports ul li {
  margin: 0;
  padding: 1rem 0rem;
}

.featuredReports ul li:last-child {
  border-bottom:0px;
}

.featuredReports ul li h3 {
  font-size: 1rem;
  margin: 0rem;
  margin-bottom: 0.2rem;
  line-height: 1.4rem;
}

.featuredReports ul li a {
  color: inherit;
  text-decoration: inherit;
  transition: 0.3s all;
}

.featuredReports ul li a:hover {
  color: var(--bright-blue);
}


</style>
