# ActionScript ArrayIndexOutOfBoundsException

This repository demonstrates a common ActionScript error: attempting to access an array element beyond its bounds. The bug.as file contains the erroneous code, while bugSolution.as provides the corrected version.

## Description

The bug arises from trying to access `myArray[myArray.length]`.  Array indices in ActionScript (and most other languages) are zero-based.  Therefore, the last valid index is `myArray.length - 1`. Accessing `myArray.length` results in an `ArrayIndexOutOfBoundsException`.

## Solution

The solution involves adjusting the array access to use the correct index: `myArray[myArray.length - 1]` (if you intend to access the last element) or adding appropriate checks to prevent out-of-bounds access.