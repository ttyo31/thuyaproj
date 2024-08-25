<template>
    <div class="enriching-experiences" style="background-color: #EAF4FC;">
      <div class="header-section">
        <h1>Enriching Experiences</h1>
        <p>These are moments that have significantly contributed to my personal and professional growth, offering unique insights and learning opportunities.</p>
      </div>
      
      <div class="experience-grid">
        <!-- Experience 1 -->
        <div class="experience-card">
          <!-- <img src="../assets/excursion.jpg" alt="Excursion Image" class="experience-image"> -->
          <div class="experience-content">
            <h3>Meet Ventures Jakarta Immersion Trip</h3>
            <p>A short 1 week immersion trip, with a business consultancy project</p>
            <button class="learn-more" @click="openModal('experience1')">Learn More</button>
          </div>
        </div>
  
        <!-- Experience 2 -->
        <div class="experience-card">
          <!-- <img src="../assets/talk.jpg" alt="Giving a Talk" class="experience-image"> -->
          <div class="experience-content">
            <h3>Giving a seminar on Course Planning in SMU to Y1 students</h3>
            <p> A course planning seminar that I gave to the freshman, so as to allow them to properly plan their academic journey</p>
            <button class="learn-more" @click="openModal('experience2')">Learn More</button>
          </div>
        </div>
  
        <!-- Experience 3 -->
        <div class="experience-card">
          <!-- <img src="../assets/workshop.jpg" alt="Workshop Image" class="experience-image"> -->
          <div class="experience-content">
            <h3>Google Professional Certification In Cybersecurity</h3>
            <p>A google certifcation that I obtained over the summer holidays.</p>
            <button class="learn-more" @click="openModal('experience3')">Learn More</button>
          </div>
        </div>
      </div>
  
      <!-- Modal -->
      <div v-if="showModal" class="modal-overlay" @click.self="closeModal">
        <div class="modal-content">
          <img :src="currentExperience.image" class="modal-image">
          <h3>{{ currentExperience.title }}</h3>
          <p>{{ currentExperience.description }}</p>
          <button @click="closeModal" class="close-modal">Close</button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'EnrichingExperiences',
    data() {
      return {
        showModal: false,
        currentExperience: {},
        experiences: {
          experience1: {
            title: 'Jakarta Immersion Trip',
            description: 'During the summer of 2024, I went on a Jakarta Immersion trip that was organised by Meet Ventures in collaboration with National Youth Council. The purpose of the trip was to learn more Indonesia and the startup culture of Indonesia. During the trip, we were also tasked with a business consultancy project for one of our sponsor company. This trip was a very enriching experience as it gave me great insight on what it takes to be a startup founder and also about Indonesia as an up and coming economic powerhouse.',
            image: require('../assets/jakarta.jpeg')
          },
          experience2: {
            title: 'Course planning workshop',
            description: 'This was a unique oppourtunity that was offered to me due to me working at the student services hub. I was tasked with giving a talk to the freshman on how they should be planning for the academic career in SMU. In the talk, I also shared with the year 1s on the importance of planning of early and also the resources that were at their disposal, that would help them to easily plan their SMU journey.',
            image: require('../assets/sshoverview.jpeg')
          },
          experience3: {
            title: 'Google Cybersecurity course',
            description: 'This is a cybersecurity course that I took during the summer of 2024. Due to nature of the digital age that we are living in, a lot of data is produced on a daily basis. Proper utilisation of this data with technology allows us to have better standards of living, however, this data is also susceptible to malicious actors. This means that data security is also becoming paramount importance. Due to this, I felt that a knowledge in cybersecurity would benefit me in my journey as a web developer or data analyst.',
            image: require('../assets/cybersecurity.png')
          }
        }
      };
    },
    methods: {
      openModal(experienceKey) {
        this.currentExperience = this.experiences[experienceKey];
        this.showModal = true;
      },
      closeModal() {
        this.showModal = false;
        this.currentExperience = {};
      }
    }
  };
  </script>
  
  <style scoped>
  .enriching-experiences {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    color: #2c3e50;
    margin-top: 50px;
  }
  
  .header-section h1 {
    font-size: 36px;
    color: #1A3E59; /* Different color from Work Experience */
    margin-bottom: 20px;
    border-bottom: 2px solid #1A3E59;
    display: inline-block;
  }
  
  .header-section p {
    font-size: 18px;
    color: #555;
    margin-bottom: 40px;
  }
  
  .experience-grid {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }
  
  .experience-card {
    background-color: #f9f9f9;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    margin: 20px;
    width: 300px;
    transition: transform 0.3s ease;
  }
  
  .experience-card:hover {
    transform: translateY(-10px);
  }
  
  .experience-image {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
  }
  
  .experience-content {
    padding: 20px;
    text-align: left;
  }
  
  .experience-content h3 {
    font-size: 24px;
    color: #1A3E59;
    margin-bottom: 10px;
  }
  
  .experience-content p {
    font-size: 16px;
    color: #666;
    margin-bottom: 20px;
  }
  
  .learn-more {
    text-decoration: none;
    color: #ffffff;
    background-color: #1A3E59;
    padding: 10px 15px;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
  }
  .learn-more:hover {
    background-color: #3A6079;
  }
  
  /* Modal Styles */
  .modal-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.6);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
  }
  
  .modal-content {
    background-color: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    max-width: 500px;
    text-align: center;
  }
  
  .modal-image {
    width: 100%;
    height: auto;
    border-radius: 10px;
    margin-bottom: 20px;
  }
  
  .close-modal {
    background-color: #1A3E59;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    margin-top: 20px;
  }
  .close-modal:hover {
    background-color: #3A6079;
  }
  </style>
  