In this 42 project you will recreate one of the most commonly used functions in the C language: the printf function

<h1 align="left">What is printf?</h1>

- The printf function is one of the most common output functions in the C language. It is a function that is part of the stdio.h library, 
which is a library that contains a set of features for handling input and output (stdio is short for 'standard input output'). 
Its main purpose is to format and print data to standard output 'stdout' (usually the screen) according to a specified format.

- It is possible, through the use of this function, to print simple text messages and/or the content of data in various formats.
Format means the type of data to which we refer (for example an integer value, decimal, a string, a character, etc.)

- Since it is a function that can handle a different number of arguments, the function is said to be variadic.


<h1>What is a variadic function</h1>

- To better understand what the term variadic means, let's look at the syntactic definition of the function:
 <code>int printf(const char *format, ...)</code>



- format: It is a format string that specifies how the data should be formatted and displayed.
- ...: The ellipsis operator (...) indicates that the function can accept a variable number of arguments, corresponding to the data to be formatted and printed

- By variable number of arguments we mean that when we call our function, within our message, there may be a variable number of data to print the contents of.
It can be 1 data, it can be 2 data, 3 data, hundreds of data or even no data but only simple text.
Hence the term variadic function.

In the event that the message we need to show consists only of simple text, we will write our message between "" like this:

Text => hello world

printf(“hello world”);

In case we want to print the data content we need to define the data format in our text:


<h1>Data format (most common)</h1>

%d : base 10 integers
%s : strings
%c : characters
%x : hexadecimal


<h1>Practical examples</h1>

- I print the number of days of the year:

int day_in_year = 365;

printf(“In a year there are %d days”, day_in_year)

Output message -> In a year there are 365 days


char *food = “carrots”;
char *color = “orange”;

printf(“The %s are %s”, food, color);
Output message ->The carrots weigh 1.75 Kilos


char letter = 'E';
int index = 5;


printf(“%c is the %d th letter of the alphabet)

Output message -> E is the 5th letter of the alphabet


<h1>Tips for making this project</h1>

- Starting from the first character, scroll through the string passed as input to the ft_printf character by character.
 
- If the character I'm on is a simple text character, print it as it is.

- If it is a character that defines a data format (%) ,check the format by checking the character that you find next to it (d or s or c...) and pass the argument
  associated with the format to another function which then check the format to convert, and give back converted to the main function ready to print on the screen

I repeat these steps until the end of the string

- Go and look at the va_start, va_arg, va_copy and va_end functions to understand the management of the arguments in our ft_printf



<h1>Useful resources</h1>

<a href="https://www.youtube.com/watch?v=GExnnTaBELk">Makefile</a><br>
<a href="https://www.youtube.com/watch?v=zuegQmMdy8M">Pointers</a><br>
<a href="https://www.youtube.com/watch?v=uBZHMkpsTfg&list=PLfqABt5AS4FmXeWuuNDS3XGENJO1VYGxl">Lists</a>
