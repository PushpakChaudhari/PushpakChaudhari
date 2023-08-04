<h1 align="center" style="color: #F74533; font-size: 36px; margin-bottom: 20px; font-weight: bold;">
  Welcome to Pushpak's profile!
  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28">
</h1>

<p align="center" class="typing-svg" style="font-family: 'Fira Code', monospace; font-size: 23px; color: #F74533; background-color: #EFFF4F00; padding: 10px; border-radius: 5px; display: inline-block;">
  A Self Taught Developer
</p>

<!-- Rest of your content remains unchanged -->

<!-- Add custom CSS for styling -->
<style>
  /* Add CSS styles for different sections here */
  /* Header style */
  h1 {
    /* Your styles */
  }

  /* Favorite tools section style */
  h1.favorite-tools {
    /* Your styles */
  }

  /* Stats section style */
  h2.stats {
    /* Your styles */
  }

  /* Footer style */
  .footer {
    /* Your styles */
  }
</style>

<!-- Add custom JavaScript for interactivity -->
<script>
  // Typing effect for the "Learning" part in the "Typing SVG" section
  document.addEventListener("DOMContentLoaded", () => {
    const textElement = document.querySelector(".typing-svg");
    const words = [
      "A Self Taught Developer",
      "Learning Web App Development",
      "Backend Developer",
      "A Quick Learner",
    ];
    let wordIndex = 0;
    let charIndex = 0;

    function type() {
      if (charIndex < words[wordIndex].length) {
        textElement.textContent += words[wordIndex].charAt(charIndex);
        charIndex++;
        setTimeout(type, 100);
      } else {
        charIndex = 0;
        wordIndex++;
        if (wordIndex === words.length) {
          wordIndex = 0;
        }
        setTimeout(() => {
          textElement.textContent = words[wordIndex].charAt(0);
          type();
        }, 2000);
      }
    }

    type();
  });
</script>
