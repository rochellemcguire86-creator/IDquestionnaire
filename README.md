<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Instructional Design Model Selector</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
<style>
  body {
    font-family: 'Montserrat', sans-serif;
    background: #ffffff;
    color: #333333;
    margin: 0;
    padding: 0;
  }
  .container {
    max-width: 900px;
    margin: 20px auto;
    padding: 30px;
    border: 2px solid #C80000;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    background: #fff;
  }
  h1 {
    color: #C80000;
    text-align: center;
    margin-bottom: 20px;
  }
  .question {
    margin-bottom: 1.5rem;
  }
  .question h3 {
    margin-bottom: 0.5rem;
  }
  label {
    display: block;
    margin-bottom: 0.5rem;
    cursor: pointer;
  }
  input[type="radio"] {
    margin-right: 8px;
  }
  button {
    display: block;
    margin: 30px auto;
    background: #C80000;
    color: #fff;
    border: none;
    padding: 12px 30px;
    font-size: 1rem;
    cursor: pointer;
    border-radius: 5px;
  }
  button:hover {
    background: #a50000;
  }
  .result {
    margin-top: 20px;
    padding: 15px;
    border: 2px solid #C80000;
    border-radius: 8px;
    background: #fff0f0;
    display: none;
    font-weight: bold;
    font-size: 1.1rem;
  }
</style>
</head>
<body>
<div class="container">
  <h1>Instructional Design Model Selector</h1>
  <form id="idForm">

    <!-- Questions 1–17 -->
    <div class="question">
      <h3>1. How clearly defined is your learning goal?</h3>
      <label><input type="radio" name="q1" value="backwards"> Very clear and measurable</label>
      <label><input type="radio" name="q1" value="sam"> Clear, but some aspects need refining</label>
      <label><input type="radio" name="q1" value="sam"> General or exploratory goals</label>
    </div>

    <div class="question">
      <h3>2. What is the primary purpose of your digital learning project?</h3>
      <label><input type="radio" name="q2" value="action"> Change behaviour or performance</label>
      <label><input type="radio" name="q2" value="addie"> Deliver knowledge or awareness</label>
      <label><input type="radio" name="q2" value="sam"> Explore new ideas or innovative approaches</label>
    </div>

    <div class="question">
      <h3>3. How flexible is your project timeline?</h3>
      <label><input type="radio" name="q3" value="sam"> Flexible, can iterate and refine</label>
      <label><input type="radio" name="q3" value="addie"> Fixed, structured process required</label>
      <label><input type="radio" name="q3" value="sam"> Very short, need rapid development</label>
    </div>

    <div class="question">
      <h3>4. How important is stakeholder involvement?</h3>
      <label><input type="radio" name="q4" value="addie"> Essential, multiple approvals</label>
      <label><input type="radio" name="q4" value="kemp"> Moderate, input at key stages</label>
      <label><input type="radio" name="q4" value="sam"> Minimal, independent design</label>
    </div>

    <div class="question">
      <h3>5. How iterative or agile should your design process be?</h3>
      <label><input type="radio" name="q5" value="sam"> Very iterative, test and refine frequently</label>
      <label><input type="radio" name="q5" value="addie"> Some iterations, mostly linear</label>
      <label><input type="radio" name="q5" value="addie"> Not iterative, linear approach</label>
    </div>

    <div class="question">
      <h3>6. How critical is alignment between assessments and objectives?</h3>
      <label><input type="radio" name="q6" value="backwards"> Essential, must match perfectly</label>
      <label><input type="radio" name="q6" value="addie"> Important but flexible</label>
      <label><input type="radio" name="q6" value="sam"> Less important, focus on experimentation</label>
    </div>

    <div class="question">
      <h3>7. What type of learner engagement is needed?</h3>
      <label><input type="radio" name="q7" value="sam"> Interactive, hands-on activities</label>
      <label><input type="radio" name="q7" value="addie"> Standard lecture or eLearning modules</label>
      <label><input type="radio" name="q7" value="kemp"> Mixed methods, tailored to learner</label>
    </div>

    <div class="question">
      <h3>8. How large is your target audience?</h3>
      <label><input type="radio" name="q8" value="addie"> Large, structured rollout needed</label>
      <label><input type="radio" name="q8" value="sam"> Small to medium, flexible approach</label>
      <label><input type="radio" name="q8" value="kemp"> Variable, multiple learner types</label>
    </div>

    <div class="question">
      <h3>9. How complex is the content?</h3>
      <label><input type="radio" name="q9" value="dickcarey"> Highly complex, multiple components</label>
      <label><input type="radio" name="q9" value="addie"> Moderate complexity</label>
      <label><input type="radio" name="q9" value="sam"> Simple concepts, easy to explain</label>
    </div>

    <div class="question">
      <h3>10. How much flexibility do you have with resources?</h3>
      <label><input type="radio" name="q10" value="sam"> High flexibility, can experiment</label>
      <label><input type="radio" name="q10" value="addie"> Moderate, some constraints</label>
      <label><input type="radio" name="q10" value="action"> Limited, focus on impact</label>
    </div>

    <div class="question">
      <h3>11. How important is performance-based assessment?</h3>
      <label><input type="radio" name="q11" value="action"> Very important, assess real actions</label>
      <label><input type="radio" name="q11" value="addie"> Somewhat important</label>
      <label><input type="radio" name="q11" value="backwards"> Important for alignment to outcomes</label>
    </div>

    <div class="question">
      <h3>12. How much does learner diversity affect your design?</h3>
      <label><input type="radio" name="q12" value="kemp"> Critical, tailor to multiple needs</label>
      <label><input type="radio" name="q12" value="sam"> Moderate, some adjustments</label>
      <label><input type="radio" name="q12" value="addie"> Minimal, standard content works</label>
    </div>

    <div class="question">
      <h3>13. How structured should documentation be?</h3>
      <label><input type="radio" name="q13" value="dickcarey"> Very structured and detailed</label>
      <label><input type="radio" name="q13" value="kemp"> Moderate structure, flexible</label>
      <label><input type="radio" name="q13" value="sam"> Minimal documentation needed</label>
    </div>

    <div class="question">
      <h3>14. How critical is instructional sequencing?</h3>
      <label><input type="radio" name="q14" value="dickcarey"> Very critical, sequence matters</label>
      <label><input type="radio" name="
