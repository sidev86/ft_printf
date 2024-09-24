<h1>ft_printf</h1>

<h2>Description</h2>

The ft_printf project is a reimplementation of the standard printf() function from the C Standard Library <strong><em>libc</em></strong>. The goal of this project is to recreate key functionalities of printf() while adhering to specific restrictions and requirements. This function provides formatted output conversion, handling various type of data such as characters, strings, integers, and hexadecimal values.

<h2>Supported Conversions</h2>
<p>The <code>ft_printf</code> function supports the following conversions:</p>
<ul>
  <li><code>%c</code>: Prints a single character.</li>
  <li><code>%s</code>: Prints a string (following the standard C string format).</li>
  <li><code>%p</code>: Prints a <code>void *</code> pointer in hexadecimal format.</li>
  <li><code>%d</code>: Prints a decimal (base 10) number.</li>
  <li><code>%i</code>: Prints an integer in base 10.</li>
  <li><code>%u</code>: Prints an unsigned decimal (base 10) number.</li>
  <li><code>%x</code>: Prints a number in lowercase hexadecimal (base 16) format.</li>
  <li><code>%X</code>: Prints a number in uppercase hexadecimal (base 16) format.</li>
  <li><code>%%</code>: Prints a percent sign.</li>
</ul>

<h2>Usage</h2>
Type <code>make</code> to generate the library file libftprintf.a. <br>To use the library in your project just include the header file "ft_printf.h"<br>
Once imported into your project, the <code>ft_printf</code> function can be used in a similar way to the standard <code>printf()</code> function:
<br><br>
<strong><em><code>ft_printf("Character: %c, String: %s, Decimal: %d\n", 'A', "Hello", 123);</code></em></strong>

<h2>Compilation instructions</h2>

<code>gcc -o <strong><em>executable_name filename.c</em></strong> -L<strong><em>/path/to/lib</em></strong> -l:libftprintf.a</code>


