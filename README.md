# MongoDB $inc Operator Error

This repository demonstrates an uncommon error related to the `$inc` operator in MongoDB update queries. The error arises when attempting to increment a field using a string value instead of a numeric value.

## Bug Description

The `$inc` operator is designed to increment a numeric field in a MongoDB document. Passing a string value to `$inc` results in unexpected behavior, potentially leading to data corruption or incorrect updates.

## Bug Reproduction

The `bug.js` file contains the erroneous code. Running this code against a MongoDB collection will not increment the field as intended.

## Bug Solution

The `bugSolution.js` file provides the corrected code.  The solution involves ensuring that the value provided to `$inc` is a numeric value. 
