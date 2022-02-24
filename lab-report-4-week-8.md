Rachel Claypool
# Lab Report 4
[my repository](https://github.com/raclay/markdown-parse)

[their repository](https://github.com/zfxd/markdown-parse)


## Test 1
![snip1](https://user-images.githubusercontent.com/97620200/155594620-4c684682-a721-419c-bee8-5b4e0bd74893.jpg)

According to the demo site, the valid link is [`google.com]

However, knowing that ` is an unsafe character in a url, we would want our program to return [google.com], the other
links are found within embedded code, which we do not want our function to recognize as a link.
![lab4test1](https://user-images.githubusercontent.com/97620200/155598199-1ba5aa68-a912-4ec7-9a58-8d0e8f0beb11.jpg)

My file did not pass the first test
![mylab4fail1](https://user-images.githubusercontent.com/97620200/155599142-8b37eda7-bf05-4441-bcab-ad7229651712.jpg)


The file I reviewed did not pass the first test
![theirlab4test1](https://user-images.githubusercontent.com/97620200/155599999-b09bcf9f-1979-4f7c-ad6e-20e012e3d928.jpg)


# Test 2
#![snip2](https://user-images.githubusercontent.com/97620200/155594649-0f5e0a12-f95f-4bb8-8c45-cef43657ceb6.jpg)

According to the demo site, the valid links are [a.com, a.com(()), example.com]
![lab4test2](https://user-images.githubusercontent.com/97620200/155597969-123de234-08e1-41fd-af65-c2c8df3feef9.jpg)

My file did not pass the second test
![mylab4fail2](https://user-images.githubusercontent.com/97620200/155599194-53263a8a-87fb-4039-be72-dc99abad0bc9.jpg)


The file I reviewed did not pass the second test
![theirlab4test2](https://user-images.githubusercontent.com/97620200/155600071-5377c57f-eff6-4f9b-9b13-4fb35fe755d1.jpg)



## Test 3
![snip3](https://user-images.githubusercontent.com/97620200/155594682-a3bda641-808b-4002-b7b9-7a900662b2ce.jpg)

According to the demo site, the valid link is [https://ucsd-cse15l-w22.github.io/] 
![lab4test3](https://user-images.githubusercontent.com/97620200/155597973-8d4d552e-1a16-468a-8f85-f400231395e9.jpg)

My file did not pass the third test
![mylab4fail3](https://user-images.githubusercontent.com/97620200/155599239-fb590370-d062-4803-b509-f1086f2e454b.jpg)


The file I reviewed did not pass the third test
![theirlab4test3](https://user-images.githubusercontent.com/97620200/155600114-52899834-eb68-494d-b685-e8b3ab57bb8d.jpg)

-----
## Snippet 1 Code Change
I think that there should be a decently small code change to make my program work for snippet 1 and other markdown files that contain inline code.  Similar to the program's ability to isolate the text within parantheses to list off links, maybe creating new variables for the backticks that signify the beginning and ending of embedded code would allow the program to keep that code out of the list of links that get returned.  For other embedded code blocks using the three backticks, the code would have to check for the beginning and ending three consecutive backticks and skip over the code between them.

## Snippet 2 Code Change


## Snippet 3 Code Change
I think that there should be a decently small code change to make my program workd for snippet 3 and other 
markdown files that contain newline characters within the brackets and parantheses.  If we have the program check the character right before the closed paranthesis  
