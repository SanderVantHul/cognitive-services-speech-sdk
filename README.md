Proces text to speech:

1. Remove all non ascii characters (regex: [^\x00-\x7F]+) 

2. Remove all code snippets

3. Select all white lines (regex: ^\s*$)

4. Replace with newline (regex: \n)

5. Now there is 2 white lines. Now replace all newlines with space. (regex: \n(?=\w+))

6. Now run text to speech program
