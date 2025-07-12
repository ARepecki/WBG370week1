# WBG370week1
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Quiz Game</title>
  <link rel="stylesheet" href="styles.css">
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <script src="script.js" defer></script>
</head>

  body {
  font-family: Arial, sans-serif;
  background-color: #fefefe;
  margin: 20px;
}

.container {
  max-width: 600px;
  margin: auto;
  padding: 20px;
  border-radius: 10px;
  background-color: #fff;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1 {
  text-align: center;
  color: #333;
}

.question {
  padding: 15px;
  margin-bottom: 15px;
  border-radius: 8px;
}

.question:nth-child(odd) {
  background-color: #f9f9f9;
}

.question:nth-child(even) {
  background-color: #e0e0e0;
}

label {
  display: block;
  margin: 5px 0;
}

.submit-button {
  display: block;
  width: 100%;
  padding: 10px;
  background-color: #5a9;
  color: white;
  font-weight: bold;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.feedback {
  margin-top: 10px;
  font-weight: bold;
}

<body>
  <div class="container">
    <h1>Trivia Quiz</h1>

    <div class="question" data-correct="a">
      <p>1. What is the capital of France?</p>
      <label><input type="radio" name="q1" value="a"> Paris</label>
      <label><input type="radio" name="q1" value="b"> Rome</label>
      <label><input type="radio" name="q1" value="c"> Madrid</label>
      <div class="feedback"></div>
    </div>

    <div class="question" data-correct="c">
      <p>2. Which planet is known as the Red Planet?</p>
      <label><input type="radio" name="q2" value="a"> Venus</label>
      <label><input type="radio" name="q2" value="b"> Jupiter</label>
      <label><input type="radio" name="q2" value="c"> Mars</label>
      <div class="feedback"></div>
    </div>

    <div class="question" data-correct="b">
      <p>3. Which element has the chemical symbol 'O'?</p>
      <label><input type="radio" name="q3" value="a"> Hydrogen</label>
      <label><input type="radio" name="q3" value="b"> Oxygen</label>
      <label><input type="radio" name="q3" value="c"> Helium</label>
      <div class="feedback"></div>
    </div>

    <button class="submit-button">Submit Answers</button>
  </div>
</body>
</html>
