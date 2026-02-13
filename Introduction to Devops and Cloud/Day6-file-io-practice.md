# Linux Fundamentals: Read and Write Text Files
- echo "Linux fundamentals practice" > notes.txt - creates file OR overwrites file - echo → prints text, > → creates file OR overwrites file, notes.txt → file name
- echo "Learning file operations in Linux" >> notes.txt
- echo "Using redirection operators" >> notes.txt - >> → append (add new line without deleting old data)
- echo "This line is written using tee" | tee -a notes.txt - tee → shows output on screen and writes to file, -a → append mode
- head -n 3 notes.txt - Shows first three lines
- tail -n 3 notes.txt - Shows last three lines

 
