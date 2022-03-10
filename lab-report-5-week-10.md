Rachel Claypool
# Lab Report 5

## Finding Different Results

After running script.sh I manually searched through the results.  After Lab 9, with the added code to identify which test file contains all the required brackets and parantheses, I looked for results where my markdown-parse's output was not an empty list, and the given implementation returned an empty string even though the brackets and parantheses were found. 

## Test 487
```
[link](/my uri)
```

Given the contents of test 487, the correct output is Joe's, MarkdownParse should return an empty list.


Joe's implementation

![their487test](https://user-images.githubusercontent.com/97620200/157748442-93238a53-8e89-4a7a-b537-3ef8828a321f.jpg)

My implementation

![mytest487](https://user-images.githubusercontent.com/97620200/157748458-32c61325-7e43-4b64-9fb6-c5d8e4db8661.jpg)


To fix my implementation, I would have to add an additional check to indentify spaces within the text in parantheses.  There currently is a check for a space, but only when it is identified that the nextOpenBracket is not equal to zero.  The additional check needs to be copied and pasted inside the else statement.

![where to add code](https://user-images.githubusercontent.com/97620200/157751082-dd50250d-9cae-4c08-abef-1652245a19a0.jpg)



## Test 490
```
[link](<foo
bar>)
```

Given the contents fo test 490, the correct output is Joe's, MarkdownParse should return an empty list.


Joe's implementation

![their490test](https://user-images.githubusercontent.com/97620200/157752290-c6968d8a-a4fa-428a-b2d4-c936d0a48862.jpg)

My implementation

![mytest490](https://user-images.githubusercontent.com/97620200/157752335-4d6ac1a5-8116-4801-b0a1-ea4922e21729.jpg)


To fix my implementation, I would have to add an additional check to identify any newline characters within the text in parantheses.  We would have to place this check within both of the if and else statements, this change could be added to the check for the spaces, 
``` 
if(! markdown.substring(openParen + 1, closeParen).contains(" ") && ! markdown.substring(openParen + 1, closeParen).contains("\n"))
```
![where to add code](https://user-images.githubusercontent.com/97620200/157751082-dd50250d-9cae-4c08-abef-1652245a19a0.jpg)
