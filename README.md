Download Link: https://assignmentchef.com/product/solved-geneticalgorithms-assignment2-marketing-budget-allocation-problem
<br>
Marketing can help scale and sustain a business, but it comes with a cost! It is expensive to run paid campaigns, so careful planning is necessary. Given a marketing budget and a set of marketing channels, we would like to allocate the budget to the different marketing channels such that the total profit is maximized.

<strong><em>What you are required to do:</em></strong>

Write a genetic algorithm to solve the marketing budget allocation problem.

<strong><em>What the input looks like: </em></strong>

You’ll be given the marketing budget, the set of marketing channels, the return-oninvestment (ROI) of each channel and a set of constraints (on investing in each channel). For simplicity, we will assume we have only 2 types of investment constraints:

<ul>

 <li>An investment in marketing channel (i) <strong>can’t be less than</strong> some value (in thousands)</li>

 <li>And/or an investment in marketing channel (i) <strong>can’t exceed</strong> some percent of the total budget.</li>

</ul>

These constraints form the lower and upper bounds of investment in each channel.

<strong><em>Example: </em></strong>

<table width="622">

 <tbody>

  <tr>

   <td width="622">Enter the marketing budget (in thousands):100 Enter the number of marketing channels:4Enter the name and ROI (in %) of each channel separated by space: TV advertising 8Google 12Twitter 7Facebook 11Enter the lower (k) and upper bounds (%) of investment in each channel:(enter x if there is no bound)2.7 5820.5 x x 18 10 x Please wait while running the GA… The final marketing budget allocation is:TV advertising -&gt; 2.7kGoogle -&gt; 76.2kTwitter -&gt; 5.6kFacebook -&gt; 15.5k The total profit is 11.457k</td>

  </tr>

 </tbody>

</table>

<strong><em>Notes:</em></strong><em>  </em>

<ul>

 <li>The ROI is given as a percentage.</li>

 <li>In this example, the investment in TV advertising can’t be less than 2.7k and can’t be more than 58% of the total budget. The investment in marketing through Google can’t be less than 20.5k and there is no restriction on the upper bound. The investment in marketing through Twitter can’t exceed 18% of the total budget and there is no restriction on the lower bound. The investment in marketing through Facebook can’t be less than 10k and there is no restriction on the upper bound.</li>

 <li>Assume a single currency is used in the entire problem.</li>

 <li>Your final solution doesn’t have to match the one in this example, but it should produce high profit. You could also display the output in a different format.</li>

</ul>










<strong><em>Important remarks: </em></strong>

<ol>

 <li>The first thing you need to do is to think about how you will encode the solution in your chromosome. Formulate the problem with the objective function and constraints to help you figure out the next steps.</li>

 <li>You should use a <strong>floating-point representation </strong>of the</li>

 <li>The population size and initialization method you use are up to you. You can actually try different population sizes to see how this will affect your results. The maximum number of generations is also up to you.</li>

 <li>Think about how you will handle <strong>infeasible solutions</strong>. Infeasible solutions are solutions that violate the constraints of the problem; therefore, they are not allowed.</li>

 <li>Implement <strong>tournament selection</strong>, <strong>2-point crossover</strong> and <strong>elitist replacement</strong>. Implement both <strong>uniform and non-uniform mutation</strong>.</li>

 <li>Run the algorithm <strong>20 times</strong> with the same input, <strong>write the output to a file</strong> and <strong>print the best solution</strong> obtained from these experiments.</li>

</ol>