Printing neatly
----------------------
CS 6363.006. Algorithms
Fall 2016; Fri, Oct 28
Programming Project
Ver 1.0: Initial description (Oct 28, 10:30 AM).
Group project: one member of each group should submit this project.
Programs can be written in Java, C++, C#, or, Python.
In addition, write or type the algorithm and submit proof of correctness and
running time analysis.
Upload a single zip file on elearning. Written parts are submitted in class.
Submissions can be overwritten by another submission before the deadline.
Due: 10:00 AM, Tue, Nov 29.
Problem 15‐4 (Printing neatly), pages 405‐406.
Write your program to accept its input from a file if the name of the file
is given in the command line, or read its input from the console.
The default value of M is 80. If the command line has a second parameter,
then use it as the value of M.
Sample program fragment to do the above in Java:
public static void main(String[] args) throws FileNotFoundException {
Scanner in;
int M = 80;
if (args.length > 0) {
File inputFile = new File(args[0]);
in = new Scanner(inputFile);
if (args.length > 1) { M = Integer.parseInt(args[1]); }
} else {
in = new Scanner(System.in);
}
etc.
Read the input file and break it into words (separated by spaces or new lines).
Output format:
Your program should print its output to the console.
In the first line of output, print the total penalty (sum of cubes of
the number of spaces added in each line). The second line of output is blank.
Starting from the third line of the output, print the input words,
formatted according to your algorithm. Try to distribute the spaces
within a line to make the output be left and right justified.