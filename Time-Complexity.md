# Working with time complexity
In this reading, you will explore a worked example of a piece of code written in Python, along with how you would evaluate it using Big-O notation. 

## Introduction
When evaluating coding solutions, Big-O notation is used. So, Big-O notation is the kilowatt hour of code evaluation. It can be applied to measuring how much time a piece of code will take or how much space it will use in memory. Not all processors will run at the same speed, so instead of timing an application, you count the number of instructions an application initiates. 

## Which measurement reflects the quickest possible execution of some code?
- O(1)
- O(n)
- O(log n)
- O(n^2)
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/IGySTDFdRFCkwd9ZdoQTnw_382da9f238024333aca779375c0e5ce1_Picture-1-1-.png?expiry=1703548800000&hmac=pCT6OvT8i34aOlDZtSMQ8Jw0e-8JSr_ToinPOxwpl4M"/>

## Worst case, best case and average case 
Of course, it is not always possible to tell how long an approach will take. When looking at the initial loop example, there was a search performed for an element that was absent. You can say that to search a loop takes O(n) times but this might not always be the case. 
Consider that the item being searched for is the first in the array. Then the return will be pretty good in O(1) time! In the example provided every item must be searched before determining that it was absent: O(n) time. The middle case would be that it is found around the middle of the loop O(n/2). When evaluating an approach, three definitions are used: best case, worst case and average case. 

## Conclusion 
This reading introduced the notion of time in relation to complexity and you explored a worked example of a piece of code written in Python. You also investigated how you would evaluate it using Big-O notation. 
A good question to ask yourself before you start is, "how many computations does my solution employ and is there a better way?" Now that you know how to use a metric to evaluate the solution to a given problem, you can start thinking of its efficacy concerning time complexity. 
