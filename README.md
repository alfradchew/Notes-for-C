### NOTES ABOUT C

CONTENTS OF THIS FILE
---------------------
 * [String Comparison](#String-Comparison)
 * [Null Value](#Null-Value)
 
 
 ### String Comparison
----------------------
Single-quotes mean "character literal" not "string literal" in C. Double-quotes mean "character literal" in C.

"string1" == "string2" does not compare the value of the strings, but rather their base addresses, i.e. pointers to characters. Use strcmp() to compare strings instead.

Reference: https://stackoverflow.com/questions/1598425/how-do-i-check-if-a-value-matches-a-string/


 ### Null Value
----------------------
The character '\0' is either a zero character or it indicates the end of a string.

Reference: https://stackoverflow.com/questions/14461695/what-does-0-stand-for/14461711

Initialise an empty character of length n instead of empty string. Example if i want to initialise an empty string of size 5, type "char hello[5];" instead of "string hello[5]". There will be issue later if you want to change the value of a partiular character inside the string if you use "string hello[5]".


