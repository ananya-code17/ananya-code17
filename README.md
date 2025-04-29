<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Ananya Joshi</title>
  <style>
    .vertical-text {
      display: flex;
      flex-direction: column;
      align-items: center;
      font-size: 2rem;
      font-weight: bold;
      animation: reveal 1s forwards;
      overflow: hidden;
      height: 20px;
    }
    .vertical-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 30px;
    }
    .letter {
      opacity: 0;
      animation: fadeIn 0.5s forwards;
    }
    @keyframes fadeIn {
      to {
        opacity: 1;
      }
    }
  </style>
</head>
<body>

<div align="center" style="display: flex; align-items: center; justify-content: center; flex-direction: column;">
  <div class="vertical-container" id="verticalText"></div>
  
  <h3>I'm a B.Tech CSE 2nd-year student passionate about data science, machine learning, and full-stack development</h3>
  
  <img src="https://user-images.githubusercontent.com/55389276/140866485-8fb1c876-9a8f-4d6a-98dc-08c4981eaf70.gif" alt="Coding" width="300"/>
</div>

<script>
  const text = "Hi 👋, I'm ANANYA JOSHI";
  const container = document.getElementById('verticalText');

  [...text].forEach((char, index) => {
    const span = document.createElement('span');
    span.className = 'letter';
    span.style.animationDelay = `${index * 0.1}s`; // delay each letter
    span.textContent = char;
    container.appendChild(span);
  });
</script>

</body>
</html>
