<template>
<div class="container mt-5">
  <h2>FAQ</h2>
  <div class="accordion" id="faqAccordion">

    <!-- First Question -->
    <div class="accordion-item">
      <h2 class="accordion-header" id="faqHeading1">
        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#faqCollapse1" aria-expanded="true" aria-controls="faqCollapse1">
        {{ $t('FAQ.QuestionOne') }}
        </button>
      </h2>
      <div id="faqCollapse1" class="accordion-collapse collapse show" aria-labelledby="faqHeading1" data-bs-parent="#faqAccordion">
        <div class="accordion-body">
          {{ $t('FAQ.BodyOne') }}
        </div>
      </div>

    </div>

    

    <!-- Second Question -->
    <div class="accordion-item">
      <h2 class="accordion-header" id="faqHeading2">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#faqCollapse2" aria-expanded="false" aria-controls="faqCollapse2">
          {{ $t('FAQ.QuestionTwo') }}
        </button>
      </h2>
      <div id="faqCollapse2" class="accordion-collapse collapse" aria-labelledby="faqHeading2" data-bs-parent="#faqAccordion">
        <div class="accordion-body">
          {{ $t('FAQ.BodyTwo') }}
        </div>
      </div>
    </div>

    <!-- Third Question -->
    <div class="accordion-item">
      <h2 class="accordion-header" id="faqHeading3">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#faqCollapse3" aria-expanded="false" aria-controls="faqCollapse3">
          {{ $t('FAQ.QuestionThree') }}
        </button>
      </h2>
      <div id="faqCollapse3" class="accordion-collapse collapse" aria-labelledby="faqHeading3" data-bs-parent="#faqAccordion">
        <div class="accordion-body">
          {{ $t('FAQ.BodyThree') }}
        </div>
      </div>
    </div>

  </div>
</div>

</template>

<script>



export default {
  name: 'FAQ',
  props: {
   content: String
  },
  created() {
    this.language=localStorage.getItem('language')
  }
  
};
</script>

<style scoped>
.container {
  margin-bottom: 15vh;
}
</style>
