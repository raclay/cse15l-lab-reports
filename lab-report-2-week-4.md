Rachel Claypool
# Lab Report 2


## First Bug
![fix1](https://user-images.githubusercontent.com/97620200/151439793-0cdd4dfe-4d86-4481-b10e-e034488e40ff.jpg)

[test3](https://github.com/raclay/markdown-parse/blob/main/test3.md?plain=1)


![symptom1](https://user-images.githubusercontent.com/97620200/151440397-be5e8cf1-25db-4cbf-b5d4-74bbd37287bc.jpg)

The first bug that I fixed was the program's response to a markdown file without any brackets or parantheses.  
Since the indexOf command returns a -1 if that char cannot be found within the file, the program was attempting to 
add a substring to the ArrayList of toReturn that did not exist because the open/close paranthesis did not refer to
a specific index.  To resolve this problem, I  checked the value of the next open bracket and if the character was 
not found, then toReturn was returned without calling an add function.

