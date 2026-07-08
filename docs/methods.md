---
title: "Functions"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/methods.html"
last_updated: "7/8/2026"
product_version: "13.0.2.6723"
---

# Functions


To manipulate values in grouping expressions, you can use the following functions:

Functions

| Function | Return Data Type | Description | Example |
| DateAdd | Date | Returns a date value to which a time interval has been added, or from which a time interval has been subtracted.  The function accepts the following arguments:   1. Date and time to which a time interval must be added, in the YYYY-MM-DD format. 2. Time interval that must be added to the initial date and time. The interval can be a positive or negative number. 3. Measurement unit of the time interval ("h" - hour, "d" - day, "m" - month, "y" - year). | Expression DateAdd("2016-10-20", 7, "d")adds 7 days to the specified date, and returns 2016-10-27.  Nested expression SnapshotCreateTime < DateAdd (DateAdd(Today, -2, "d")) returns True if the latest VM snapshot was created earlier than 2 days and 12 hour ago. |
| IndexOf | Numeric (integer) | Returns the position of the first occurrence of a specified value (substring) in a string. Index of the first character in a string is 0.  Returns -1 if the value is not found within the string.  The function accepts the following arguments:   1. String value. 2. Substring value whose index position must be found within the string value. | Expression IndexOf("vdi001\_mrk", "\_") returns 6.  Expression IndexOf("vdi001", "\_") returns -1. |
| Left | Text (string) | Returns a substring that contains a specified number of characters from the left side of a string.  The function accepts the following arguments:   1. String value. 2. Number of characters from the left side of a string to return. | Expression Left("vdi001\_mrk", 6) returns vdi001.  Nested expression Left("vdi001\_replica", IndexOf("vdi002\_replica", "\_")) returns vdi002. |
| Length | Numeric (integer) | Returns the number of characters in a string.  The function accepts a string value as an argument. | Expression Length("123456789") returns 9.  For a VM, expression Length("Name") returns the number of characters in the VM name. |
| Replace | Text (string) | Returns a string in which a specified substring has been replaced with another substring.  The function accepts the following arguments:   1. String value. 2. Substring value that must be replaced. 3. Substring value that must replace the sought substring.   Note: If the there are two or more equal substrings in a string, all substrings will be replaced. | Expression Replace("vdi002 mrk", " ", "\_") changes the vdi002 mrk value to vdi002\_mrk.  For a VM, expression Replace(Name, "\_replica", "") removes the \_replica suffix from the VM name. |
| Right | Text (string) | Returns a substring that contains a specified number of characters from the right side of a string.  The function accepts the following arguments:   1. String value. 2. Number of characters from the right side of a string to return. | Expression Right("vdi003\_mrk", 3) returns mrk.  Nested expression Right("vdi003\_replica", (IndexOf("vdi003\_replica", "\_")) + 1) returns replica. |
| Space | Text (string) | Returns a string that consists of the specified number of spaces.  The function accepts a positive integer as an argument. | Nested expression Replace("vdi004\_mrk", "\_", Space(1)) changes the vdi004\_mrk value to vdi004 mrk. |
| Substring | Text (string) | Retrieves a substring from a specified string. The substring starts at the specified character position (index) and has the specified length. Index of the first character in a string is 0.  The function accepts the following arguments:   1. String value. 2. Start index position of a substring that must be retrieved. 3. Number of characters to retrieve starting with the specified index position. | Expression Substring("vdi005\_mrk", 7, 3) returns mrk. |
| Trim | Text (string) | Returns a string with no leading or trailing spaces.  The function accepts a string value as an argument. | Expression Trim("  vdi006  ") returns vdi006. |
| TrimLeft | Text (string) | Returns a string with no leading spaces.  The function accepts a string value as an argument. | Expression Trim("  vdi007") returns vdi007. |
| TrimRight | Text (string) | Returns a string with no trailing spaces.  The function accepts a string value as an argument. | Expression Trim("vdi008  ") returns vdi008. |
| ToDate | Date | Converts a string containing a valid date representation to the DateTime format.  Note: The function is based on the [DateTime.TryParse](https://msdn.microsoft.com/library/system.datetime.tryparse%28v%3Dvs.110%29.aspx) function and accepts the same input values. | Expression ToDate("2009/03/12") returns 2009-03-12.  Expression ToDate("ToDate(" 2009/03/01") returns 2009-03-01. |
| ToLowerCase | Text (string) | Converts a string to lower case letters.  The function accepts a string value as an argument. | Expression ToLowerCase("LoWeRCaSe") returns lowercase. |
| ToUpperCase | Text (string) | Converts a string to upper case letters.  The function accepts a string value as an argument. | Expression ToUpperCase("uppercase") returns UPPERCASE. |


