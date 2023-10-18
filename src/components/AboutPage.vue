<template>
  <div class="pictures">
    <div class="TextWrapper">
      <img src="../assets/Andie.jpg" class="andie" alt="Your Image">
      <div class="about">
        Andie Pereyra’s drawings are inspired by her Filipino heritage and suburban American upbringing. Her artwork explores what shapes our sense of identity and how this self evolves through a lifetime. Her colorful illustrations convey a sense of nostalgia which juxtaposes subject matter of feeling foreign in both Filipino and American communities. Her work centers on self-discovery and otherness, serving as a means to reconnect and reclaim space within both of her cultures.
      </div>
    </div>
    <div class="contact-info">
      <div class="contact-info-text">
        <p>pereyra.adrianna@gmail.com</p>
      </div>
      <a href="https://www.instagram.com/andie_pereyra/" target="_blank">
        <img src="../assets/ig.png" alt="Instagram Link" class="instagram-icon">
      </a>
    </div>
  </div>
</template>

<style scoped>
.pictures {
  text-align: center;
  margin-top: 100px;
}

.andie {
  max-width: 100%;
  height: auto;
  border-radius: 40px;
  width: 30vw;
}

.TextWrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
}

.about {
  font-size: 20px;
  color: black;
  width: 30%;
  line-height: 40px;
  margin-left: 50px;
}

/* Responsive Design */

@media only screen and (min-width: 2000px) {
  .about {
    width: 22%;
    line-height: 50px;
  }
}

@media only screen and (max-width: 1170px) {
  .andie {
    width: 70vw;
    margin-right: 20px;
  margin-left: calc(1/3 * 70vw); /* Position the image 1/3 through the page */
  border-radius: 40px;
  }
  .about {
    width: 100%; /* Make the text occupy full width */
    margin-left: 0; /* Remove margin on the left */
  }
}

/* Mobile Devices */
@media only screen and (max-width: 1170px) {
  .TextWrapper {
    flex-direction: column; /* Display content in columns on mobile */
    align-items: flex-start; /* Align content to the start */
    margin-left: 0; /* Remove margin on the left */
  }

  .andie {
    width: 100%; /* Make the image occupy full width on mobile */
    margin: 0; /* Remove margin on the image */
    border-radius: 40px;
  }

  .about {
    font-size: 16px; /* Adjust font size for mobile */
    width: 100%; /* Make text occupy full width on mobile */
  }
  
}

@media only screen and (min-width: 2000px) {

.contact-info {
  display: flex;
  align-items: center;
  margin-top: 10px;
  margin-left: 800px;

}

.contact-info-text {
  text-align: center;
  margin-right: 20px; 
  font-size: 20px;/* Add margin to the right of the text for spacing */
}

.instagram-link {
  display: flex;
  align-items: center;
  margin-top: 50px;
}

.instagram-icon {
  max-width: 30px;
  height: auto;
}

}

@media only screen and (max-width: 1999px) {

.contact-info {
  display: flex;
  align-items: center;
  margin-top: 10px;
  margin-left: 480px;

}

.contact-info-text {
  text-align: center;
  margin-right: 20px; 
  font-size: 20px;/* Add margin to the right of the text for spacing */
}

.instagram-link {
  display: flex;
  align-items: center;
  margin-top: 50px;
}

.instagram-icon {
  max-width: 30px;
  height: auto;
}

}
/* Mobile Styles */


@media only screen and (max-width: 1170px) {
  .contact-info {
    flex-direction: column; /* Display content in columns on mobile */
    align-items: center; /* Align content to the start */
    margin-left: 0; /* Remove margin on the left */

  }

  .contact-info-text {
    margin-right: 0; /* Remove the margin on the right of the text for mobile */
  }

  .instagram-link {
    margin-top: 10px; /* Adjust the top margin for better spacing on mobile */
  }
}
</style>


