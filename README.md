# React Native AsyncStorage Complex Data Handling Error
This repository demonstrates a common error in React Native when working with AsyncStorage and complex data structures (objects and arrays).  The incorrect approach attempts to store non-string data, which AsyncStorage does not support directly. The correct approach uses `JSON.stringify` for storage and `JSON.parse` for retrieval. 

## Bug Description:
Attempting to directly store objects or arrays in AsyncStorage leads to unpredictable behavior or data loss.  AsyncStorage only accepts strings.

## Solution:
Stringify the objects/arrays before storage and parse the retrieved strings back to their original structure.