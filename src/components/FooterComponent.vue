<template>
  <footer class="amazing-footer">
    <div class="footer-content">
      <div class="footer-section">
        <h4>About</h4>
        <p>
          We are a team of hardworking developers trying to create and
          provide the best user experience.
        </p>
      </div>
      <div class="footer-section">
        <h4>Links</h4>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Portfolio</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h4>Reach Out</h4>
        <p><i class="fas fa-map-marker-alt"></i> ABC Street, VIC, Australia</p>
        <p><i class="fas fa-phone"></i> +61 987 654 321</p>
        <p><i class="fas fa-envelope"></i> mehtanamish4@icloud.com</p>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2023 NamishDevOnTop. All rights reserved.</p>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped>
.amazing-footer {
  background-color: grey;
  color: white;
  padding: 40px 0;
  font-family: "Arial", sans-serif;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.footer-section {
  flex: 1;
  margin-right: 20px;
}

.footer-section:last-child {
  margin-right: 0;
}

.footer-section h4 {
  border-bottom: 2px solid black;
  padding-bottom: 10px;
  margin-bottom: 20px;
}

.footer-section p,
.footer-section li {
  margin-bottom: 10px;
}

.footer-section a {
  color: white;
  text-decoration: none;
  transition: color 0.3s;
}

.footer-section a:hover {
  color: black;
}

.footer-bottom {
  text-align: center;
  margin-top: 40px;
  border-top: 1px solid black;
  padding-top: 20px;
}

.fas {
  margin-right: 10px;
}
</style>
