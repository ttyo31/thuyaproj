<template>
  <div class="home">
  <div class="container-fluid" style="padding: 0;margin: 0;width: 100%;">
    <div class="row grey" style="margin-left: 0;text-align: start;">
      <div class="col-4">
        <h1>
          I am an aspiring
          <br>
  <a class="typewrite" data-period="2000" data-type='["Web developer","Data Analyst"]'>
    <span class="wrap"></span>
  </a>
  <br>
  From SMU
</h1>

      </div>
      <div class="col-4">
        <div>
          <img src="../assets/thuya.jpg" alt="" style="padding-bottom: 10px;border-radius: 100%;" class="round-image">
        </div>

      </div>
      <div class="col-4">
        <div>
          <p style="font-size: 30px;font-family: 'Comic Sans MS'">
            Looking for Internship:
            <br>
            <b>Jan 2025 - June 2025 <br>
              <p style="color: #b9393a;font-size: 30px">(6 Months)</p> </b>
          </p>

        </div>

      </div>
    </div>
    <div style="background-color: #eae2d6;">
      <div class="row" style="align-items: start;">
        <div class="col-5">
          <p style="font-size: 40px;font-family: 'Georgia', serif; font-size: 40px;font-weight: bold;"><b>
              Who Am I?
            </b>
          </p>
          <p style="font-size: 16px;text-align: left;padding-left: 5px;"><b>
              Hello, I'm Thuya, a Year 3 Information Systems student at Singapore Management University (SMU). I am
              dual-tracking in Business Analytics and Digitisation & Cloud Solutions, with a second major in
              Cybersecurity.
              My passion lies in the evolving tech landscape, particularly in how data is leveraged to innovate and
              improve lives. Recognizing the critical importance of data security, I chose to pursue Cybersecurity to
              complement my studies and ensure that the data-driven solutions I work on are well-protected.
            </b>
          </p>
        </div>

        <div class="col-2"></div>
        <div class="col-5" style="text-align: left; padding-left: 40px;">
          <div class="skills-section">
            <p style="font-size: 30px;font-family: 'Georgia', serif; font-weight: bold;color: #b9393a;">
              <b>Hard Skills:</b>
            </p>
            <ol style="font-size: small;">
              <li>Python</li>
              <li>SQL</li>
              <li>JavaScript</li>
              <li>Web Development</li>
              <li>Docker/Containerization</li>
              <li>Spreadsheet Modelling using Excel</li>
              <li>Basics understanding of Cyber security</li>
              <li>Java <b>(In Progress)</b></li>
              <li>Object Oriented Programming <b>(In Progress)</b></li>
              <li>Data Analytics <b>(In Progress)</b></li>
            </ol>
          </div>
        </div>


      </div>
      <br>
      <div class="row" style="background-color: #f1f1f1;padding-top: 20px; text-align: center;position: relative;border-radius: 100px;">
        <div class="col-12">
          <h2>Personal Projects/Achievements</h2>
        </div>
      </div>
      <div class="row">
        <div class="col-4 box">
          <div class="row">
            <h4>Profile website</h4>
          </div>
          <div class="row">
            <img src="../assets/profilewebsite.png"class ="round">
          
          </div>
          <div class="row">
            <p style="text-align: start;">
              This is a personal project to showcase some of my personal web development skill whilst creating a MyPortfolio
              website that is easy for people to look through. The website is deployed on Github and was made using VueJS.
              <br>
              <br>
              <b>Frontend:</b>
              <br>VueJS Framework
              <br>Bootstrap+CSS
              <br>HTML
            </p>
          </div>
          <div class="row">
            <p></p>
          </div>
        </div>
        <div class="col-4 box">
          <div class="row">
            <h4>Bookquest Webapp For school</h4>
          </div>
          <div class="row">
            <img src="../assets/bookquest.png"class ="round">
          </div>
          <div class="row">
            <p style="text-align: start;">This was a school project in which we were tasked to design a Web application. My contribution to this specific project
was in the form of designing the skill tree portion of bookquest, which used CSS to design the tree itself and used a 
simple algorithm + api call to google books to sort the new books into the skill tree.
              <br>
              <br>
              
<b>Frontend:</b><br>

Bootstrap 5 
Vue3
SceneJS
<br>
<b>Backend</b><br>
Laravel-Breeze Template<br>

Laravel PHP<br>
<b>Database:</b><br>
MySQL<br>
<b><a href="https://youtu.be/bEcbRV4Oa6U">Website Demo</a></b><br>
<b><a href="https://github.com/ZhiLinR/WAD2-Book-App">Github Link</a></b>

</p>
          </div>
        </div>
        <div class="col-4 box">
          <div class="row">
            <h4>Google Cybersecurity Course</h4>
          </div>
          <div class="row">
            <img src="../assets/cybersecurity.png"class ="round">
          </div>
          <div class="row">
            <p style="text-align: start">
              This is a google cert in cybersecurity that I have obtained over the summer of 2024.This certification gave
              me a better glimpse into the world of cybersecurity. It taught me the importance of cybersecurity to ensure 
              the compliance of the CIA triad. It also give me the basic's of using SIEM tools and linux command line to 
              retrieve logs. I was also taught the basics on how to analyse logs and weed out suspicious behaviour that
              could be due to attacks.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div>
    </div>
  </div>

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  mounted() {
    var TxtType = function(el, toRotate, period) {
        this.toRotate = toRotate;
        this.el = el;
        this.loopNum = 0;
        this.period = parseInt(period, 10) || 2000;
        this.txt = '';
        this.tick();
        this.isDeleting = false;
    };

    TxtType.prototype.tick = function() {
        var i = this.loopNum % this.toRotate.length;
        var fullTxt = this.toRotate[i];

        if (this.isDeleting) {
        this.txt = fullTxt.substring(0, this.txt.length - 1);
        } else {
        this.txt = fullTxt.substring(0, this.txt.length + 1);
        }

        this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

        var that = this;
        var delta = 200 - Math.random() * 100;

        if (this.isDeleting) { delta /= 2; }

        if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
        } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
        }

        setTimeout(function() {
        that.tick();
        }, delta);
    };

    var elements = document.getElementsByClassName('typewrite');
    for (var i=0; i<elements.length; i++) {
        var toRotate = elements[i].getAttribute('data-type');
        var period = elements[i].getAttribute('data-period');
        if (toRotate) {
          new TxtType(elements[i], JSON.parse(toRotate), period);
        }
    }
    // INJECT CSS
    var css = document.createElement("style");
    css.type = "text/css";
    css.innerHTML = ".typewrite > .wrap { border-right: 0.08em solid #fff}";
    document.body.appendChild(css);
  }
}
</script>

<style>
#HomeView {
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
  height: 250px;
}

.round-image {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 50%;
  overflow: hidden;
  border: 10px solid #f1e8db;
  /* Adds a ring-like border */
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
}

.custom-navbar {
  background-color: #f1e8db;
  /* Matches the navbar background color */
  font-family: 'Georgia', serif;
  /* Optional: Matches the font style */
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

.custom-navbar {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);

}

.skills-section {
  border: 2px solid black;
  padding: 15px;
  border-radius: 5px;
  background-color: #dfeffc;
}

body {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

.container-fluid {
  padding: 0;
  margin: 0;
  width: 100%;
}

.row {
  margin-left: 0;
  margin-right: 0;
}
.box{
  border: 2px solid black;
  padding: 15px;
  border-radius: 5px;
}
.round {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 50%;
  overflow: hidden;
  border: 10px solid #f1e8db;

}
</style>
