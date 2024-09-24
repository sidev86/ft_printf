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



