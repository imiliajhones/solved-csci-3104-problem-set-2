Download Link: https://assignmentchef.com/product/solved-csci-3104-problem-set-2
<br>
<em>Advice 1</em>: For every problem in this class, you must justify your answer: show how you arrived at it and why it is correct. If there are assumptions you need to make along the way, state those clearly.

<em>Advice 2</em>: Purely verbal or purely mathematical reasoning is typically insufficient for full credit. Instead, use mathematics to make your argument more precise and logical, and use language to explain your mathematical reasoning more clearly.

<ol>

 <li>(20 pts total) Solve the following recurrence relations using any of the following methods: unrolling, tail recursion, recurrence tree (include tree diagram), or expansion. Each each case, show your work.

  <ul>

   <li><em>T</em>(<em>n</em>) = <em>T</em>(<em>n </em>− 2) + <em>C n </em>if <em>n &gt; </em>1, and <em>T</em>(<em>n</em>) = <em>C </em>otherwise</li>

   <li><em>T</em>(<em>n</em>) = 3<em>T</em>(<em>n </em>− 1) + 1 if <em>n &gt; </em>1, and <em>T</em>(1) = 3</li>

   <li><em>T</em>(<em>n</em>) = <em>T</em>(<em>n </em>− 1) + 3<em><sup>n </sup></em>if <em>n &gt; </em>1, and <em>T</em>(1) = 3 (d) <em>T</em>(<em>n</em>) = <em>T</em>(<em>n</em><sup>1<em>/</em>4</sup>) + 1 if <em>n &gt; </em>2 , and <em>T</em>(<em>n</em>) = 0 otherwise</li>

  </ul></li>

 <li>(10 pts) Consider the following function:</li>

</ol>

<table width="0">

 <tbody>

  <tr>

   <td width="417"><strong>CSCI 3104</strong><strong>Problem Set 2</strong></td>

   <td width="207"><strong>Profs. Clauset &amp; Grochow</strong><strong>Spring 2018, CU-Boulder</strong></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="95"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

def foo(n) { if (n &gt; 1) {

print( ’’hello’’ ) foo(n/3) foo(n/3)

}}

In terms of the input <em>n</em>, determine how many times is “hello” printed. Write down a recurrence and solve using the Master method.

<ol start="3">

 <li>(30 pts) Professor McGonagall asks you to help her with some arrays that are <em>raludominular</em>. A raludominular array has the property that the subarray <em>A</em>[1<em>..i</em>] has the property that <em>A</em>[<em>j</em>] <em>&gt; A</em>[<em>j </em>+ 1] for 1 ≤ <em>j &lt; i</em>, and the subarray <em>A</em>[<em>.n</em>] has the property that <em>A</em>[<em>j</em>] <em>&lt; A</em>[<em>j </em>+ 1] for <em>i </em>≤ <em>j &lt; n</em>. Using her wand, McGonagall writes the following raludominular array on the board <em>A </em>= [7<em>,</em>6<em>,</em>4<em>,</em>−1<em>,</em>−2<em>,</em>−9<em>,</em>−5<em>,</em>−3<em>,</em>10<em>,</em>13], as an example.

  <ul>

   <li>Write a recursive algorithm that takes asymptotically sub-linear time to find theminimum element of <em>A</em>.</li>

  </ul></li>

</ol>

1

<ul>

 <li>Prove that your algorithm is correct. (Hint: prove that your algorithm’s correctness follows from the correctness of another correct algorithm we already know.)</li>

 <li>Now consider the <em>multi-raludominular </em>generalization, in which the array contains <em>k </em>local minima, i.e., it contains <em>k </em>subarrays, each of which is itself a raludominular array. Let <em>k </em>= 2 and prove that your algorithm can fail on such an input.</li>

 <li>Suppose that <em>k </em>= 2 and we can guarantee that neither local minimum is closer than <em>n/</em>3 positions to the middle of the array, and that the “joining point” of the two singly-raludominular subarrays lays in the middle third of the array. Now write an algorithm that returns the minimum element of <em>A </em>in sublinear time. Prove that your algorithm is correct, give a recurrence relation for its running time, and solve for its asymptotic behavior.</li>

</ul>

<ol start="4">

 <li>(15 pts extra credit)</li>

</ol>

Asymptotic relations like <em>O</em>, Ω, and Θ represent relationships between <em>functions</em>, and these relationships are transitive. That is, if some <em>f</em>(<em>n</em>) = Ω(<em>g</em>(<em>n</em>)), and <em>g</em>(<em>n</em>) = Ω(<em>h</em>(<em>n</em>)), then it is also true that <em>f</em>(<em>n</em>) = Ω(<em>h</em>(<em>n</em>)). This means that we can sort <em>functions </em>by their asymptotic growth.<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>

<table>

 <tbody>

  <tr>

   <td width="95"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

Sort the following <em>functions </em>by order of asymptotic growth such that the final arrangement of functions <em>g</em><sub>1</sub><em>,g</em><sub>2</sub><em>,…,g</em><sub>12 </sub>satisfies the ordering constraint <em>g</em><sub>1 </sub>= Ω(<em>g</em><sub>2</sub>), <em>g</em><sub>2 </sub>= Ω(<em>g</em><sub>3</sub>), <em>…</em>, <em>g</em><sub>11 </sub>= Ω(<em>g</em><sub>12</sub>).

<table width="0">

 <tbody>

  <tr>

   <td width="25"><em>n</em></td>

   <td width="40"><em>n</em>1<em>.</em>5</td>

   <td width="42">8lg<em>n</em></td>

   <td width="48">4lg<sup>∗ </sup><em>n</em></td>

   <td width="30"><em>n</em>!</td>

   <td width="57">(lg<em>n</em>)!</td>

   <td width="47"></td>

   <td width="57"><em>n</em>1<em>/</em>lg<em>n</em></td>

   <td width="52"><em>n</em>lg<em>n</em></td>

   <td width="54">lg(<em>n</em>!)</td>

   <td width="30">e<em>n</em></td>

   <td width="32">42</td>

  </tr>

 </tbody>

</table>

Give the final sorted list and identify which pair(s) functions <em>f</em>(<em>n</em>)<em>,g</em>(<em>n</em>), if any, are in the same equivalence class, i.e., <em>f</em>(<em>n</em>) = Θ(<em>g</em>(<em>n</em>)).

2

<a href="#_ftnref1" name="_ftn1">[1]</a> The notion of sorting is entirely general: so long as you can define a pairwise comparison operator for a set of objects S that is transitive, then you can sort the things in S. For instance, for strings, we use a comparison based on lexical ordering to sort them. Furthermore, we can use any sorting algorithm to sort S, by simply changing the comparison operators <em>&gt;</em>, <em>&lt;</em>, etc. to have a meaning appropriate for S. For instance, using Ω, <em>O</em>, and Θ, you could apply QuickSort or MergeSort to the functions here to obtain the sorted list.