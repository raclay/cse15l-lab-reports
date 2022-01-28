Rachel Claypool
# Lab Report 2


## First Bug
![fix1](https://user-images.githubusercontent.com/97620200/151439793-0cdd4dfe-4d86-4481-b10e-e034488e40ff.jpg)

A file without any links caused an error:
[test3](https://github.com/raclay/markdown-parse/blob/main/test3.md?plain=1)


![symptom1](https://user-images.githubusercontent.com/97620200/151440397-be5e8cf1-25db-4cbf-b5d4-74bbd37287bc.jpg)

The first bug that I fixed was the program's response to a markdown file without any brackets or parantheses.  
Since the indexOf command returns a -1 if that char cannot be found within the file, the program was attempting to 
add a substring to the ArrayList of toReturn that did not exist because the open/close paranthesis did not refer to
a specific index.  To resolve this problem, I  checked the value of the next open bracket and if the character was 
not found, then toReturn was returned without calling an add function.

## Second Bug
![fix2](https://user-images.githubusercontent.com/97620200/151491802-3c4182b4-69d4-43fb-b5f2-57cee078a94e.jpg)

A file with links and an image caused an error:
[myTest](https://github.com/raclay/markdown-parse/blob/main/myTest.md?plain=1)


![symtpom 2](https://user-images.githubusercontent.com/97620200/151492026-92913be0-72b1-4ad5-a3f0-bbcf007432e3.jpg)

The second bug I fixed was the program's response to a markdown file with an image among the links.  The function of
the program was to return an ArrayList of Strings, strings that are found between parantheses.  We did not want the title
of the image file to be added to our ArrayList, so I had to change the code to check for a '!' character before the opening
bracket and skip to the next iteration without retaining the link.
