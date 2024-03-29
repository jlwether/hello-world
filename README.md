# hello-world
a first experiment

OK, just testing out the interface.  
Not too bad for working with a simple text file.

Actually, I've heard that github markdown allows you to insert LaTeX math, so I want to test that.

see https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions

**Inline math:**

Math is called inline when it is placed in the flow of the text.
* "$"-syntax works: `$e^{i\pi} + 1 = 0$` gives $e^{i\pi} + 1 = 0$.
* But not the alternate "\\(" ... "\\)" syntax from LaTeX: `\(e^{i\pi} = - 1\)` gives \(e^{i\pi} = - 1\), so that doesn't work.

**Display math**

Display math is shown on it's own line, usually centered horizontally.  Here is an example of what this looks like:

$$ e^{i\pi} + 1 = 0 $$

For display math, the `$$` syntax from LaTeX works, but there are some limits:
```
* You can't put the display math on the same line as other text. This: $$ e^{i\pi} + 1 = 0 $$
   doesn't work.
```
* You can't put the display math on the same line as other text. This: `$$ e^{i\pi} + 1 = 0 $$` 
   doesn't work.
```
* It also has problems if it is on its own line but immediately after a list, 
   because markdown sees it as part of the list text:
$$ e^{i\pi} + 1 = 0 $$
```
* It also has problems if it is on its own line but immediately after a list, 
   because markdown sees it as part of the list text:
$$ e^{i\pi} + 1 = 0 $$
```
* But it is OK if you make the display math it's own paragraph:

$$e^{i\pi} + 1 = 0$$
```
* But it is OK if you make the display math it's own paragraph:

$$e^{i\pi} + 1 = 0$$
```
In non-list text, it is sometimes sufficient for it to be on its own line, but I think it is good 
practice to use a separate paragraph, because that always seems to work.  But here goes:
$$e^{i\pi} + 1 = 0$$
Yes, that works.
```
In non-list text, it is sometimes sufficient for it to be on its own line, but I think it is good 
practice to use a separate paragraph, because that always seems to work.  But here goes:
$$e^{i\pi} + 1 = 0$$
Yes, that works.

Finally, the "$$" syntax doesn't work if it is a long equation where you want several lines for 
entering the equation.  For this, a "math" code block is supposed to work, but I don't seem to be doing it right:
```math
e^{i\pi}  + 1 = 0
```
So I guess you just have to put math equations on a single input line in the markdown file.
