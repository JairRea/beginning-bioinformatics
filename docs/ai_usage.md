# AI Use Log
- Tool/model & version:

  ChatGPT 5 // Gemini 2.0 // Microsoft CoPilot // Claude AI
---
- What I asked for:

  For Rosalind problem 2: Explain splicing and indices and provide examples with explanations.

  For Rosalind problem 5: Provide me examples of python dictionaries and explain how python dictionaries work line by line.

  For Task 19.2: How could I implement Count() to a previous solution of mine.

  For Rosalind problem 9: Would I need to multiply my output so that it could match the following output and is that correct to do.
---
- Snippet of prompt(s):

  In Python, every character in a string (or item in a list) has a position, called an index. It starts at zero. So if you have the word , the letter  is at position 0,  is at 1, and so on. You can grab any character by using its index like this:  gives you .
Now, slicing—or splicing—is how you grab a chunk of that string. You use a colon to say where to start and where to stop. For example,  gives you . It starts at index 1 and goes up to—but doesn’t include—index 4. That’s a key thing: Python slicing always stops just before the end index.

  In Python, a dictionary is a built-in data structure that stores data in key-value pairs. Unlike lists, which are ordered collections indexed by position, dictionaries are unordered collections indexed by keys. Each key in a dictionary must be unique, and it maps to a corresponding value. This structure is incredibly useful when you want to associate one piece of data with another—for example, storing a person’s name as a key and their age as the value.

  When you read the file and split it into words using line.split() , you get a list—something like [list]. This list contains duplicates because words can appear more than once in the text. If you loop through that list directly and use  on each word, you’ll end up recalculating the count for  three separate times, once for each occurrence. That’s inefficient, especially for large files. This is where Set() comes in. A set in Python is an unordered collection of unique elements. When you pass your list of words into , it strips out all the duplicates and gives you just the unique words. So  becomes set(EXAMPLE) bceomes the following. By looping over set(words), you ensure that each word is only processed once.
---
- What I changed before committing:

  I changed the outputs for certain cells that matched what I was provided via Rosalind.

  I completed every cell making sure everything was completed perfectly and ran with no errors.

  I changed the color of each headings/sections color to green so that I would not lose track as I went along with the file & problems. Yellow signified that I was working on a cell block and it was not done yet.
---
- How I verified correctness (tests, sample data):

  I provided the sample dataset and ran the code to check it.
  
  I did tests of my own to see if there were any errors that would pop up.
  
  I asked AI to provide me more examples to continue testing.
  
  I asked AI if there was potentially anything wrong with my code.
