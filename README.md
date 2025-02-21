# MongoDB $inc operator error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numeric field by a specified value. However, if the value provided is not a number, the operation will fail or produce unexpected results.

## Bug
The original code incorrectly uses a string ('1') instead of a number (1) as the increment value. This results in the field not being incremented correctly, and possibly an error depending on MongoDB version.

## Solution
The solution involves changing the string increment value to a number.
