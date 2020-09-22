<div align="center">

## C/C\+\+ 101: Introduction to C/C\+\+ \(Part II\)


</div>

### Description

This tutorial is made to help people learning C/C++ language which is commonly believed as a hard language.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Albert Tedja](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/albert-tedja.md)
**Level**          |Beginner
**User Rating**    |5.0 (40 globes from 8 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Documents](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/documents__3-27.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/albert-tedja-c-c-101-introduction-to-c-c-part-ii__3-2986/archive/master.zip)





### Source Code

<html>
<head>
<title>C/C++ 101: Introduction to C/C++ (Part I)</title>
</head>
<body>
<p><font face="Arial" size="4">C/C++ 101: Introduction to C/C++</font></p>
<p><font face="Arial" size="2">&nbsp;</font></p>
<p><font size="2" face="Arial"><b>Part II: return keyword, void data type, and printing text on
screen.</b></font></p>
<p><font face="Arial" size="2">&nbsp;</font></p>
<p><i><font face="Arial" size="2">Quote from the previous part:</font></i></p>
<p><i><font face="Arial" size="2">But wait, before this one, we didn't mention the type of return value of
function <font face="Courier New" size="2" color="#000080">main()</font>, would
that be okay? Technically, no. However, it depends on the compiler you use. Some
compilers put a default type if we don't specify it. For example, Borland Turbo
C++ 3.0 use <font face="Courier New" size="2" color="#000080">int</font> as the
default.</font></i></p>
<p><font face="Arial" size="2">&nbsp;</font></p>
<p><font face="Arial" size="2">In the previous section, we have discussed about
the </font><font color="#000080" face="Courier New" size="2">int</font><font face="Arial" size="2">
data type and how it affects the main return value. However, how do we return
the value? To do this, we use the keyword </font><font size="2" face="Courier New" color="#000080">return</font><font face="Arial" size="2">,
followed by the number we wish to return. So, if we modify our previous code to
return a value, we will get something like this:</font></p>
<table border="0" width="100%">
 <tr>
  <td width="100%" bgcolor="#99FFCC"><font face="Courier New" size="2">int</font><font face="Courier New" size="2"> main() {<br>
<br>
&nbsp;&nbsp;&nbsp; <font color="#0000FF">return 0;</font><br>
}</font></td>
 </tr>
</table>
<p><font face="Arial" size="2">The above code will return a number 0, and pass
it to the operating system. Why 0, not 1 or 999? In this case, 0 means
&quot;success.&quot; It means that our program exits in the proper way. There
are no such errors that terminate our program.&nbsp;What about if we replace the
0 with 1 or other numbers? It still compiles, but, you have to be careful. You
really are passing that number to the operating system. If you pass a non-zero
number, it means &quot;error,&quot; and you don't know what operating system is
going to do with that number. Last time I did it, I got a blue screen. I'm sure
you don't want to crash your own computer, so always put 0 even though you must
exit your program because of an error.</font></p>
<p><font face="Arial" size="2">If we look more carefully in the code above, we
will see a new symbol: a semi-colon (</font><font size="2" face="Courier New" color="#000080">;</font><font face="Arial" size="2">).
What is it doing there? In C/C++, it means &quot;end of statement.&quot; So, we
tell the compiler that we want to end our statement (</font><font size="2" face="Courier New" color="#000080">return
0</font><font face="Arial" size="2">) there. What about if we didn't include it?
The compiler would interpret the code above like this: </font><font size="2" face="Courier New" color="#000080">return
0}</font><font face="Arial" size="2">, and gives you error messages because it
doesn't recognize it. So, every time you want to end a statement, always use a
semi-colon.</font></p>
<p><font face="Arial" size="2">There is another data type that is commonly
associated with </font><font size="2" face="Courier New" color="#000080">main()</font><font face="Arial" size="2">.
It is called </font><font size="2" face="Courier New" color="#000080">void</font><font face="Arial" size="2">.
As the name suggests, it means empty or nothing; therefore, </font><font color="#000080" face="Courier New" size="2">main()</font><font face="Arial" size="2">
returns nothing. In this case, we don't specify any number after the keyword
return, leaving the code like this:</font></p>
<table border="0" width="100%">
 <tr>
  <td width="100%" bgcolor="#99FFCC"><font face="Courier New" size="2"><font color="#0000FF">void</font>
   main() {<br>
<br>
&nbsp;&nbsp;&nbsp; <font color="#0000FF">return ;</font><br>
}</font></td>
 </tr>
</table>
<p><font face="Arial" size="2">You may also want to omit the keyword </font><font size="2" face="Courier New" color="#000080">return</font><font face="Arial" size="2">,
removing it completely from the code. But keep in mind that </font><font size="2" face="Courier New" color="#000080">return</font><font face="Arial" size="2">
can also be used to end a function before the closing brace (</font><font size="2" face="Courier New" color="#000080">}</font><font face="Arial" size="2">).</font></p>
<p><font face="Arial" size="2">So, I think you have been bored with all of the
details, now let's code the real stuff.</font> <font face="Arial" size="2">The
simplest program in C that gives you some output is printing a text on the
screen. How do we do that? In C, this is done by using a function called </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">.
What </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">
does is printing a text on the screen. Suppose we want to print a text
&quot;Hello World&quot; on the screen using </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">.
How do we do that? Look at the following code:</font></p>
<table border="0" width="100%">
 <tr>
  <td width="100%" bgcolor="#99FFCC"><font face="Courier New"><font size="2">int</font></font><font face="Courier New" size="2"> main() {<br>
   &nbsp;&nbsp;&nbsp; <font color="#0000FF">printf(&quot;Hello World&quot;);</font><br>
<br>
&nbsp;&nbsp;&nbsp; return 0;<br>
}</font></td>
 </tr>
