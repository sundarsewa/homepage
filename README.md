<!-- Add this code right after the <body> tag in your Blogger template -->
<b:section id='homepage-wrapper' showaddelement='no'>
<div class='homepage-container'>
  
  <!-- Hero Section with 3D Accounting Elements -->
  <section class='hero-section'>
    <div class='hero-content'>
      <h1>Professional Accounting Services in Nepal</h1>
      <p>Trusted financial solutions for businesses and individuals</p>
      <div class='hero-buttons'>
        <a href='#services' class='btn-primary'>Our Services</a>
        <a href='#contact' class='btn-secondary'>Contact Us</a>
      </div>
    </div>
    <div class='hero-3d'>
      <div class='accounting-cube'></div>
      <div class='financial-chart'></div>
      <div class='document-stack'></div>
    </div>
  </section>

  <!-- Services Section -->
  <section id='services' class='services-section'>
    <h2 class='section-title'>Our Accounting Services</h2>
    <div class='services-grid'>
      <div class='service-card'>
        <div class='service-icon'>📊</div>
        <h3>Tax Accounting</h3>
        <p>Comprehensive tax planning and preparation services</p>
      </div>
      <div class='service-card'>
        <div class='service-icon'>💼</div>
        <h3>Business Accounting</h3>
        <p>Full-service accounting for businesses of all sizes</p>
      </div>
      <div class='service-card'>
        <div class='service-icon'>🔍</div>
        <h3>Audit Services</h3>
        <p>Thorough financial audits to ensure compliance</p>
      </div>
      <div class='service-card'>
        <div class='service-icon'>📈</div>
        <h3>Financial Consulting</h3>
        <p>Strategic advice for financial growth and stability</p>
      </div>
    </div>
  </section>

  <!-- Team Section -->
  <section class='team-section'>
    <h2 class='section-title'>Meet Our Expert Team</h2>
    <div class='team-grid'>
      <div class='team-member'>
        <img src='https://www.sundarsewa.com.np/your-team-photo1.jpg' alt='Team Member'/>
        <h3>Member Name</h3>
        <p>Position/Role</p>
        <div class='social-links'>
          <a href='#'>LinkedIn</a>
          <a href='#'>Email</a>
        </div>
      </div>
      <!-- Add more team members as needed -->
    </div>
  </section>

  <!-- Testimonials -->
  <section class='testimonials-section'>
    <h2 class='section-title'>What Our Clients Say</h2>
    <div class='testimonial-slider'>
      <div class='testimonial'>
        <p>"Sundar Sewa transformed our financial management completely!"</p>
        <div class='client-info'>
          <span>- Happy Client</span>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section id='contact' class='cta-section'>
    <h2>Ready to Transform Your Finances?</h2>
    <p>Contact us today for a free consultation</p>
    <a href='/contact' class='btn-primary'>Get Started</a>
  </section>

</div>
</b:section>

<!-- Add this CSS in the <head> section or in Blogger's CSS editor -->
<style>
.homepage-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  font-family: 'Poppins', sans-serif;
}

/* Hero Section Styles */
.hero-section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: 80vh;
  background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
  padding: 40px;
  border-radius: 20px;
  margin-bottom: 60px;
  position: relative;
  overflow: hidden;
}

.hero-content h1 {
  font-size: 3.5rem;
  color: #2c3e50;
  margin-bottom: 20px;
}

.hero-content p {
  font-size: 1.5rem;
  color: #7f8c8d;
  margin-bottom: 30px;
}

.hero-buttons {
  display: flex;
  gap: 20px;
}

.btn-primary {
  background: #3498db;
  color: white;
  padding: 12px 30px;
  border-radius: 50px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
}

.btn-secondary {
  background: transparent;
  color: #3498db;
  padding: 12px 30px;
  border-radius: 50px;
  border: 2px solid #3498db;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
}

/* 3D Elements */
.hero-3d {
  position: relative;
  width: 50%;
  height: 400px;
  perspective: 1000px;
}

.accounting-cube {
  position: absolute;
  width: 150px;
  height: 150px;
  transform-style: preserve-3d;
  animation: rotate 15s infinite linear;
  right: 50px;
  top: 50px;
}

/* Services Section */
.services-section {
  margin-bottom: 80px;
}

.section-title {
  text-align: center;
  font-size: 2.5rem;
  color: #2c3e50;
  margin-bottom: 50px;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
}

.service-card {
  background: white;
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
  text-align: center;
}

.service-card:hover {
  transform: translateY(-10px);
}

.service-icon {
  font-size: 3rem;
  margin-bottom: 20px;
}

/* Team Section */
.team-section {
  margin-bottom: 80px;
}

.team-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
}

.team-member {
  background: white;
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  text-align: center;
}

.team-member img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 20px;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-section {
    flex-direction: column;
    text-align: center;
  }
  
  .hero-3d {
    width: 100%;
    margin-top: 40px;
  }
  
  .hero-buttons {
    justify-content: center;
  }
}

/* Animation */
@keyframes rotate {
  0% { transform: rotateY(0deg); }
  100% { transform: rotateY(360deg); }
}
</style>

<!-- Add this JavaScript before the closing </body> tag -->
<script>
// Simple animation for 3D elements
document.addEventListener('DOMContentLoaded', function() {
  const cube = document.querySelector('.accounting-cube');
  let rotation = 0;
  
  setInterval(() => {
    rotation += 1;
    cube.style.transform = `rotateY(${rotation}deg)`;
  }, 50);
});
</script>
