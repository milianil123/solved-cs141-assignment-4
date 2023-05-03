Download Link: https://assignmentchef.com/product/solved-cs141-assignment-4
<br>
<h1>Input Validation Methods</h1>

<strong> </strong>

Convert the code you used in Asg. 3 for user input validation into two methods:

int validateInt(String prompt) and  double vlidateDouble(String prompt)

Each of these methods does the following

<ul>

 <li>takes prompt string as a parameter,</li>

 <li>asks user for input using the prompt sting provided,</li>

 <li>validates input, making sure the type of the numeric value provided by the user is correct.</li>

</ul>

The methods handle exceptions as they arise, use exceptions to determine if the type of the number entered was correct. The input prompt is repeated in the loop until the user provides the numeric value of correct type.

<ul>

 <li>returns the integer or double value (according to the name of the method) to the calling code.</li>

</ul>

From now on you can call these methods whenever user input validation is needed.  Please see file <strong>InputValidationMethods.java</strong> – it contains a good staring platform for your program.

<strong> </strong>

<strong> </strong>

<strong> </strong>

<h1>Pattern Display Method</h1>

Write a method

public static void patternDisplay(int size, char c, boolean direction) throws IllegalArgumentException that prints patterns of symbols.

Parameter size defines the size of pattern, in particular the size of the longest sequence of characters in the pattern.

Parameter c defines the choice of character that is used to display the patters Parameter direction defines the direction of the pattern.

Please see two function calls and the patterns they produced below.

The method must throw IllegalArgumentException when the value of parameter size is a negative number.




Test your new method in main(). Do not ask user for input, instead hard-code all the values you will be using to test your code. Make sure to use try/catch block in order to test that the exception is being thrown by the method when the argument size is negative. Make sure the method works well for correct arguments too.




patternDisplay(7, ‘+’, true)




























patternDisplay(4, ‘#’, false)

####

###

##

#

<strong> </strong>

<strong> </strong>

<strong> </strong>

<h1>Random Numbers in Files Method</h1>




Name this project RandomNumsInFiles.java

<strong><em> </em></strong>

This problem is based on the “File with Random Numbers” problem from Assignment 3.




Write method void randomNumsFile(String fileName, int howMany, int rangeFrom, int rangeTo) throws IOException that takes file name

as a string and 3 integer as parameters. The method generates random integers and saves them in a file, placing each new number on a new line. Parameters represent the following

<ol>

 <li>String fileName – file name. File created if it does not exist. <u>If the file does</u> <u>exist its content is being replaced with this method.</u></li>

 <li>int howMany – Number of random numbers to be generated</li>

 <li>int rangeFrom and int rangeTo – The range of random numbers to be generated. If the rangeFrom is smaller than rangeTo  – swap them.</li>

</ol>




This method throws IOException when the file fails to open for writing.




Test your method by calling it in main(). Make sure to use try-catch block to handle IOExcptions your new method may throw. Main() should not throw exceptions. Do not use user input for testing, <strong><u>create test cases</u></strong> that are easy to follow when reading your code.




<strong> </strong>

<strong> </strong>

<h1>File Analysis Method</h1>

<strong> </strong>

Write method int fileAnalysis (String inputFileName, String

outputFileName) that analyzes the sequence of integers stored in a file with a given name (inputFileName), and calculates the following statistics about the data stored in file:

<ul>

 <li>the number of integers stored,</li>

 <li>the largest and the smallest number stored in file,</li>

 <li>the total of all numbers stored in the file.</li>

</ul>

All that statistics must be stored in another file. The name of that output file is provided in parameter outputFileName.

The method returns the number of the integers processed.

Assume that all the numbers stored in the input file are integers and stored one number per line.

The method throws IOException when the files fail to open for reading and writing. If the input file does not exist, the method returns 0.




Sample statistics output file format is the following:

Numeric data file name: nums.txt

Number of integers: 5

The total of all integers in file: 15

The largest integer in the set: 5

The smallest integer in the set: 1




Test new method in main(). Make sure to use try/catch block to handle IOExceptions it may throw. Do not use user input for testing, <strong><u>create test cases</u></strong> that are easy to follow when reading your code.




<em>Suggested testing strategy: create a small testing text file containing 3 – 5 numbers that are easy to add up and where smallest and largest numbers are obvious. Make sure your method runs well with this data set. Do not use user input in your test cases. Sample file contents: </em>

<em>5 </em>

<em>3 </em>

<em>1 </em>

<em>4 </em>

<em>2 </em>


