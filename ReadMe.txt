QUESTION 1:
Given two sets of elements, find the sum of all distinct elements from the set. 
In other words, find the sum of all elements which are present in either of the given set.
Initialize variable sum = 0
 
Code written in Pseudocode

//Begin of for loop through set 1
 for each element in set1 do
    if element is not in set2 and element is not in distinct_elements then
        add element to distinct_elements
        add element to sum
    end if
 end for

//Begin of for loop through set 2	
 for each element in set2 do
    if element is not in set1 and element is not in distinct_elements then
        add element to distinct_elements
        add element to sum
    end if
 end for

 return sum 

                      OR

Code written in javascript

 // function sumOfDistinctElements(set1, set2) { // let distinctElements = [];

// for(let i=0; i<set1.length; i++) { // if(!distinctElements.includes(set1[i])) { // distinctElements.push(set1[i]); // } // }

// for(let i=0; i<set2.length; i++) { // if(!distinctElements.includes(set2[i])) { // distinctElements.push(set2[i]); // } // }

// let sum = 0; // for(let i=0; i<distinctElements.length; i++) { // sum += distinctElements[i]; // }

// return sum; // }

// //Example usage // let set1 = [3, 1, 7, 9]; // let set2 = [2, 4, 1, 9, 3]; // console.log(sumOfDistinctElements(set1, set2)); // Output: 13



QUESTION 2:
You are asked to write an algorithm that fulfill the following: 

Name: Dot product
Description:

1.Write a procedure, called dot_product which calculates in the variable ps, 
 the dot(scalar) product of v1 and v2 (v1 and v2 are vectors of IR)

2.Write an algorithm which determines, for n pairs of given vectors, whether two vectors of given IR are orthogonal, 
 by calling the procedure defined in the previous question. The dot product of two orthogonal vectors is zero.

3.Modify the previous algorithm if you use a dot_product function instead of a procedure.

Code written in pseudocode

Procedure dot_product(v1, v2):
a. Initialize ps = 0.
b. For i = 0 to n-1:
i. ps += v1[i] * v2[i]
c. Return ps

Algorithm check_orthogonality(n, v):
a. For i = 0 to n-1:
i. For j = i+1 to n-1:
1. ps = dot_product(v[i], v[j])
2. If ps == 0, print "Vector i and vector j are orthogonal"
3. Else, print "Vector i and vector j are not orthogonal"

Function dotProduct(v1, v2):
a. Initialize ps = 0.
b. For i = 0 to n-1:
i. ps += v1[i] * v2[i]
c. Return ps

Function dotProduct(v1, v2):
a. Initialize ps = 0.
b. For i = 0 to n-1:
i. ps += v1[i] * v2[i]
c. Return ps

Code written in JavaScript

For i from 1 to n do: ps = dot_product(v1[i], v2[i]) If ps equals 0: Print "Vectors", v1[i], "and", v2[i], "are orthogonal" Else: Print "Vectors", v1[i], "and", v2[i], "are not orthogonal"

Function dot_product(v1, v2): Initialize ps to 0 For i from 1 to length of v1 do: ps = ps + v1[i] * v2[i] Return ps

Algorithm to determine orthogonality using function dot_product: Input: n pairs of vectors v1 and v2 of IR Output: whether each pair of vectors is orthogonal

For i from 1 to n do: ps = dot_product(v1[i], v2[i]) If ps equals 0: Print "Vectors", v1[i], "and", v2[i], "are orthogonal" Else: Print "Vectors", v1[i], "and", v2[i], "are not orthogonal"

// function sumOfDistinctElements(set1, set2) { // const distinctElements = []; // const unionSet = [...set1, ...set2];

// for (let i = 0; i < unionSet.length; i++) { // const element = unionSet[i]; // if (!distinctElements.includes(element)) { // distinctElements.push(element); // } // }

// const sum = distinctElements.reduce((total, current) => total + current, 0); // return sum; // }

// // Example usage: // const set1 = [3, 1, 7, 9]; // const set2 = [2, 4, 1, 9, 3]; // console.log(sumOfDistinctElements(set1, set2)); // Output: 13














