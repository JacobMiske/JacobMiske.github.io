---
layout: page
title: FE General Examples
permalink: /general_fe_examples/
---

I have decided to break this down by domain.
# From Lindeberge's FE Review Manual

### Units 
Example 1.1 

Calculate the weight, in lbf, of a 1.0 lbm object in a gravitational field of 27.5 ft/s^2.

$$
\begin{align*}
    F = \dfrac{m a}{g_c} = \dfrac{(1 \text{lbm})(27.5 \text{ft/s^2})}{(32.2 \dfrac{\text{lbm ft}}{\text{lbf s^2}})}
\end{align*}
$$

Example 1.2 

A rocket with mass of 4000 lbm travels at 27,000 ft/s. What is its kinetic energy in ft-lbf?

$$
\begin{align*}
    E_k = \dfrac{m v^2}{2 g_c} = (1/2)\dfrac{(4000 \text{lbm}) (27000 ft/s)^2}{32.2\dfrac{\text{lbm ft}}{\text{lbf s^2}}}
\end{align*}
$$

Example 1.3 

A 10 kg block hangs from a cable. What is the tension in the cable?

$$
\begin{align*}
    F = mg = (10kg)(9.81m/s^2) = 98.1 N
\end{align*}
$$

Example 1.4

A 10 kg block is raised vertically 3m. What is the change in potential energy?

$$
\begin{align*}
    \Delta E_p = mg \Delta h = (10kg)(9.81m/s^2)(3m) = 294 Nm = 294 J
\end{align*}
$$

Example





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
