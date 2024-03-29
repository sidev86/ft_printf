In this 42 project, you will recreate one of the most commonly used functions in the C language: the printf function.

<h1 align="left">What is printf?</h1>

- The printf function is one of the most common output functions in the C language. It is a function that is part of the 'stdio.h' library, 
which is a library that contains a set of features for handling input and output (stdio is short for 'standard input output'). 
Its main purpose, is to format and print data to standard output 'stdout' (usually the screen), according to a specified format.

- It is possible, through the use of this function, to print simple text messages and/or the content of data in various formats.
Format means the type of data to which we refer (for example an integer value, decimal, a string, a character, etc.)

- Since it is a function that can handle a different number of arguments, the function is said to be variadic.


<h1>What is a variadic function?</h1>

- To better understand what the term 'variadic' means, let's look at the syntax definition of the function:<br>

<code>&nbsp;&nbsp;&nbsp;int printf(const char *format, ...);</code>



- format: specifies how the data should be formatted and displayed.
- ...: The ellipsis operator (...) indicates that the function can accept a variable number of arguments, corresponding to the data to be formatted and printed.

- By variable number of arguments, we mean that when we call our function within our message, there may be a variable number of data to print the contents of.
It can be 1 data, it can be 2 datas, 3 datas, hundreds of datas or even no data but only simple text.
Hence the term 'variadic function'.

In case that the message we need to show consists only of simple text, we will write our message between "" like this:

Text => hello world

<code>printf(“hello world”);</code>

In case we want to print the data content we need to define the data format in our text:


<h1>Data format (most common)</h1>

%d : base 10 integers <br>
%s : strings <br>
%c : characters <br>
%x : hexadecimal <br>


<h1>Practical examples</h1>

<code>int day_in_year = 365;</code><br>
<code>printf(“In a year there are %d days”, day_in_year)</code>

Output message -> In a year there are 365 days


<code>char *food = “carrots”;</code> <br>
<code>char *color = “orange”;</code><br>
<code>printf(“The %s are %s”, food, color);</code>

Output message ->The carrots are orange


<code>char letter = 'E';</code><br>
<code>int index = 5;</code><br>
<code>printf(“%c is the %dth letter of the alphabet)</code>

Output message -> E is the 5th letter of the alphabet


<h1>Tips for making this project</h1>

- Starting from the first character, scroll through the string passed as input to the ft_printf, character by character.
 
- If the character we're pointing to, is a simple text character, print it as it is.

- If it is a character that defines a data format (%) ,check the format by checking the character that you find next to it (d or s or c...) and pass the argument
  associated with the format to another function which then check the format to convert, and give back converted to the main function ready to print on the screen

- Repeat these steps above, until you reach the end of the string.

- Go and look at the va_start, va_arg, va_copy and va_end functions to understand the management of the arguments in your ft_printf.



<h1>Useful resources</h1>

<a href="https://www.youtube.com/watch?v=oDC208zvsdg">Variadic Functions</a><br>
<a href="https://www.youtube.com/watch?v=zuegQmMdy8M">Pointers</a><br>
