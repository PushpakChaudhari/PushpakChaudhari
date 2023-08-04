<!-- Your existing content goes here -->

<!-- Add custom CSS for styling -->
<style>
  /* Style for the header */
  h1 {
    color: #F74533;
    font-size: 36px;
    margin-bottom: 20px;
    font-weight: bold;
  }

  /* Style for the typing animation */
  p.typing-svg {
    font-family: 'Fira Code', monospace;
    font-size: 23px;
    color: #F74533;
    background-color: #EFFF4F00;
    padding: 10px;
    border-radius: 5px;
    display: inline-block;
  }

  /* Style for the favorite tools section */
  h1.favorite-tools {
    color: #F74533;
    font-size: 28px;
    margin-top: 50px;
    font-weight: bold;
  }

  .tools-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    margin-top: 30px;
  }

  .tool-icon {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    background-color: #F74533;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 30px;
    color: white;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  }

  /* Style for the stats section */
  h2.stats {
    color: #F74533;
    font-size: 28px;
    margin-top: 50px;
    font-weight: bold;
  }

  /* Style for the footer */
  .footer {
    margin-top: 50px;
    text-align: center;
  }

  .footer img {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    margin-bottom: 10px;
  }
</style>

<!-- Add custom JavaScript for interactivity -->
<script>
  // Function to animate the typing effect
  function typeWriter(textElement, words, wait = 3000) {
    let wordIndex = 0;
    let charIndex = 0;
    let isDeleting = false;

    function type() {
      const currentWord = words[wordIndex];
      if (isDeleting) {
        textElement.textContent = currentWord.substring(0, charIndex - 1);
      } else {
        textElement.textContent = currentWord.substring(0, charIndex + 1);
      }

      if (!isDeleting && charIndex === currentWord.length) {
        isDeleting = true;
        wait = 2000;
      } else if (isDeleting && charIndex === 0) {
        isDeleting = false;
        wordIndex++;
        wait = 3000;
      }

      charIndex++;
      if (wordIndex === words.length) {
        wordIndex = 0;
      }
      setTimeout(type, wait);
    }

    type();
  }

  // Call the typing effect function
  document.addEventListener("DOMContentLoaded", () => {
    const textElement = document.querySelector(".typing-svg");
    const words = [
      "A Self Taught Developer",
      "Learning Web App Development",
      "Backend Developer",
      "A Quick Learner",
    ];
    typeWriter(textElement, words);
  });
</script>



<h1 align="center">
  Hi there! I'm Pushpak Chaudhari 👋
</h1>

<p align="center">
  <a href="mailto:pushpakchaudhari383@gmail.com">
    <img src="https://img.shields.io/badge/Contact%20Me-Mail-ff69b4">
  </a>
  <a href="https://www.linkedin.com/in/pushpak-chaudhari-a3941323a/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blueviolet">
  </a>
  <a href="https://github.com/PushpakChaudhari" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Follow-brightgreen">
  </a>
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/73097560/131186779-58ce5c9e-9d2f-4a8c-a186-91e1d900bf1a.png" width="400" alt="Tech Enthusiast">
</p>

<h2 align="center">🚀 About Me 🚀</h2>

- 🎓 Graduated with a BCA degree from Sant Gadge Baba Amravati University.
- 💡 Passionate about technology and its potential to transform businesses and lives.
- 🌱 Always eager to learn new skills and explore emerging technologies.
- 💻 Experienced in building web applications with Java Spring Boot and Angular.
- 🧠 Currently learning more about cloud computing and DevOps practices.

<h2 align="center">💻 Tech Stack 💻</h2>

<div align="center">
    <h3>👨‍💻 Programming Languages</h3>
    <p align="center">
        Java &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; JavaScript &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Python
    </p>

    <h3>🧰 Frameworks and Libraries</h3>
    <p align="center">
        Angular &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Spring Boot &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Bootstrap
    </p>

    <h3>🗄️ Databases and Cloud Hosting</h3>
    <p align="center"> 
        MySQL &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Oracle &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heroku &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AWS
    </p>

    <h3>💻 Software and Tools</h3>
    <p align="center"> 
        Visual Studio &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Eclipse &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Git
    </p>
</div>

<h2 align="center">📊 GitHub Stats 📊</h2>

<p align="center">
    <img src="https://github-readme-stats.vercel.app/api?username=PushpakChaudhari&theme=radical&show_icons=true&count_private=true&hide=prs,issues,contribs" alt="GitHub Stats" />
</p>

<h2 align="center">🔥 Top Languages 🔥</h2>

<p align="center">
    <img src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=PushpakChaudhari&theme=radical&hide_border=true&layout=compact" alt="Top Languages" />
</p>

<h2 align="center">📍 Profile Visitor Count 📍</h2>

<p align="center">   
    <img src="https://profile-counter.glitch.me/PushpakChaudhari/count.svg" alt="Profile Visitor Count" />
</p>
