Proces text to speech:

1. Remove all code snippets

2. Select all white lines (regex: ^\s*$)

3. Replace with newline (regex: \n)

4. Now there is 2 white lines. Now replace all newlines with space. (regex: \n(?=\w+))

5. Now run text to speech program
