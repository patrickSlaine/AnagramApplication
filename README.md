# AnagramApplication

This Git Repository Contains Patrick Slaine's Anagram Application
Written using C#

Assumptions Made:
1. The input values can be uppercase and lowercase. For instance, (A & a) when compared should be treated as equal.
2. New Input Data should be added to both cache and file storage, if the input values (inputValueOne & inputValueTwo) are not found within the respective storages. The username is of little reliance to determining if the input data should be stored.


Features Contained Within the Application:
  Validation:
  1. Input Data is Rejected if it contains any characters other than letters
 
  Persistence & Performance:
  1. Newly processed values are added to file & cache storage, only if the respective storages dont already contain the values already.
  2. Newly added values are appended to file storage.
  3. Input values are checks against cache storage before being processed by application logic, if necessary.
  
  Maintainabilty & Supportability 
  1. Test Suites have been added for the following classes (11 Tests Total):
    - JsonAccess.cs
    - AnagramCreator.cs
    - AnagramApplication.cs
  2. Logging to a Text File has been added with Serilog

Additional Features Covered
- Unique values only added to file & cache storage
- Factory Creator Pattern used to create AnagramApplication
- Inputs are validated against special characters
- The Abstract Storage Class can easily be extended to enable loading and storing to different file types, other than JSON.
- Cache Loaded on Start Up
  
