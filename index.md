## Welcome to Buffalo Treasures

Project for keeping an oral architectural history of Buffalo

### Guaranty Building

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Making Sound</title>
    <link href="https://fonts.googleapis.com/css?family=Shadows+Into+Light" rel="stylesheet">
    <style>
      #assessment {
        font-family: 'Shadows Into Light', cursive;
        width: 450px;
        border: 1px solid #ccc;
        background-color: #fbfbfb;
        padding: 10px;
        box-shadow: 2px 2px #ccc;
      }

      #assessment h1 {
        margin-top: 0px;
      }

      #assessment button {
        width: 100%;
        height: 30px;
        margin-top: 8px;
        border-radius: 5px;
        background-color: #999;
        color: #333;
        font-size: 1.15em;

      }

    </style>
  </head>
  <body>
      <audio id="sound">
          <source src="Correct Answer.mp3" />
      </audio>
      <audio id="wrongSound">
          <source src="Wrong 02.wav" />
      </audio>
      <div id="assessment">
        <h1>Who played the character of Harry Potter in the movie series?</h1>
        <button id="wrong1">George Clooney</button>
        <button id="correct">Daniel Radcliff</button>
        <button id="wrong2">George Peppard</button>
        <button id="wrong3">George Burns</button>
      </div>
  </body>
  <script>
      const mySound = document.getElementById("sound");
      const correctButton = document.getElementById("correct");
      const wrong1 = document.getElementById("wrong1");
      const wrong2 = document.getElementById("wrong2");
      const wrong3 = document.getElementById("wrong3");

      correctButton.addEventListener("click", function(){
        mySound.play();
      })

      wrong1.addEventListener("click", wrongAnswer);
      wrong2.addEventListener("click", wrongAnswer);
      wrong3.addEventListener("click", wrongAnswer);

      function wrongAnswer(e){
          document.getElementById("wrongSound").play();
      }
  </script>
</html>

### Swan Street Diner

