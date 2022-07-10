<script>
  export default{
  data(){
    return{
    }
  },
  methods:{
    // CLICK on specific image
    CTA_click(isWhat){
      switch (isWhat) {
        case 'img1': console.log('IMAGE_01_SECTION_01_CTA')
         break;
        case 'img2': console.log('IMAGE_02_SECTION_01_CTA') 
          break;
        case 'img3': console.log('IMAGE_03_SECTION_01_CTA') 
          break;
        default:
          console.log('Error Occured')
      }
    }
  }
}

</script>

<template>
  <div class="flex items-center justify-center h-screen">
    <div class="flex md:flex-row ml-5">
      <div class="flex flex-row">
        <a @click="this.CTA_click('img1')">
        <img src="../../assets/images/section01/image-01.jpg">
        </a>
      </div>  
      
      <div class="flex flex-col ml-5">
        <div class="mb-5">
          <a @click="this.CTA_click('img2')">
          <img src="../../assets/images/section01/image-02.jpg">
          </a>
        </div>
        <div>
          <a @click="this.CTA_click('img3')">
          <img src="../../assets/images/section01/image-03.jpg">
          </a>
        </div>
      </div>
      <div class="ml-5">
        <span class="underline underline-offset-8 font-OpenSansRegular text-2xl tracking-wider">
          <p>
            ANSWER YOUR BODY'S NEEDS
          </p>
        </span>
        <span class="font-OpenSansLight text-base leading-loose tracking-wide">
          <p>
            The way ingredients are sourced affects the <br>
            way we nourish our bodies. Author Mark<br>
            Schatzer believes our body naturally develops<br>
            an appetite for the foods and nutrients it needs<br>
            to be healthy, but that artificial flavourings are<br>
            getting in the way. This can be reversed by<br>
            focousing on high-quality ingredients and being<br>
            mindful as your appetite guides you to<br>
            consume according to your body's needs.<br>
          </p>
        </span>
        <span class="">
          <p>
            BE MINDFUL
          </p>
        </span>
        <span class="">
          <p>
            Sourcing local or organic food is a good way<br>
            to start being more mindful about what<br>
            your're cooking and eating.
          </p>
        </span>
      </div>
    </div>
  </div>
</template>
