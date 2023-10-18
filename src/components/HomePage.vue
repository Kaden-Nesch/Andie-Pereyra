<template>
  <div class="pictures">
    <div class="image-container">
      <div class="img__wrap" @mouseenter="showTooltip('BUG BITE')" @mouseleave="resetImage">
        <img
          ref="mosquitoImage"
          src="../assets/moskeet.jpeg"
          class="mosquito"
          alt="Mosquito"
        />
        <div class="img__description">{{ tooltipText }}</div>
      </div>
    </div>
    </div>
    <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('AYCE')" @mouseleave="resetImage">
      <img
        src="../assets/ballz.jpg"
        class="ball"
        alt="Ball"
      />
      <div class="img__description" v-if="tooltipText === 'AYCE'">AYCE</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('BEEIRCING')" @mouseleave="resetImage">
      <img
        src="../assets/bee.jpeg"
        class="bee"
        alt="Bee"
      />
      <div class="img__description" v-if="tooltipText === 'BEEIRCING'">BEEIRCING</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('MERMAID')" @mouseleave="resetImage">
      <img
        src="../assets/mermaid.jpg"
        class="mermaid"
        alt="Mermaid"
      />
      <div class="img__description" v-if="tooltipText === 'MERMAID'">MERMAID</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('CUPOD')" @mouseleave="resetImage">
      <img
        src="../assets/cupod.jpeg"
        class="cupod"
        alt="Cupod"
      />
      <div class="img__description" v-if="tooltipText === 'CUPOD'">CUPOD</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('EYES SMALL LIKE')" @mouseleave="resetImage">
      <img
        src="../assets/ant.jpeg"
        class="ant"
        alt="Ant"
      />
      <div class= "img__description" v-if="tooltipText === 'EYES SMALL LIKE'">EYES SMALL LIKE</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('KAIN TAYO')" @mouseleave="resetImage">
      <img
        src="../assets/vj.jpeg"
        class="vj"
        alt="VJ"
      />
      <div class="img__description" v-if="tooltipText === 'KAIN TAYO'">KAIN TAYO</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('Crowded Mind')" @mouseleave="resetImage">
      <img
        src="../assets/tuna.jpeg"
        class="tuna"
        alt="Tuna"
      />
      <div class="img__description" v-if="tooltipText === 'Crowded Mind'">CROWDED MIND</div>
    </div>
  </div>
  <div class="pictures">
    <div class="image-container" @mouseenter="showTooltip('PRETTY PILL')" @mouseleave="resetImage">
      <img
        src="../assets/flower.jpg"
        class="flower"
        alt="flower"
      />
      <div class= "img__description" v-if="tooltipText === 'PRETTY PILL'">PRETTY PILL</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  data() {
    return {
      tooltipText: '',
    };
  },
  methods: {
    showTooltip(name) {
      this.tooltipText = name;
    },
    resetImage() {
      this.tooltipText = '';
    },
  },

};
</script>

<style scoped>
.pictures {
  text-align: center;
  margin-top: 50px;
}

.image-container {
  position: relative;
  display: inline-block;
}

/* Apply the width to the image using a class */
.mosquito {
  width: 40vw; /* 40% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
  transition: filter 0.3s ease; /* Add transition effect to filter property */
}



.ball:hover{
  filter: grayscale(80%); /* Turn the image grey on hover */
}

.img__description {
  position: absolute;
  bottom: 50%;
  left: 50%;
  transform: translateX(-50%);
  color: rgb(255, 255, 255);
  display: none;
  font-size: 80px;
  font-weight:bolder;
  cursor: pointer; /* Add a pointer cursor on hover */
}


.image-container:hover .img__description {
  display: block; /* Show the tooltip on image hover */
}

.image-container:hover .mosquito{
  filter: grayscale(80%);
}
.image-container:hover .ball{
  filter: grayscale(80%);
}
.image-container:hover .bee{
  filter: grayscale(80%);
}
.image-container:hover .mermaid{
  filter: grayscale(80%);
}
.image-container:hover .cupod{
  filter: grayscale(80%);
}
.image-container:hover .ant{
  filter: grayscale(80%);
}

.image-container:hover .vj{
  filter: grayscale(80%);
}

.image-container:hover .tuna{
  filter: grayscale(80%);
}

.image-container:hover .flower{
  filter: grayscale(80%);
}

@media only screen and (max-width: 1170px) {
  .img__description {
  position: absolute;
  bottom: 50%;
  left: 50%;
  transform: translateX(-50%);
  color: rgb(255, 255, 255);
  display: none;
  font-size: 30px;
  font-weight:bolder;
  cursor: pointer; /* Add a pointer cursor on hover */
}
}

@media only screen and (max-width: 600px) {
  .img__description {
  position: absolute;
  bottom: 50%;
  left: 50%;
  transform: translateX(-50%);
  color: rgb(255, 255, 255);
  display: none;
  font-size: 15px;
  font-weight:bolder;
  cursor: pointer; /* Add a pointer cursor on hover */
}
  
}

.ball {
  width: 50vw; /* 50% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}

.bee {
  width: 35vw; /* 40% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}

.cupod{
  width: 50vw; /* 60% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}

.ant{
  width: 40vw; /* 60% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}

.vj{
  width: 50vw; /* 60% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}
.mermaid{
  width: 40vw; /* 60% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}
.tuna{
  width: 40vw; /* 60% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}

.flower{
  width: 40vw; /* 60% of the viewport width */
  max-width: 100%; /* Ensure the image does not exceed its natural width */
  height: auto; /* Maintain the image's aspect ratio */
  border-radius: 10px;
  cursor: pointer; /* Add a pointer cursor on hover */
}

</style>