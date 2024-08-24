<template>
  <div class="Work experiences">
    <div class="container-fluid" style="padding: 0;margin: 0;width: 100%;">
      <div class="row grey" style="margin-left: 0;text-align: start;">
        <div class="col-12">
          <h1>Professional Experiences</h1>
          <p>
            Explore some of the key experiences that have shaped my professional journey. Each experience showcases the
            skills, responsibilities, and achievements that have contributed to my growth.
          </p>
        </div>
      </div>
    </div>
    

    <div class="container">
      <!-- Experience 1 -->
      <div class="experience row">
        <div class="col-8">
        <h3>Sales assistant @ Jimei Flower</h3>
        <p><b>Company/Organization:</b> Jimei</p>
        <p><b>Role:</b> Sales Assistant</p>
        <p><b>Duration:</b> Dec 2016 - Feb 2017</p>
        <p>So basically this was my first ever job that I had. It was when I had just finished O-levels and was waiting
          for the results to come out. So basically, in this job, we had to interact with customers who were there to buy
          Christmas trees, get their order and schedule their orders to their house. We also handled communications with 
          the delivery staff and had to coordinate their deliveries based on both delivery date and area. 
        </p>
        <p><b>Skills Learned:</b>Effective Communication, Sales,Patience in working with a team</p>
      </div>
      <div class="col-4">
        <img src="../assets/logo.png" class="round-image" >
      </div>
      </div>
      <div class="experience row">
        <div class="col-8">
        <h3>National Service</h3>
        <p><b>Company/Organization:</b> SAF</p>
        <p><b>Role:</b> Driver</p>
        <p><b>Duration:</b> 2019-2021</p>
        <p>During my national service, I was a driver for 1st transport Alpha company. Our company was incharge of moving
          bullets and transporting vehincles using low loaders. Due to our specialisation even amongst other transport 
          company, it made my national service more rewarding, fun and even scary at times. We were trained not just in
          class 3 but also class 4 and class 4a vehicles. Initially, it was very scary to drive such a huge vehicle on 
          the road espicially knowing that 1. You could easily collide with another car if you are not too careful and 2.
          if we do get into a traffic accident, it could be a huge catostraphe due to the live ordinance that we were carrying.
          It took me awhile to get over this fear and only through many trial and error was I finally confident enough to 
          drive the low loader. 
        </p>
        <p><b>Skills Learned:</b>Teamwork, Attention to detail, Problem Solving</p>
      </div>
      <div class="col-4">
        <img src="../assets/logo.png" class="round-image" >
      </div>
      </div>
      <div class="experience row">
        <div class="col-8">
        <h3>M1 digital ambassador</h3>
        <p><b>Company/Organization:</b> M1 Pte Ltd</p>
        <p><b>Role:</b> Digital ambassador</p>
        <p><b>Duration:</b>Feb 2021 - May 2021</p>
        <p>So this was the job that I took on after I finished my national service. In this job, I was tasked with teaching
          M1 customers on how to use their phone, digital app and also in charge of dispensing a queue ticket for their 
          enquiries. I was the first line of contact for anyone that walks into a M1 shop. This job was particularly
          challenging as often times I had to communicate with elderly or people who are less techincally saavy, and
          in most cases, it often takes quite alot of patience to teach them how to do things. I was also tasked with
          managing queue times, by ensuring that queries that did not need to be raised to counter staff were resolved 
          so as to not make queutimes unnecessarily long. 
        </p>
        <p><b>Skills:</b>Patience, Tech literacy, Effective communication in multiple languages</p>
      </div>
      <div class="col-4">
        <img src="../assets/logo.png" class="round-image" >
      </div>
      </div>
      <!-- Experience 2 -->
      <div class="experience row">
        <div class="col-8">
        <h3>Samsung Mobile Phone Promoter</h3>
        <p><b>Company/Organization:</b> Samsung</p>
        <p><b>Role:</b> Mobile Phone promoter</p>
        <p><b>Duration:</b>May 2021 - Aug 2024</p>
        <p>This was my longest job that I ever had. So my job was to promote to customers Samsung mobile phone products.
          This job was made easier espicially because of the fact that my previous job was working in a Telco company, it
          meant that I had many transferable skills like being able to converse effectively in both English and Mandaring
          about this topic, being very literate espicially when it came to mobile phones and also I was experienced in
          working with many difficult customers

        </p>
        <p><b>Skills:</b>Customer service, Sales</p>
      </div>
      <div class="col-4">
        <img src="../assets/logo.png" class="round-image" >
      </div>
      </div>

      <!-- Experience 3 -->
      <div class="experience row">
        <div class="col-8">
        <h3>SMU student services hub</h3>
        <p><b>Company/Organization:</b> SMU</p>
        <p><b>Role:</b> Student advisor</p>
        <p><b>Duration:</b> Dec 2023- Now</p>
        <p>This is my current job that I have held for almost the past year. My job is stationed at the student service
          hub located in SMU. In this job, I help with student queries and direct them to the proper channels in which 
          they are able to resolve their queries. Through, this job has provided me with many unique experiences like
          interacting with students of different backgrounds and even allowed me to go up on stage to give a talk to 
          the Y1s for their course planning.
        </p>
        <p><b>Skills:</b>Customer service, Public speaking</p>
      </div>
      <div class="col-4">
        <img src="../assets/logo.png" class="round-image" >
      </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ExperiencesView'
};
</script>

<style scoped>
.experiences {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.grey {
  width: 100%;
  padding: 50px;
  background-color: #c1b5a7;
  height: auto;
}

.custom-navbar {
  background-color: #f1e8db;
  font-family: 'Georgia', serif;
  padding: 10px 20px;
}

.navbar-brand {
  font-size: 24px;
  font-weight: bold;
  color: #2c3e50;
}

.navbar-nav .nav-item .nav-link {
  font-size: 18px;
  color: #2c3e50;
  padding: 10px 15px;
  transition: color 0.3s, background-color 0.3s;
}

.navbar-nav .nav-item .nav-link:hover {
  color: #ffffff;
  background-color: #2c3e50;
  border-radius: 5px;
}

.navbar-nav .nav-item .nav-link.active {
  color: #ffffff;
  background-color: #2c3e50;
  border-radius: 5px;
}

.container {
  margin-top: 20px;
}

.experience {
  margin-bottom: 40px;
  text-align: left;
}

.round-image {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 50%;
  overflow: hidden;
  border: 10px solid #f1e8db;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
}
</style>
