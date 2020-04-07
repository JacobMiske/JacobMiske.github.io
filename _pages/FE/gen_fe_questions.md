---
layout: page
title: FE General Questions
permalink: /general_fe_questions/
---

I have decided to break this down by domain.
##  From Lindeberge's FE Review Manual

### Units 
Problem 1.1

What is a metric ton?

- A: 200 kg
- B: 1000 kg
- C: 2000 kg
- D: 2 kN

Solution: B, a metric ton (tonne) is 1000kg

Problem 1.2 

What is a kip?

- A: 1000 in-lbf (torque)
- B: 1000 lbm (mass)
- C: 1000 lbf (force)
- D: 1000 psi (pressure)

Solution: C, kip is a measure of force

Problem 1.3

What is a the SI unit with units $$ kg m^2/s^2 $$

- A: joule
- B: pascal
- C: tesla
- D: watt

Solution: A, KE is measured as 1/2 m v^2, same units


### Algebra and Linear Algebra
Problem 5.1

Which of the following is equal to $$ log_8 50 $$?

- A: 0
- B: 0.53
- C: 0.79
- D: 1.88

Solution: D, $$ log_8 50 = \dfrac{log 50}{log 8} $$







<h2>JavaScript Can Validate Input</h2>
Which of the following is equal to $$ log_8 50 $$?

- A: 0
- B: 0.53
- C: 0.79
- D: 1.88

<p>The answer is D.</p>
<input id="numb">
<button type="button" onclick="resultFunction(inputId = 'numb', correctAns='D')">Submit</button>
<p id="demo"></p>
<script>
function resultFunction(inputId, correctAns) {
  let x, text;
  x = document.getElementById(inputId).value;
  if (x === correctAns) {
    text = "Correct";
  } else {
    text = "Incorrect";
  }
  document.getElementById("demo").innerHTML = text;
}
</script>
