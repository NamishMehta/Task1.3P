<template>
    <div>
      <h1>This is My Resume</h1>
  
      <section id="work-experience">
        <h2>Work Experience</h2>
  
        <ul>
          <li>
            <li>None at the Moment</li>
          </li>
        </ul>
      </section>
  
      <section id="education">
        <h2>Education</h2>
  
        <ul>
          <li>
            <h3>Bachelor of Information Technology</h3>
            <p>Deakin University, Melbourne</p>
            <p>2023 - Present</p>
          </li>
        </ul>
      </section>
  
      <section id="skills">
        <h2>Skills</h2>
  
        <ul>
          <li>Vue.js</li>
          <li>HTML</li>
          <li>JavaScript</li>
          <li>CSS</li>
          <li>C++</li>
        </ul>
      </section>
  
      <section id="contact">
        <h2>Contact</h2>
  
        <form action="/contact" method="post">
          <input type="text" name="name" placeholder="Your Name">
          <input type="email" name="email" placeholder="Your Email">
          <textarea name="message" placeholder="Your Message"></textarea>
          <button type="submit">Submit</button>
        </form>
      </section>
    </div>
  </template>
  
  <script setup>
  </script>
  
  <style>
    body {
      font-family: sans-serif;
    }
  
    h1 {
      text-align: center;
      font-size: 2rem;
    }
  
    section {
      margin-bottom: 2rem;
    }
  
    ul {
      list-style: none;
      padding: 0;
    }
  
    li {
      margin-bottom: 1rem;
    }
  
    h2 {
      font-size: 1.5rem;
    }
  
    h3 {
      font-size: 1.25rem;
    }
  
    form {
      margin: 0 auto;
      width: 50%;
    }
  
    input, textarea {
      width: 100%;
      padding: 0.5rem;
      margin-bottom: 1rem;
    }
  
    button {
      background-color: blue;
      color: white;
      padding: 0.5rem;
      border: none;
      cursor: pointer;
    }
  </style>
  