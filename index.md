---
layout: page
title: " "
---

<style>
.video-container {
  top: 0;
  left: 0;
  height: 100vh;
  width: 100%;
  overflow: hidden;
  z-index: 1;
  margin-bottom: -5px;
}

.video-container video {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.overlay-text {
  position: absolute;
  top: 70%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 2rem;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  animation: changeWord 5s infinite;
}

.overlay-text2 {
  position: absolute;
  top: 80%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 2rem;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  animation: changeWord 5s infinite;
}  

@keyframes changeWord {
  0% {
    content: "My";
  }
  33% {
    content: "research";
  }
  66% {
    content: "interest :";
  }
  100% {
    content: "X-ray Astronomy";
  }
}

.content-wrapper {
  margin-top: 100vh;
  padding: 2rem;
  margin-top: -5px;
}

.column.is-one-quarter {
  float: left;
  margin-right: 1rem;
}

.column:last-child {
  margin-bottom: 1rem;
}

@media screen and (max-width: 768px) {
 .column.is-one-quarter {
   float: none;
   margin-right: 0;
   margin-bottom: 1rem;
  }
}

</style>

<div class="video-container">
  <video autoplay muted loop>
    <source src="ic10_timelapse.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <div class="overlay-text">
    <h1>Hi ! I'm Sayantan </h1>
  </div>
  <div class="overlay-text2">
    <h3>My research interest : <span class="changing-word"></span></h3>
  </div>
</div>

<div class="content-wrapper">
  <!-- Rest of your content -->
  <section class="section">
    <div class="container">
      <div class="columns">
        <div class="column is-one-quarter">
          <img src="/assets/1.jpg" alt="Figure" width="100" height="200">
        </div>
        <div class="column">
          <p>
            I am a curious stargazer, eager to decipher the mysteries of the universe. Trained as a physicist, I find my solace in the heart of nature. I also have a keen interest in advanced computational techniques to make astronomy more interesting.
          </p>
        </div>
      </div>

      <p>
        I'm currently a PhD student at the Department of Physics and Applied Physics, University of Massachusetts, Lowell, MA. I also enjoy teaching undergraduate courses as a Graduate Teaching Assistant here.
      </p>

      <p>
        I'm a member of Dr. Silas Laycock's astronomy research group at LoCSST, UMass Lowell. Here you can find more information about my background, research interests, projects, and publications.
      </p>

      <p>
        For more information on any of my interests or to contact me personally, please feel free to reach out!
      </p>
    </div>
  </section>
</div>

<script>
// JavaScript to change the last word in the overlay text
document.addEventListener("DOMContentLoaded", function() {
  var changingWord = document.querySelector(".changing-word");
  var words = ["X-ray Astronomy", "Black Holes", "Massive Stars"];
  var index = 0;
  
  setInterval(function() {
    changingWord.textContent = words[index];
    index = (index + 1) % words.length;
  }, 2000);
});
</script>

