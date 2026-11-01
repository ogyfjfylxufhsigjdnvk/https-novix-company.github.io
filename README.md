HTML

<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#050914">
<title>NOVIX | Digital Innovation</title>

<style>
:root {
  --blue: #087cff;
  --cyan: #00c8ff;
  --bg: #050914;
  --card: #0c1425;
  --white: #ffffff;
  --muted: #a0aec0;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  background: var(--bg);
  color: var(--white);
  font-family: Arial, sans-serif;
  line-height: 1.7;
}

a { text-decoration: none; color: inherit; }

nav {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(5,9,20,.94);
  backdrop-filter: blur(15px);
  border-bottom: 1px solid #15233c;
  padding: 17px 7%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 27px;
  font-weight: 900;
  letter-spacing: 3px;
  color: var(--cyan);
  text-shadow: 0 0 18px #087cff;
}

.nav-links {
  display: flex;
  gap: 24px;
  align-items: center;
  font-size: 14px;
}

.nav-links a:hover { color: var(--cyan); }

.lang {
  border: 1px solid var(--blue);
  background: transparent;
  color: white;
  padding: 8px 14px;
  border-radius: 8px;
  cursor: pointer;
}

.hero {
  min-height: 88vh;
  padding: 100px 8%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  background:
    radial-gradient(ellipse at 50% 35%, #063b7c55, transparent 60%),
    var(--bg);
}

.tag {
  color: var(--cyan);
  border: 1px solid #087cff66;
  background: #087cff15;
  padding: 8px 18px;
  border-radius: 30px;
  font-size: 13px;
  margin-bottom: 25px;
}

.hero h1 {
  font-size: clamp(42px, 8vw, 82px);
  line-height: 1.15;
  font-weight: 900;
}

.hero h1 span {
  color: var(--cyan);
  text-shadow: 0 0 35px #087cff88;
}

.hero p {
  max-width: 650px;
  color: var(--muted);
  margin: 25px 0 32px;
  font-size: 17px;
}

.btn {
  display: inline-block;
  background: linear-gradient(110deg, #087cff, #00c8ff);
  color: white;
  padding: 13px 27px;
  border-radius: 9px;
  font-weight: bold;
  box-shadow: 0 0 25px #087cff44;
  transition: .3s;
  border: none;
  cursor: pointer;
}

.btn:hover {
  transform: translateY(-4px);
  box-shadow: 0 0 35px #087cff88;
}

section { padding: 85px 8%; }

.section-title {
  text-align: center;
  margin-bottom: 45px;
}

.section-title h2 {
  font-size: 36px;
  margin-bottom: 10px;
}

.section-title span { color: var(--cyan); }

.section-title p { color: var(--muted); }

.about {
  max-width: 850px;
  margin: auto;
  text-align: center;
  color: var(--muted);
  font-size: 17px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
}

.card {
  background: linear-gradient(145deg, #101d33, #090f1d);
  border: 1px solid #1c3151;
  padding: 28px;
  border-radius: 15px;
  transition: .3s;
}

.card:hover {
  transform: translateY(-7px);
  border-color: var(--blue);
  box-shadow: 0 10px 35px #087cff20;
}

.card .icon {
  font-size: 34px;
  margin-bottom: 15px;
}

.card h3 { margin-bottom: 10px; }

.card p { color: var(--muted); font-size: 14px; }

.project-label {
  display: inline-block;
  font-size: 11px;
  color: var(--cyan);
  margin-bottom: 10px;
  border: 1px solid #087cff55;
  padding: 3px 9px;
  border-radius: 20px;
}

.vision {
  text-align: center;
  background: linear-gradient(100deg, #071a36, #0a1020);
  border-top: 1px solid #163a68;
  border-bottom: 1px solid #163a68;
}

.vision p {
  max-width: 700px;
  margin: 15px auto;
  color: var(--muted);
}

.contact-wrap {
  max-width: 650px;
  margin: auto;
}

form {
  display: grid;
  gap: 15px;
}

input, textarea {
  width: 100%;
  padding: 15px;
  background: #0c1425;
  border: 1px solid #233858;
  border-radius: 9px;
  color: white;
  font: inherit;
}

textarea { min-height: 140px; resize: vertical; }

input:focus, textarea:focus {
  outline: 1px solid var(--blue);
}

#form-status {
  color: var(--cyan);
  text-align: center;
}

footer {
  padding: 35px 8%;
  text-align: center;
  border-top: 1px solid #182943;
  color: var(--muted);
}

footer .logo { margin-bottom: 10px; }

@media(max-width: 800px) {
  .grid { grid-template-columns: repeat(2, 1fr); }
  .nav-links { gap: 12px; font-size: 12px; }
}

@media(max-width: 560px) {
  nav { padding: 14px 5%; flex-wrap: wrap; gap: 12px; }
  .nav-links { order: 3; width: 100%; justify-content: center; }
  .grid { grid-template-columns: 1fr; }
  section { padding: 65px 6%; }
  .hero { min-height: 78vh; padding: 70px 6%; }
  .section-title h2 { font-size: 29px; }
}

[dir="rtl"] body { text-align: right; }
[dir="rtl"] .hero,
[dir="rtl"] .section-title,
[dir="rtl"] .vision,
[dir="rtl"] footer { text-align: center; }
</style>
</head>

<body>

<nav>
  <a href="#home" class="logo">NOVIX.</a>

  <div class="nav-links">
    <a href="#home" data-en="Home" data-ar="الرئيسية">Home</a>
    <a href="#about" data-en="About" data-ar="من نحن">About</a>
    <a href="#services" data-en="Services" data-ar="خدماتنا">Services</a>
    <a href="#projects" data-en="Projects" data-ar="مشاريعنا">Projects</a>
    <a href="#contact" data-en="Contact" data-ar="تواصل معنا">Contact</a>
  </div>

  <button class="lang" onclick="toggleLanguage()">العربية</button>
</nav>

<header class="hero" id="home">
  <div class="tag" data-en="WELCOME TO NOVIX" data-ar="مرحباً بك في نوفيكس">
    WELCOME TO NOVIX
  </div>

  <h1>
    <span data-en="INNOVATION" data-ar="الابتكار">INNOVATION</span>
    <br>
    <span data-en="STARTS HERE." data-ar="يبدأ من هنا.">STARTS HERE.</span>
  </h1>

  <p data-en="Building tomorrow's digital world through technology, creativity and innovation."
     data-ar="نبني عالم الغد الرقمي من خلال التكنولوجيا والإبداع والابتكار.">
    Building tomorrow's digital world through technology, creativity and innovation.
  </p>

  <a href="#services" class="btn"
     data-en="Explore Our Services" data-ar="اكتشف خدماتنا">
    Explore Our Services
  </a>
</header>

<section id="about">
  <div class="section-title">
    <h2 data-en="About <span>NOVIX</span>" data-ar="من نحن <span>NOVIX</span>">
      About <span>NOVIX</span>
    </h2>
    <p data-en="Technology with a vision" data-ar="تكنولوجيا برؤية مستقبلية">
      Technology with a vision
    </p>
  </div>

  <div class="about">
    <p data-en="NOVIX is a technology company focused on creating modern digital solutions. We transform ideas into innovative websites, applications and software experiences."
       data-ar="NOVIX شركة تكنولوجية تهتم بتطوير الحلول الرقمية الحديثة. نحول الأفكار إلى مواقع إلكترونية وتطبيقات وتجارب برمجية مبتكرة.">
      NOVIX is a technology company focused on creating modern digital solutions.
    </p>
  </div>
</section>

<section id="services">
  <div class="section-title">
    <h2 data-en="Our <span>Services</span>" data-ar="خدماتنا <span>الرقمية</span>">
      Our <span>Services</span>
    </h2>
    <p data-en="Solutions designed for the future"
       data-ar="حلول مصممة للمستقبل">Solutions designed for the future</p>
  </div>

  <div class="grid">

    <div class="card">
      <div class="icon">🌐</div>
      <h3 data-en="Website Development" data-ar="تطوير المواقع">Website Development</h3>
      <p data-en="Modern, responsive and professional websites."
         data-ar="مواقع إلكترونية حديثة واحترافية ومتجاوبة.">
        Modern, responsive and professional websites.
      </p>
    </div>

    <div class="card">
      <div class="icon">📱</div>
      <h3 data-en="Mobile Applications" data-ar="تطبيقات الموبايل">Mobile Applications</h3>
      <p data-en="Creative mobile app experiences."
         data-ar="تجارب تطبيقات موبايل مبتكرة.">
        Creative mobile app experiences.
      </p>
    </div>

    <div class="card">
      <div class="icon">💻</div>
      <h3 data-en="Software Solutions" data-ar="الحلول البرمجية">Software Solutions</h3>
      <p data-en="Smart software for modern businesses."
         data-ar="حلول برمجية ذكية للشركات الحديثة.">
        Smart software for modern businesses.
      </p>
    </div>

    <div class="card">
      <div class="icon">🎨</div>
      <h3 data-en="UI/UX Design" data-ar="تصميم واجهات المستخدم">UI/UX Design</h3>
      <p data-en="Beautiful and easy-to-use interfaces."
         data-ar="واجهات جميلة وسهلة الاستخدام.">
        Beautiful and easy-to-use interfaces.
      </p>
    </div>

    <div class="card">
      <div class="icon">🛡️</div>
      <h3 data-en="Cybersecurity" data-ar="الأمن السيبراني">Cybersecurity</h3>
      <p data-en="Helping protect digital systems and information."
         data-ar="المساعدة في حماية الأنظمة والمعلومات الرقمية.">
        Helping protect digital systems and information.
      </p>
    </div>

    <div class="card">
      <div class="icon">🚀</div>
      <h3 data-en="Digital Innovation" data-ar="الابتكار الرقمي">Digital Innovation</h3>
      <p data-en="Turning creative ideas into digital products."
         data-ar="تحويل الأفكار الإبداعية إلى منتجات رقمية.">
        Turning creative ideas into digital products.
      </p>
    </div>

  </div>
</section>

<section id="projects">
  <div class="section-title">
    <h2 data-en="Our <span>Projects</span>" data-ar="مشاريعنا <span>التجريبية</span>">
      Our <span>Projects</span>
    </h2>
    <p data-en="A glimpse into our creative direction"
       data-ar="نظرة على أفكارنا الإبداعية">
      A glimpse into our creative direction
    </p>
  </div>

  <div class="grid">
    <div class="card">
      <span class="project-label" data-en="DEMO PROJECT" data-ar="مشروع تجريبي">DEMO PROJECT</span>
      <h3 data-en="Business Website" data-ar="موقع شركة">Business Website</h3>
      <p data-en="A modern corporate website concept."
         data-ar="تصور لموقع شركة عصري.">A modern corporate website concept.</p>
    </div>

    <div class="card">
      <span class="project-label" data-en="DEMO PROJECT" data-ar="مشروع تجريبي">DEMO PROJECT</span>
      <h3 data-en="Mobile App" data-ar="تطبيق موبايل">Mobile App</h3>
      <p data-en="A creative mobile application concept."
         data-ar="تصور إبداعي لتطبيق موبايل.">A creative mobile application concept.</p>
    </div>

    <div class="card">
      <span class="project-label" data-en="DEMO PROJECT" data-ar="مشروع تجريبي">DEMO PROJECT</span>
      <h3 data-en="Digital Platform" data-ar="منصة رقمية">Digital Platform</h3>
      <p data-en="A modern digital platform concept."
         data-ar="تصور لمنصة رقمية حديثة.">A modern digital platform concept.</p>
    </div>
  </div>
</section>

<section class="vision">
  <div class="section-title">
    <h2 data-en="Our <span>Vision</span>" data-ar="رؤيتنا <span>للمستقبل</span>">
      Our <span>Vision</span>
    </h2>
  </div>

  <p data-en="To build meaningful digital experiences and make technology accessible through creativity and innovation."
     data-ar="أن نصنع تجارب رقمية مؤثرة ونجعل التكنولوجيا أكثر سهولة من خلال الإبداع والابتكار.">
    To build meaningful digital experiences and make technology accessible through creativity and innovation.
  </p>
</section>

<section id="contact">
  <div class="section-title">
    <h2 data-en="Contact <span>Us</span>" data-ar="تواصل <span>معنا</span>">
      Contact <span>Us</span>
    </h2>
    <p data-en="Let's build something great together."
       data-ar="دعنا نبني شيئاً مميزاً معاً.">
      Let's build something great together.
    </p>
  </div>

  <div class="contact-wrap">
    <form id="contact-form">
      <input type="text" required
        data-en-placeholder="Your Name"
        data-ar-placeholder="اسمك"
        placeholder="Your Name">

      <input type="email" required
        data-en-placeholder="Your Email"
        data-ar-placeholder="بريدك الإلكتروني"
        placeholder="Your Email">

      <textarea required
        data-en-placeholder="Tell us about your project..."
        data-ar-placeholder="أخبرنا عن مشروعك..."
        placeholder="Tell us about your project..."></textarea>

      <button type="submit" class="btn"
        data-en="Send Message" data-ar="إرسال الرسالة">
        Send Message
      </button>

      <p id="form-status" aria-live="polite"></p>
    </form>
  </div>
</section>

<footer>
  <div class="logo">NOVIX.</div>
  <p data-en="Building the Digital Future."
     data-ar="نبني المستقبل الرقمي.">
    Building the Digital Future.
  </p>
  <p>© 2026 NOVIX. All Rights Reserved.</p>
</footer>

<script>
let currentLanguage = "en";

function toggleLanguage() {
  currentLanguage = currentLanguage === "en" ? "ar" : "en";

  document.documentElement.lang = currentLanguage;
  document.documentElement.dir =
    currentLanguage === "ar" ? "rtl" : "ltr";

  document.querySelectorAll("[data-en]").forEach(element => {
    element.innerHTML = element.dataset[currentLanguage];
  });

  document.querySelectorAll("[data-en-placeholder]").forEach(element => {
    element.placeholder =
      element.dataset[currentLanguage === "ar"
        ? "arPlaceholder"
        : "enPlaceholder"];
  });

  document.querySelector(".lang").textContent =
    currentLanguage === "en" ? "العربية" : "English";
}

document.getElementById("contact-form").addEventListener("submit", function(e) {
  e.preventDefault();

  document.getElementById("form-status").textContent =
    currentLanguage === "en"
    ? "Demo form only. Connect an email service to receive messages."
    : "هذا نموذج تجريبي فقط. يجب ربط خدمة بريد إلكتروني لاستقبال الرسائل.";

  this.reset();
});
</script>

</body>
</html>
# https-novix-company.github.io
https://novix-company.github.io
