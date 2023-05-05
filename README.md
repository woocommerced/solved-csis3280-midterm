Download Link: https://assignmentchef.com/product/solved-csis3280-midterm
<br>
You are asked to write a PHP program that generates a piece of code randomly, containing a random array and a random foreach loop. The code evaluates the generated code and displays to the user what the result would be if the piece of code executed.




<h2>Requirements</h2>

<ol>

 <li>You must write your program as requested below. It must conform with the following requirements. If something has not been explicitly requested, you can choose your own style or the most efficient choice.</li>

 <li>The name of the array is always fixed, and it is <strong>values</strong>. Therefore, all randomly generated arrays have the same name.</li>

 <li>The number of elements of the array is random. It can at least 1 element to maximum 10 elements. The values are generated randomly of integers from -10 to 10.</li>

 <li>After generating the array, there is always the statement <strong>result = 0 ;</strong> Then the foreach loop is generated. There is always <strong>foreach (values as v)</strong>.</li>

 <li>Inside the foreach loop, there is an if-else statement.</li>

 <li>The condition (Boolean expression) in front of if-keyword is generated randomly. A comparison operator (&gt;, &lt;, &gt;=, &lt;=, ==, !=) is picked randomly among the list and the integer value after the comparison operator is generated randomly. This integer value can be from -8 to 8.</li>

 <li>In the body of if-statement is always <strong>break;</strong></li>

 <li>The else-statement has always 1 expression using either += or -= operators. This operator must be picked randomly.</li>

 <li>After the array and foreach loop definition, your program must display what the value of result would be if the piece of code executed.</li>

 <li>define a function called <strong>evaluate_foreach_loop. </strong>This function has 4 input parameters:

  <ol>

   <li>The array of randomly generated values (9,-3,-6,6,3,-2 in the example top-middle)</li>

   <li>a string indicating the comparison operator in front of if-keyword (in the first example above is</li>

  </ol></li>

</ol>

‘&lt;‘)

<ul>

 <li>the value after the comparison operator. ( -5 in the first example on top-left)</li>

</ul>

<ol>

 <li>the compound operator in the expression of the else-statement (‘-=’ in the first example, and ‘+=’ in the second example above.</li>

</ol>

<ol>

 <li>The function returns 1 value: the evaluated value of result if the code executed.</li>

 <li>You may use two loops in this function. First loop to start from the beginning of the array to the point in the array where an element violates the condition of the Boolean expression in front of if-keyword. For example, in the middle example above 9 violates the condition (v &gt; 5), and in the third example above, none of the elements (10 and -9) does not violate (v==3).</li>

</ol>

The second loop calculates either += or -= on the elements of the array from the beginning of the array to the element that you found in the first loop.

<ol>

 <li>You must also define a function<strong> evaluated_bool_expression</strong>. This function is used in the first loop to evaluated if the condition in front of if-keyword is true or false

  <ol>

   <li>This function has 3 inputs and returns 1 Boolean value (true or false)</li>

   <li>The 3 input parameters are: the value of an element of the array, comparison operator, and the integer value after the comparison operator. iii. You must use a switch-case to find what the comparison operator is and if the boolean expression is evaluated to true or false.</li>

  </ol></li>

 <li>For formatting you can use <strong>&lt;br /&gt;</strong> for line break and <strong>&amp;nbsp;</strong> for spaces. For example, define consts like the following and use them in your strings where you want to create a new line or :

  <ul>

   <li>const white_4space = “&amp;nbsp;&amp;nbsp;&amp;nbsp;&amp;nbsp;”;</li>

   <li>const new_line = “&lt;br /&gt;”;</li>

  </ul></li>

</ol>