</table>
<p><font face="Arial" size="2">We put the string &quot;Hello World&quot; as an
argument of </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">.
Then, </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">
uses our &quot;Hello World&quot; and put it on the screen, and don't forget the
semi-colon. However, when you try to compile the above code, you will get an
error message telling you that the compiler doesn't recognize </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">
function, or it's undeclared (error messages may vary, depend on the compilers).
What's wrong with this? Nothing wrong. At this point, it's true that the
compiler doesn't recognize our </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">
function because we haven't defined/declared it yet. So, we need to define it
first before using it. The following code will show you how:</font></p>
<table border="0" width="100%">
 <tr>
  <td width="100%" bgcolor="#99FFCC"><font face="Courier New"><font size="2" face="Courier New"><font color="#0000FF">#include
   &lt;stdio.h&gt;</font><br>
   <br>
   int main() {<br>
   &nbsp;&nbsp;&nbsp; printf(&quot;Hello World&quot;);<br>
<br>
&nbsp;&nbsp;&nbsp; return 0;<br>
}</font></font></td>
 </tr>
</table>
<p><font face="Arial" size="2">Now it should compiles. However, </font><font face="Arial" size="2">you
may get confused with the new line we put in our code, but let's discuss one by
one. What is </font><font size="2" face="Courier New" color="#000080">#include</font><font face="Arial" size="2">?
It is a <i>directive</i> used to include the file specified, in this case: </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">,
to our code. What about the pound sign? Is that really necessary? Yes. That
pound sign shows actions that the compiler must take before compiling our code.
It has nothing to do with the code. In the above code, the action that the
compiler must take is to include file </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">
to our code. But what the heck is </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">?
</font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">
is called a header file and it's where </font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">
function is defined; that's why we include it. We want the compiler to know what
</font><font size="2" face="Courier New" color="#000080">printf()</font><font face="Arial" size="2">
is before we use it. Now, what about those less-than and greater-than symbols
enclosing </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">?
They tell the compiler to find the file </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">
in the <i>include directories</i>. Include directories? Yes, they are special
directories containing header files that we can include in our program. What
about if we want to include a file outside the include directories? There are
two ways of doing this. First, we copy that file to the include directories and
include it to our code as usual. Second, we replace the less-than and
greater-than symbols with other symbol: the quotation mark (</font><font size="2" face="Courier New" color="#000080">&quot;</font><font face="Arial" size="2">).
If we do this, the compiler will find the file in the specified location, if not
found, it will find it in include directories. Let's look at these examples:</font></p>
<p><font size="2" face="Courier New">1: <font color="#000080">#include &quot;filename.h&quot;</font><br>
2: <font color="#000080">#include &quot;C:\filename.h&quot;</font></font></p>
<p><font face="Arial" size="2">Number 1 will find file </font><font size="2" face="Courier New" color="#000080">filename.h</font><font face="Arial" size="2">
in the <i>current directory</i>, if not found, include directories. Number 2
will find file </font><font size="2" face="Courier New" color="#000080">filename.h</font><font face="Arial" size="2">
in C:\, if not found, include directories. It's really simple, huh?</font></p>
<p><font face="Arial" size="2">There's one thing I need to say regarding this
include stuff. </font><font size="2" face="Courier New" color="#000080">#include</font><font face="Arial" size="2">
is unique to C/C++ and sometimes it causes great confusion for non-C
programmers. C language doesn't have built-in functions like other languages. It
only has some keywords and symbols. So, every time we want to use a function, we
need to get it from other sources. That sources are called libraries. In order
to access these libraries, we need header files. The header files are just
regular files that contain C/C++ language, just like our code. However, they are
made to access the libraries which are written using Assembly language.
Different compilers have different header files. </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">
in compiler A may be different with </font><font size="2" face="Courier New" color="#000080">stdio.h</font><font face="Arial" size="2">
in compiler B, so, don't mix them up.</font></p>
<p><font face="Arial" size="2">This is the end of Part II. Next part, we will
talk more about printing text on the screen and some special characters we can
use in C/C++.</font></p>
<p>&nbsp;</p>
<p><font face="Arial" size="2">Some words used in this tutorial:</font></p>
<table border="1" width="97%" height="66">
 <tr>
  <td width="20%" height="1"><b><font size="2" face="Arial">directives</font></b></td>
  <td width="80%" height="1"><font size="2" face="Arial">directions that tells
   the compiler what to do before compiling the code.</font></td>
 </tr>
 <tr>
  <td width="20%" height="1" valign="top"><b><font size="2" face="Arial">include
   directories</font></b></td>
  <td width="80%" height="1"><font size="2" face="Arial">special directories
   where the header files are. Some compilers may only have one directory,
   but other compilers can have more than one.</font></td>
 </tr>
 <tr>
  <td width="20%" height="12"><b><font size="2" face="Arial">current directory</font></b></td>
  <td width="80%" height="12"><font face="Arial" size="2">current working
   directory, usually where the source code is.</font></td>
 </tr>
</table>
<p><font face="Arial" size="2">&nbsp;</font></p>
<p><font face="Arial" size="2">Note: all words, materials, and definitions
defined in this tutorial are my own opinions which I consider true. If in any
case you find them wrong, corrections would be very helpful. This tutorial is
made to help people learning C/C++ language which is commonly believed as a hard
language.</font></p>
<p><font face="Arial" size="2">Copyright (C) 2001, Albert Tedja.</font></p>
</body>
</html>

