<template>
  <!-- <div class="indigo darken-4 d-flex align-center mb-4" :aspect-ratio="3"> -->
  <div>
    <v-img cover gradient="#595B86,#595B86" :aspect-ratio="6" class="d-flex align-center mb-4 secondary">
      <p class="mx-8 my-4 d-flex justify-center align-center text-h2 text-white font-weight-medium title">
        Contact Us
      </p>
    </v-img>
    <!--<div class="d-flex align-center justify-center">
      <iframe class="mx-auto d-flex align-center justify-center" src="https://docs.google.com/forms/d/e/1FAIpQLSeLyZ9pGAXYWuLiis2-hCV4fqdIQqy4gR74Q0ns2b7NBYHlPg/viewform?embedded=true" width="640" height="963" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
    </div>-->
    <div class="mx-md-16 my-16">
      <Block title="Hello, World!">
        <template v-slot:title>
          Hello, World!
        </template>
        <p class="body-1 mx-md-8">
          For general questions about the team or interest in what we're doing, please reach Cornell Data Science
          at <a href="mailto: cornelldatascience@gmail.com">cornelldatascience@gmail.com</a>!
          <br />
          <br />
          If you are a company interested in sponsoring us, please view our sponsorship packet below, and reach
          out to us
          if you have any questions.
        </p>
      </Block>
      <Block title="Sponsorship Packet">
        <template v-slot:title>
          Sponsorship <br /> Packet
        </template>
        <v-expansion-panels>
          <v-expansion-panel>
            <v-expansion-panel-title>
              <div class="text-h4 secondary--text">Open to View</div>
            </v-expansion-panel-title>
            <v-expansion-panel-text class="d-flex justify-center px-auto">
              <v-row justify="center">
                <iframe class="mx-auto mt-2"
                  src="https://docs.google.com/presentation/d/e/2PACX-1vRs4rrovYiIcWlG3ByrGVFu29-JNx_94b4JD_h7W5z8llzwr-eH94KzAuumMIgi6-k2Kl5if6-NX4AD/embed?start=true&loop=false&delayms=3000"
                  frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true"
                  webkitallowfullscreen="true"></iframe>
              </v-row>
            </v-expansion-panel-text>
          </v-expansion-panel>
        </v-expansion-panels>
        <div class="my-4 mx-md-8">
          <a plain text href="../../CDS_Sponsorship_Sp22.pdf" class="text-h6 primary--text text-decoration-none">Download
            PDF</a>
        </div>
      </Block>
      <br />
    </div>
  </div>
</template>

<script setup lang="ts">
const contactImg = getImgUrl('people.jpg')

useHead({ title: "Contact" })
</script>