Proces text to speech:

1. Remove all non ascii characters (regex: [^\x00-\x7F]+) 

2. Remove all code snippets

3. Select figures for change if necessary (regex: figure(?=[ \d]))

4. Select all white lines (regex: ^\s*$)

5. Replace with newline (regex: \n)

6. Now there is 2 white lines. Now replace all newlines with space. (regex: \n(?=\w+))

7. Create newline after every period (.) (regex: (?!\D\w)\.    |   replace with: .\n\n)

8. Replace starting space if necessary (regex: ^\s*)

9. Now run text to speech program