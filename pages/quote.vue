<template>
  <div class="container">
    <section class="wrapper py-3 bb-light flex flex-justify">
      <div class="headline flex40">
        <h1>Request a Quote</h1>
        <div class="arrowpipe" />
      </div>
      <div class="excerpt flex50 py-3">
        <p>
          To request more information about a particular mixer and application,
          or to request a quote, fill out our request form below. If you have
          any questions, don't hestitate to call us at 1-800-243-ROSS, or email
          us at <a href="mailto:mixers.com">mail@mixers.com</a>.
        </p>
      </div>
    </section>
    <main class="wrapper py-3">
      <FormsQuoteRequest showApplications="true"/>
    </main>
  </div>
</template>

<script setup>
useSeoMeta({
  title: 'Request a Quote, Purchase a Static Mixer Online',
  description: 'Static and motionless - no moving parts inline continuous mixers for food, chemical, petrochemical, wastewater applications',
  ogImage: 'https://cms.mixers.com/assets/A54D4CFE-789F-4197-8E12-DA556F850C89?height=700&format=webp'
})
</script>

<style scoped>

.arrowpipe {
  top: 2rem;
  left: 0rem;
  z-index: 5;
  position: relative;
  width: 80%;
  height: 0.4rem;
  background: var(--light-gray);
  float: left;
}

.arrowpipe::before {
  content: '';
  width: 1.8rem;
  height: 1.8rem;
  background: var(--light-gray);
  display: block;
  transform: rotate(225deg);
  position: absolute;
  right: 0;
  bottom: -0.7rem;
}

@media screen and (max-width: 768px) {
  .excerpt {
    margin-top:4rem;
  }
}

</style>