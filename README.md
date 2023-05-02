Download Link: https://assignmentchef.com/product/solved-cpe459-exercise3-traffic-lights
<br>
Design and implement a two-traffic light intersection control system. The system should use one PLC to control two red-green-yellow traffic lights.  One traffic light should control north-south traffic and the other east-west.

Build the circuit

Build a circuit with 3 LED: 1 for each light in the north-south stack.  Control the LEDs with your ladder logic.  There are only 4 digital outputs on Arduino Uno so we can only have one physical red-yellow-green traffic light stack.  The second light stack will be present in ladder logic and the HMI only.

<h1>3         Build the Ladder Logic</h1>

<ul>

 <li>Each light should use timers to cycle the lights through red-green-yellow.  The lights should cycle with green on for 10 seconds, yellow on for 5 seconds, and then red on.  The north-south red light should be on when the east-west green or yellow lights are on. The east-west red light should be on when the north-south green or yellow lights are on. There is no timer needed for the red lights. The red lights can simply use OR logic.</li>

</ul>

<ul>

 <li>Add safety logic in the ladder to ensure the following properties.

  <ol>

   <li>To be green, the red LED in the other stack must be on and the green and yellow LED in the other stack must be off.</li>

   <li>To be yellow, the red LED in the other stack must be on and the green and yellow LED in the other stack must be off.</li>

  </ol></li>

</ul>

<h1>4         Build the HMI</h1>

<ul>

 <li>The HMI should display each LED’s state.</li>

 <li>The HMI should display a counter next to each light in the stack that counts down to transitions.</li>

 <li>In the HMI add a background image that shows the intersection.</li>

</ul>




<h1>5         Post Exercise Report</h1>

Answer the following questions.

<ol>

 <li>Submit a short video of your working traffic light.</li>

</ol>


