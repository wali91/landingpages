<template>
<div class="container-fluid">
  <div class="container pt-5 pb-5">
    <div class="row justify-content-center">
      <div class="col-4  text-left">
      <h1 class="title pb-0 mb-0" style="font-weight:1000">DAMCorp</h1>
      <h5>PT Dam Korporindo Digital</h5>
      <p>Mangkuluhur City 7th floor
        Jl. Gatot Subroto Kav. 1 – 3
        Jakarta Selatan 12930</p>
      <p class="whatsapp mb-0 pb-0"><span style="font-weight:800">WhatsApp</span> : +62 811-1950-9333</p>
      <p class="email mt-0"><span style="font-weight:800">Email</span> : business.solution@damcorp.id</p>
    </div>
    <div class="col-2  text-left">
      <h4 style="font-weight:600">Sitemap</h4>
      <p class="textmargin link" ><a class="textmargin" aria-current="page" @click="toHome" >Home</a></p>
      <p class="textmargin link"><a class="textmargin" aria-current="page" @click="toSolutionPage">Solutions</a></p>
      <p class="textmargin link"><a class="textmargin" aria-current="page" @click="toPartnersPage">Partners</a></p>
      <p class="textmargin link"><a class="textmargin" aria-current="page" @click="toFAQPage">FAQ</a></p>
      <p class="textmargin">Platform</p>
    </div>
    <div class="col-2 text-left">
      <h4 style="font-weight:600">Our Products</h4>
      <p class="textmargin">Whatsapp Business</p>
    </div>
    <div class="col-3 text-left">
      <h4 style="font-weight:600">Follow Us</h4>
      <p class="textmargin">WhatsApp: +62 811-1950-9333</p>
<p class="textmargin">Instagram: <a class="custom-link" href="https://www.instagram.com/damcorpdigital/" target="_blank">@damcorpdigital</a></p>
<p class="textmargin">Facebook: <a class="custom-link" href="https://www.facebook.com/damcorp.id/" target="_blank">Damcorp.id</a></p>
<p class="textmargin">LinkedIn: <a class="custom-link" href="https://www.linkedin.com/company/damcorp-id/mycompany/" target="_blank">Damcorp.id</a></p>

    </div>
    </div>
  </div>
</div>
<div class="container bottom">
  <img src="@/assets/public/meta.png" height="90px">
  <h5 class="mt-1 text-left"><b>META</b> <br> <span style="font-size:16px;">Official Business Partner</span></h5>
</div>
</template>

<script>
export default {
    /* eslint-disable vue/multi-word-component-names */
  name: 'Footer',
  methods: {
   toHome() {
      this.$router.push(`/`);
    },
    toSolutionPage() {
      this.$router.push(`/solutionpage`);
    },
    toPartnersPage() {
      this.$router.push(`/partnerspage`);
    },
    toBlogPage() {
      this.$router.push(`/blogpage`);
    },
    toFAQPage() {
      this.$router.push(`/faq`);
    }
  }
};
</script>

<style scoped>
.container-fluid {
  background-color:#009C77;
  font-family: metrophobic;
  color:white;
}
.bottom {
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: metrophobic;
  height: 5vh;
  padding-top: 35px;
  background-color:white;

}
.text-left {
  text-align: left;
}
.textmargin {
  padding-bottom: 0;
  margin-bottom: 3%;
  color: white; /* Set your desired color */
  text-decoration: none; /* Remove underline */
  cursor: pointer;
}
.link:hover {
  text-decoration: underline; /* Underline only on hover */

}
.custom-link {
  color: white; /* Set your desired link color */
  text-decoration: none; /* Remove default underline */
}

.custom-link:hover {
  text-decoration: underline; /* Underline only on hover */
}

</style>
