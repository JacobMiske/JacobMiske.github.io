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







<h2>JavaScript Can Validate Input</h2>
<p>Please input a number between 1 and 10:</p>
<input id="numb">
<button type="button" onclick="myFunction()">Submit</button>
<p id="demo"></p>
<script>
function myFunction() {
  let x, text;
  x = document.getElementById("numb").value;
  if (isNaN(x) || x < 1 || x > 10) {
    text = "Input not valid";
  } else {
    text = "Input OK";
  }
  document.getElementById("demo").innerHTML = text;
}
</script>
