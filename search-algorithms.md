# Time and Space Complexity in Search Algorithms

In this reading, you will explore time and space complexity in both linear and binary searching algorithms. To gain a greater sense of how time and space complexity feature, these two searches are examined noting the time and space used in finding the target element.

## Linear Search

A linear search is the most direct way of retrieving an item. It means that the search starts at the first item and iterates until either the target item is found or there are no more items left in the array to check.

Given a list of numbers, start at index location 0 and compare each item with a target variable. Return when the index location has been determined or the entire list has been checked and there is no instance of the target element.
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/0Fbe9ssqQoyVfEq93uBeeg_d430216c8dd647e990a35276d7f62fe1_Searching-element-15.png?expiry=1704153600000&hmac=UK5lMWLqphySHV2_MgkQQgHUEWqbn0MIqdhvzyDZPas"/>

- **Worst case**: The item is absent from the list. Every possible location in the list size n has to be searched. O(n) time complexity.
- **Average case**: The element is found in the middle. This is considered an outcome of O(n).
- **Best case**: The item is found at the starting index and no further checks are required, so O(1).
- **Space complexity**: No additional space is required to perform the search. Space required will only be as large as the items that have to be stored in the list, space complexity O(n).

## Binary Search

A binary search is performed by first identifying the mid-point on a sorted list, comparing the target element to it and discarding the half that is less than the target element. This halving at the mid-point is repeated until the target element is found or there is no more list to half.

To conduct a binary search, the list must first be sorted.
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/j4xL9v8dSt2T8fbpnjcgCg_e5587341c7834abcb3d738ae1ca6b2e1_Searching-element.png?expiry=1704153600000&hmac=ISUuCxoEzuWJvTbEVuZBKbW54eh_emveORkILRakGs4"/>
First, a middle point is selected. The value at index 3, is 15. Is this greater than or less than the target element? The search space is broken in two and the left is further examined. 
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/bqSlNcJ8THSvwnCU-1RysQ_7587421162904be6a1315847a678d6e1_Searching-element-1.png?expiry=1704153600000&hmac=RgfXKRuhnkFDc2ONWqBmg0mKxlyp2hT0Lb6PmMy17IM"/>
A new central point is selected. This time there are only three slots to check; index location 1 is at the halfway point. 
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/eGJH3t7UTk2g8eoc-D45Rw_48da5bc0ad744045aa55dd580ce9dde1_Searching-element-2.png?expiry=1704153600000&hmac=vhrKK5pAPRQglifxAJN_RnllmST4_bnjJIWECHnfCfM"/>

- **Worst case**: The item is absent from the list. Due to the nature of the approach, overall complexity is O(log N).
- **Average case**: The element is found after several iterations. After a medium number of searches, the complexity is O(log N).
- **Best case**: The item is found at the starting index and no further checks are required, so O(1).
- **Space complexity**: No additional space is required to perform the search. Space required will only be as large as the items to be stored in the list, space complexity O(n).

## Conclusion

In this reading, you explored time and space complexity in both linear and binary searching algorithms. The time and space complexity for linear and binary search has been analyzed. Both approaches are in-place searches; therefore, there is no additional space required, so the space complexity is small. Linear search has shown itself to be more time complex in all instances, other than the correct item being found on the first attempt.

Binary search halves the state space at every iteration, making it far more efficient. However, you should consider factoring the time taken to sort the array in the overall calculations when evaluating the efficacy of selecting this approach for a general application.
