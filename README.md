# CS3

CS3 (AKA CSSS, AKA CSS Sorter)
is a CSS rule sorter.

Due to personal preference,
developers might want to keep their CSS rules alphabetically sorted.
This becomes harder as the number of lines increase.
CS3 provides a simple way to
individually sort rules of every ruleset (or block) alphabetically.

### Warning

- CS3 works only if it is fed CSS of a specific format:

  ```
  selector {
      property: value;
      property: value;
      ...
  }
  ```

_**Note:**
This was created and tested using
Firefox Developer Edition 77.0b6 (64-bit)
on Ubuntu 16.04 LTS.
There may be discrepancies in case of other browsers 
or other versions of the same browser(s)
or other operating systems._

### Why Use It

CSS rules, sorted alphabetically, are useful for
both personal aesthetics and ease of finding one out quickly.
If sorted,
we can intuitively look for a rule starting with a "z" from the bottom
and one starting with a "c" from the top.
This saves a quite a good amount of time when there are lots of rules.

### How to Use It

On the HTML page, there are two boxes and one button.
The box on the left is for input,
and the one on the right for output.

1. Paste your code in the input box.

2. Click the "Sort" button.

The sorted code will appear in the output box.

### How It Works

CS3 breaks the entire code down by splitting them at line breaks.
Then it separates rulesets (or blocks)
by detecting the starting and the ending curly braces,
and sorts the lines (rules) inside using JavaScript's native "`sort()`" function.

### Upside

- Rules can easily be sorted repeatedly without much manual labor.

- Finding a rule in the sorted form saves a lot of time.

### Downside

- CS3 only supports input of a specific format.

### Future Plan

- Support CSS of more formats
  - All rules in a single line
  - Mixed formats

### Miscellaneous

#### Is there a debug mode?

No.
But helpful messages may be printed in the browser console in a few scenarios.
