Download Link: https://assignmentchef.com/product/solved-cpts-540-artificial-intelligence-homework-10
<br>






<ol>

 <li>Consider the table of data below, which contains seven examples of the class value Pass based on the features Party, Sleep and Study. Suppose we want to classify the new instance &lt;Party=yes, Sleep=yes, Study=yes&gt; using the Naïve Bayes learning method. Compute the following. Show your work. Note: use the “add 1 / |values|” method if the original P(feature | class) = 0.</li>

</ol>




<table width="240">

 <tbody>

  <tr>

   <td width="60"><strong>Party </strong></td>

   <td width="60"><strong>Sleep </strong></td>

   <td width="60"><strong>Study </strong></td>

   <td width="60"><strong>Pass </strong></td>

  </tr>

  <tr>

   <td width="60">yes</td>

   <td width="60">yes</td>

   <td width="60">no</td>

   <td width="60">no</td>

  </tr>

  <tr>

   <td width="60">yes</td>

   <td width="60">no</td>

   <td width="60">yes</td>

   <td width="60">no</td>

  </tr>

  <tr>

   <td width="60">yes</td>

   <td width="60">no</td>

   <td width="60">no</td>

   <td width="60">no</td>

  </tr>

  <tr>

   <td width="60">no</td>

   <td width="60">yes</td>

   <td width="60">yes</td>

   <td width="60">yes</td>

  </tr>

  <tr>

   <td width="60">no</td>

   <td width="60">yes</td>

   <td width="60">no</td>

   <td width="60">yes</td>

  </tr>

  <tr>

   <td width="60">no</td>

   <td width="60">no</td>

   <td width="60">yes</td>

   <td width="60">yes</td>

  </tr>

  <tr>

   <td width="60">no</td>

   <td width="60">no</td>

   <td width="60">no</td>

   <td width="60">no</td>

  </tr>

 </tbody>

</table>




<ol>

 <li>Compute the prior probabilities P(Pass=yes) and P(Pass=no).</li>

 <li>Compute P(Party | Pass) for all combinations of Party  {yes, no} and Pass  {yes, no}.</li>

 <li>Compute P(Sleep | Pass) for all combinations of Sleep  {yes, no} and Pass  {yes, no}.</li>

 <li>Compute P(Study | Pass) for all combinations of Study  {yes, no} and Pass  {yes, no}.</li>

 <li>Compute P(Pass=yes | Party=yes, Sleep=yes, Study=yes) and P(Pass=no | Party=yes, Sleep=yes, Study=yes).</li>

 <li>Which class would Naïve Bayes choose for the new instance?</li>

</ol>







1

<ol start="2">

 <li>Train a perceptron on the 7 examples from the table in Problem 1 and then use the trained perceptron to classify the new instance. Specifically,

  <ol>

   <li>First, translate the examples (including the Pass class value) according to the mapping: no→ 0, yes → Show a new table of examples using this mapping.</li>

   <li>Train the perceptron below by updating the weights according to the perceptron learning rule (slide 34 of Learning lecture). Assume the initial weights are all equal to 1.0, and the learning rate  = 0.25. Consider each example in the order presented in the table in Problem 1 and show the weight updates for each incorrectly-classified example. Continue until the perceptron correctly classifies all the training examples. Show the final perceptron weights. <em>Hint</em>: The perceptron should correctly classify all 7 examples on the 3<sup>rd</sup> pass through the examples.</li>

   <li>How would the trained perceptron classify the new instance &lt;Party=yes, Sleep=yes, Study=yes&gt;? Show your work.</li>

  </ol></li>

</ol>













<ol start="3">

 <li><em>CptS 540 Students Only</em>: Put the 7 training examples from the table in Problem 1 into an ARFF file suitable for input to WEKA. Follow the procedure below to run the Naive Bayes classifier.

  <ol>

   <li>Download and install WEKA from <a href="https://www.cs.waikato.ac.nz/ml/weka/downloading.html">cs.waikato.ac.nz/ml/weka/downloading.html</a><a href="https://www.cs.waikato.ac.nz/ml/weka/downloading.html">.</a></li>

   <li>Start WEKA and choose the Explorer mode.</li>

   <li>Under the Preprocess tab, choose “Open file…” and load your ARFF file.</li>

   <li>Under the Classify tab, choose the “bayes→NaiveBayes” classifier.</li>

   <li>Under Test options, choose “Use training set”.</li>

   <li>Click Start to run the classifier on your data.</li>

   <li>Include your ARFF file and WEKA’s output in your submission.</li>

  </ol></li>

</ol>







2