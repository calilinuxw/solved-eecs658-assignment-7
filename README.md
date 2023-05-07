Download Link: https://assignmentchef.com/product/solved-eecs658-assignment-7
<br>
Deliverables:

<ol>

 <li>Copy of Rubric7.docx with your name and ID filled out (do not submit a PDF)</li>

 <li>Python source code.</li>

 <li>Screen print showing the successful execution of your Python code. (Copy and paste the output from the Python console screen to a Word document and PDF it).</li>

 <li>Answer to Part 1, Question 1.</li>

 <li>Answer to Part 2, Question 2.</li>

</ol>




Assignment:

<ul>

 <li>For both parts, we are going to use a modified version of the Gridtask World described in the lectures. The only difference is that the grid is a 5-by-5 grid instead of a 4-by-4 grid:</li>

</ul>

<table width="192">

 <tbody>

  <tr>

   <td width="38"> </td>

   <td width="38">1</td>

   <td width="38">2</td>

   <td width="38">3</td>

   <td width="38">4</td>

  </tr>

  <tr>

   <td width="38">5</td>

   <td width="38">6</td>

   <td width="38">7</td>

   <td width="38">8</td>

   <td width="38">9</td>

  </tr>

  <tr>

   <td width="38">10</td>

   <td width="38">11</td>

   <td width="38">12</td>

   <td width="38">13</td>

   <td width="38">14</td>

  </tr>

  <tr>

   <td width="38">15</td>

   <td width="38">16</td>

   <td width="38">17</td>

   <td width="38">18</td>

   <td width="38">19</td>

  </tr>

  <tr>

   <td width="38">20</td>

   <td width="38">21</td>

   <td width="38">22</td>

   <td width="38">23</td>

   <td width="38"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Everything else is the same:

  <ul>

   <li>The goal of the Gridworld Task is for a robot, starting at any square in the grid, to move through the grid and end up in a termination state (grey squares) which ends the game. o Each grid square is a state (s).  o The actions (a) that can be taken are up, down, left, or right.</li>

   <li>The rewards (r) are:

    <ul>

     <li>-1 on all transitions</li>

     <li>0 terminal state</li>

     <li>-1 when it hits a wall (no transition, but still a reward) o Assume:</li>

     <li>p(r<sub>t+1</sub>|s<sub>t</sub>,a<sub>t</sub>) = 0.25</li>

     <li>p(s<sub>t+1</sub>|s<sub>t</sub>,a<sub>t</sub>) = 0.25</li>

     <li>γ = 1</li>

    </ul></li>

  </ul></li>

</ul>




Part 1: RL Policy Iteration Algorithm

<ul>

 <li>Write a Python program that uses the RL Policy Iteration algorithm to develop an optimal policy (π*).</li>

 <li>The program should display the optimal policy (π*) as a Python array similar to this:</li>

</ul>

[[0.0 -0.9 -0.8 -0.7 -0.6]

[-0.9 -0.9 -0.8 -0.7 -0.6]

[-0.9 -0.9 -0.8 -0.7 -0.6]

[-0.9 -0.9 -0.8 -0.7 -0.6]

[-0.9 -0.9 -0.8 -0.7 0.0]]

<ul>

 <li>The policy the robot follows, no matter what square it is in, is to go to the square next to it with the highest value.</li>

 <li>If it follows this policy, it will end up in one of the termination squares in the least amount of moves.</li>

 <li>Note: The values in this array are NOT the ones you will get.</li>

 <li>The program should print out the policy array with the iteration number for iteration 0 (the initial values), iteration 1, iteration 10, and the final iteration.</li>

 <li>Determine a method for deciding when the Policy Iteration algorithm has converged.</li>

 <li>Question 1: Explain the convergence method and why you picked it. There is no wrong answer. You will get credit for any method you pick as long as it converges and you provide a reasonable explanation of why you picked it.</li>

 <li>For help, consult: <a href="https://towardsdatascience.com/reinforcement-learning-rl-101-with-python-e1aa0d37d43b">https://towardsdatascience.com/reinforcement-learning-rl-101</a><a href="https://towardsdatascience.com/reinforcement-learning-rl-101-with-python-e1aa0d37d43b">with-python-e1aa0d37d43b</a></li>

</ul>




Part 2: RL Value Iteration Algorithm

<ul>

 <li>Write a Python program that uses the RL Value Iteration algorithm to develop an optimal policy (π*).</li>

 <li>The program should display the optimal policy (π*) as a Python array similar to this:</li>

</ul>

[[ 0 -1 -2 -3 -4]

[-5 -6 -7 -8 -9]

[-5 -6 -7 -8 -9]

[-5 -6 -7 -8 -9]

[-5 -6 -7 -8 0]]

<ul>

 <li>The policy the robot follows, no matter what square it is in, is to go to the square next to it with the highest value.</li>

 <li>If it follows this policy, it will end up in one of the termination squares in the least amount of moves.</li>

 <li>Note: The values in this array are NOT the ones you will get.</li>

 <li>The program should print out the policy array with the iteration number for iteration 0 (the initial values), iteration 1, iteration 2, and the final iteration.</li>

 <li>Determine a method for deciding when the Value Iteration algorithm has converged.</li>

 <li>Question 2: Explain the convergence method and why you picked it. There is no wrong answer. You will get credit for any method you pick as long as it converges and you provide a reasonable explanation of why you picked it.</li>

</ul>




Remember:

<ul>

 <li>Your Programming Assignments are individual-effort.</li>

 <li>You can brainstorm with other students and help them work through problems in their programs, but everyone should have their own unique assignment programs.</li>

</ul>