# ip_address
#ruby
Program deciding which input was used
You are given N strings that may or may not be an Internet Protocol (IP) address. You need to detect if the text contained in each of the lines represents
IPv4 address
IPv6 address or
Neither of these

IPv4 was the first publicly used Internet Protocol; it used 4-byte addresses and permitted 232 distinct value. The typical format of an IPv4 address is A.B.C.D where A, B, C and D are integers lying between 0 and 255 (both inclusive).
IPv6, with 128 bits, was developed to permit the expansion of the address space.
“The 128 bits of an IPv6 address are represented in 8 groups of 16 bits each. Each group is written as 4 hexadecimal digits and the groups are separated by colons (:). The address
2001:0db8:0000:0000:0000:ff00:0042:8329 is an example of this representation.”

Groups with leading zeros, or which are identically zeroes, may not omit any of those zeroes.
Input Format
An integer N on a separate line, followed by N lines each containing a string that is either an IPv4 address or an IPv6 address, or an arbitrary text which does not correspond to either format. The input is NOT a text file. You must read each line from standard input.
Constraints
N ≤ 50
There will be no extra text or white-space leading or trailing the IP address in a line that has an IP address. The number of characters in each line will not exceed 500.
Output Format
N lines.
The Ith output line should describe what you detected the Ith input line to be, using one of the following strings, with capitalization preserved:
IPv4
IPv6
Neither
For example, in the sample input, the first line after the integer ("This line has junk text") line is neither an IPv4 or IPv6 so the text Neither is printed.

Sample Input
3
This line has junk text
121.18.19.20
2001:0db8:0000:0000:ff00:0042:8329
Sample Output
Neither
IPv4
IPv6



