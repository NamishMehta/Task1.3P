<template>
  <section class="about-me-page">
    <div class="profile-image">
      <img
        src="../assets/images/profilepic.jpg"
        alt="Your Name"
        class="hover-effect"
      />
    </div>
    <div class="about-content">
      <h1>About Me</h1>
      <p>
        Hello! My Name is Namish, I'm a passionate web developer with over 2 years
        of experience in creating responsive websites. I do this as a hobby and as a
        professional developer.
      </p>
      <p>
       I am currently studying at Deakin University in Bachelors of Information Technology and 
       I've been doing this side by side which is helping me in developing knowledge.
      </p>
      <p>
        I like to do this in my free time, I also love Travelling and exploring new places
      </p>
      <button class="download-btn">Download My Resume</button>
      <p>
        Thanks for viewing my portfolio. Wanna collaborate or chat???
        <a href="mailto:mehtanamish4@icloud.com">contact me</a>!
      </p>
    </div>
  </section>
</template>

<script setup>
// You can add any reactive properties or methods if needed.
</script>

<style scoped>
.about-me-page {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px 0;
  font-family: "Arial", sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  background-color: whitesmoke;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.profile-image {
  flex: 1;
  padding-right: 50px;
}

.profile-image img.hover-effect {
  max-width: 100%;
  border-radius: 50%;
  transition: transform 0.3s, box-shadow 0.3s;
}

.profile-image img.hover-effect:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

.about-content {
  flex: 2;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
}

.about-content h1 {
  font-size: 2.5em;
  margin-bottom: 20px;
}

.about-content p {
  margin-bottom: 20px;
  line-height: 1.6;
}

.about-content a {
  color: blue;
  text-decoration: none;
  transition: color 0.3s;
}

.about-content a:hover {
  color: black;
}

.download-btn {
  display: inline-block;
  background-color: grey;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s;
}

.download-btn:hover {
  background-color: black;
}
</style>
