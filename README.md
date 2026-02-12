# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

A truth table was used to create a KMap. Two equations, a Sum of Products and Product of Sums were extracted from the KMap and implemented into the code. The code was then able to showcase how a truth table can be implemended into Vivado, and the program itself will simplify the final function. 

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
The reason that the groups of 1's or 0's that can be selected in a KMap to go across the edges is because the KMap is a cylinder that folds horziontally and vertically. This allows for the 1's and 0's to connect even if they may not be touching right next to each other. To help visualize this, the top and bottom rows touch and the first and last columns touch as well allowing for the KMap to go across the edges. 

### Why are the names Sum of Products and Products of Sums?
The reason why the name is the Sum of Products is because, in this case we are looking at the minterms which are the 1's in the KMap. When looking at minterms, we must use AND gates and then add all of the AND gates together by connecting them with OR gates. AND is multiplication and OR is addition which results in the Sum of Products. In Products of Sum, we are instructed to look at the maxterms which are the 0's in the KMap. To connect these 0's we use OR gates and then connect all of the OR gates at the end using AND gates. OR gates are addition and AND gates are multiplication, which result in a Product of Sums. 

### Open the test.v file – how are we able to check that the signals match using XOR?
The way that we are able to check that the signals match using XOR is by checking to see either of the values are different.
-if A XOR B does not equal 0 an error will result (Minterms)
-if A and C do not equal 0, meaning they are not equal to each other an error will result (Maxterm)
