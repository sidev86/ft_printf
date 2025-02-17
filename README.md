<h1>ft_printf</h1>

<h2>Description</h2>

The ft_printf project is a reimplementation of the standard printf() function from the C Standard Library <strong><em>libc</em></strong>. The goal of this project is to recreate key functionalities of printf() while adhering to specific restrictions and requirements. This function provides formatted output conversion, handling various type of data such as characters, strings, integers, and hexadecimal values.
<br><br>
<h2>Supported Conversions</h2>
<p>The <code>ft_printf</code> function supports the following conversions:</p>
<ul>
  <li><strong><code>%c</code></strong>: Prints a single character.</li>
  <li><strong><code>%s</code></strong>: Prints a string (following the standard C string format).</li>
  <li><strong><code>%p</code></strong>: Prints a <code>void *</code> pointer in hexadecimal format.</li>
  <li><strong><code>%d</code></strong>: Prints a decimal (base 10) number.</li>
  <li><strong><code>%i</code></strong>: Prints an integer in base 10.</li>
  <li><strong><code>%u</code></strong>: Prints an unsigned decimal (base 10) number.</li>
  <li><strong><code>%x</code></strong>: Prints a number in lowercase hexadecimal (base 16) format.</li>
  <li><strong><code>%X</code></strong>: Prints a number in uppercase hexadecimal (base 16) format.</li>
  <li><strong><code>%%</code></strong>: Prints a percent sign.</li>
</ul>

<h2>Usage</h2>
Type <code>make</code> to generate the library file <code>libftprintf.a.</code> To use the library in your project just include the header file "ft_printf.h". Once imported into your project, the <code>ft_printf</code> function can be used in a similar way to the standard <code>printf()</code> function:

<h3>Example</h3>
<strong><code>ft_printf("Character: %c, String: %s, Integer number: %d\n", 'A', "Hello", 123);</code></strong>
<br><br>
<h2>Compilation instructions</h2>

<code>gcc -o <strong><em>executable_name filename.c</em></strong> -L<strong><em>/path/to/lib</em></strong> -l:libftprintf.a</code>


