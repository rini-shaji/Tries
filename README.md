# Tries
Programs related to Tries data structure
Problem 1: 
Ref: https://www.hackerrank.com/challenges/ctci-contacts
Problem Description from kackerrank:

We're going to make our own Contacts application! The application must perform two types of operations:

add name, where  is a string denoting a contact name. This must store  as a new contact in the application.
find partial, where  is a string denoting a partial name to search the application for. It must count the number of contacts starting with  and print the count on a new line.
Given  sequential add and find operations, perform each operation in order.

Input Format

The first line contains a single integer, , denoting the number of operations to perform. 
Each line  of the  subsequent lines contains an operation in one of the two forms defined above.

Constraints

It is guaranteed that  and  contain lowercase English letters only.
The input doesn't have any duplicate  for the  operation.
Output Format

For each find partial operation, print the number of contact names starting with on a new line.

Sample Input

4
add hack
add hackerrank
find hac
find hak
Sample Output

2
0
Explanation

We perform the following sequence of operations:

Add a contact named hack.
Add a contact named hackerrank.
Find and print the number of contact names beginning with hac. There are currently two contact names in the application and both of them start with hac, so we print  on a new line.
Find and print the number of contact names beginning with hak. There are currently two contact names in the application but neither of them start with hak, so we print  on a new line.
---------------------------------------------------------------------------------------------------------------------------------------
Problem 2:
Ref: https://www.hackerrank.com/challenges/no-prefix-set
Given N strings. Each string contains only lowercase letters from a-j (both inclusive). The set of N strings is said to be GOOD SET if no string is prefix of another string else, it is BAD SET. (If two strings are identical, they are considered prefixes of each other.)

For example, aab, abcde, aabcd is BAD SET because aab is prefix of aabcd.

Print GOOD SET if it satisfies the problem requirement. 
Else, print BAD SET and the first string for which the condition fails.

Input Format 
First line contains N, the number of strings in the set. 
Then next N lines follow, where ith  line contains ith string.

Constraints 
 1<=N<=10^5
 1<=Length of the string<=60 

Output Format 
Output GOOD SET if the set is valid. 
Else, output BAD SET followed by the first string for which the condition fails.

Sample Input00

7
aab
defgab
abcde
aabcde
cedaaa
bbbbbbbbbb
jabjjjad

Sample Output00

BAD SET
aabcde
Sample Input01

4
aab
aac
aacghgh
aabghgh
Sample Output01

BAD SET
aacghgh
Explanation 
aab is prefix of aabcde. So set is BAD SET and it fails at string aabcde.
