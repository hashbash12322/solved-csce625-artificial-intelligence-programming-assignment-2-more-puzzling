Download Link: https://assignmentchef.com/product/solved-csce625-artificial-intelligence-programming-assignment-2-more-puzzling
<br>
<h1>Question</h1>

In this assignment you’re asked to write a program to solve a discrete parts assembly puzzle. It involves the placement of blocks on a 7×7 board. Figure 1a shows the board. The pieces that need to be placed on the board each have a unique shape and are shown in Figure 1b. The pieces are composed of unit cells that match the board cells in dimension, and vary in area from 2 to 8 units. The idea is to place the pieces onto the board in such a way that none of them overlap.

<table>

 <tbody>

  <tr>

   <td width="124"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

However, all nine pieces taken together make up 48 units in total. Thus, we see that even if a configuration is found that packs the pieces into the board without overlaps, it must, inevitably, leave one cell uncovered. This is the point of the entries marked {H1<em>,</em>H2<em>,…,</em>H13} as shown in Figure 1a. They denote special cells that we call <em>hole locations</em>. For each such hole location, we obtain a new variant of the puzzle.

Rule: the pieces may be translated and rotated, but not flipped or mirrored. For their final placement to be considered legal, no two pieces should overlap, and they must be entirely within the bounds of the board.

<table width="414">

 <tbody>

  <tr>

   <td width="138">


    <table width="111">

     <tbody>

      <tr>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16">H1</td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

      </tr>

      <tr>

       <td width="16">H2</td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16">H3</td>

       <td width="16">H4</td>

       <td width="16"> </td>

      </tr>

      <tr>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

      </tr>

      <tr>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16">H5</td>

       <td width="16">H6</td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

      </tr>

      <tr>

       <td width="16"> </td>

       <td width="16">H7</td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16">H8</td>

       <td width="16"> </td>

       <td width="16">H9</td>

      </tr>

      <tr>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16">H10</td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

      </tr>

      <tr>

       <td width="16">H11</td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16"> </td>

       <td width="16">H12</td>

       <td width="16">H13</td>

       <td width="16"> </td>

      </tr>

     </tbody>

    </table></td>

   <td width="276"></td>

  </tr>

 </tbody>

</table>

(a) Board with hole positions shown.                  (b) The 9 pieces to placed on the board.

Figure 1: The assembly puzzle for this programming assignment.

1

Figure 2: A solution for H11.

<h1>Approach</h1>

Implement a program that can solve the puzzle.

Task1

Use your program to find a solution for each of the thirteen hole locations. (An example solution one of the holes is shown in Figure 2.)

Task2

For each of the thirteen hole locations, compute an estimate of the total number of distinct solutions there are.

Task3

Are there locations other than {H1<em>,</em>H2<em>,…,</em>H13} where a hole might be placed to give a new puzzle?

Implementation

You may use any programming language you choose.

<h2>Opportunity</h2>

One important question is how to represent the board and pieces. There are multiple options. It’ll be worth collaborating or even sharing code with your peers especially for this first phase of the problem