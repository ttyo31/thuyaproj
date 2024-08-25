<template>
    <div class="hobby-page" style="background-color: #EAF4FC;">
      <div class="header-section">
        <h1>My Hobby: Badminton</h1>
      </div>
      
      <div class="hobby-content">
        <div class="hobby-description">
          <p>
            During my free time, one of my favorite hobbies that I like to partake in is playing badminton. It is a great way for me to be able to relax and keep fit after a long day of work or school.
            Usually in a week, I try to play badminton roughly about 3 times a week. 
          </p>
        </div>
        
        <div class="hobby-gallery">
          <h3>Some of My Favorite Shots</h3>
          <div class="image-grid">
            <div class="image-card">
              <!-- <img src="../assets/photography1.jpg" alt="Landscape Photo" class="gallery-image"> -->
            </div>
            <div class="image-card">
              <!-- <img src="../assets/photography2.jpg" alt="Portrait Photo" class="gallery-image"> -->
            </div>
            <div class="image-card">
              <!-- <img src="../assets/photography3.jpg" alt="Nature Photo" class="gallery-image"> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  <script>
  export default {
    name: 'HobbyPage',
    data() {
      return {
        hobbyImages: [
          { src: require('../assets/logo.png'), alt: 'Landscape Photo' },
          { src: require('../assets/logo.png'), alt: 'Portrait Photo' },
          { src: require('../assets/logo.png'), alt: 'Nature Photo' }
        ]
      };
    }
  };
  </script>
<style scoped>
.hobby-page {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 50px;
}

.header-section h1 {
  font-size: 36px;
  color: #1A3E59;
  margin-bottom: 20px;
  border-bottom: 2px solid #1A3E59;
  display: inline-block;
}

.header-section p {
  font-size: 18px;
  color: #555;
  margin-bottom: 40px;
}

.hobby-content {
  margin: 0 auto;
  max-width: 800px;
  text-align: left;
}

.hobby-description h3 {
  font-size: 24px;
  color: #1A3E59;
  margin-bottom: 15px;
}

.hobby-description p {
  font-size: 16px;
  color: #666;
  margin-bottom: 20px;
}

.hobby-gallery h3 {
  font-size: 24px;
  color: #1A3E59;
  margin-bottom: 15px;
  text-align: center;
}

.image-grid {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.image-card {
  margin: 10px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.gallery-image {
  width: 100%;
  height: auto;
  display: block;
}
</style>
  