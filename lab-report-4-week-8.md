# Lab Report 4 (Week 8)

[My MarkdownParse](https://github.com/aconsiglio03/markdown-parse/blob/main/MarkdownParse.java)

[Group Reviewed MarkdownParse](https://github.com/nseyoum/CSE15L-Platypus)

# My Implementation
# Snippet 1

## Expected Output:
'["`google.com", "google.com", "ucsd.edu"]'

## Test:
![Screenshot (322)](https://user-images.githubusercontent.com/97714738/157550903-d5959509-a59b-46a5-a226-d446144c38d5.png)

## Output of test:
![Screenshot (317)](https://user-images.githubusercontent.com/97714738/157550989-d2289ef2-48af-45ad-809a-4e80e0b3e0c2.png)



# Snippet 2

## Expected Output:
'["a.com", "a.com(())", "example.com"]'

## Test:
![Screenshot (323)](https://user-images.githubusercontent.com/97714738/157551044-17f03d26-5021-4b4d-841f-8f3732fca73d.png)

## Output of Test:
![Screenshot (318)](https://user-images.githubusercontent.com/97714738/157551096-a69c5a38-c557-41fa-b0e0-b60a39d4ff05.png)



# Snippet 3

## Expected Output:
'["https://ucsd-cse15l-w22.github.io/"]'

## Test:
![Screenshot (321)](https://user-images.githubusercontent.com/97714738/157551174-b3f46388-91e3-4f34-8d54-a7832db2799d.png)

## Output of Test:
![Screenshot (319)](https://user-images.githubusercontent.com/97714738/157551255-8d59a98e-ff22-4db3-959c-87a3efdfa53c.png)


# Other Implementation
## Test 1
![Screenshot (317)](https://user-images.githubusercontent.com/97714738/157551549-ac879f79-786b-4146-b32a-6d1aa06d869f.png)

## Test 2
![Screenshot (318)](https://user-images.githubusercontent.com/97714738/157551579-28afe2e8-55a6-42eb-bad4-da1ef7a30e45.png)

## Test 3
![Screenshot (319)](https://user-images.githubusercontent.com/97714738/157551598-7afdd577-6046-4300-ad9b-7d0c5bda36ea.png)

# Response
1. Snippet 1 had a faulty output partially because of not checking for brackets within brackets. This could be fixed in under 10 lines of code using a stack (as suggested by the group that reviewed our code). For each open bracket, it could be pushed onto the stack, and for each closed, it could be popped from the stack.

2. Snippet 2 had a similar issue, with parentheses and brackets within the links. This can also be fixed with the implementation stated before, using a stack.

3. Snippet 3 had an issue with the output because my code doesn't check for empty spaces or long stretches. If I were to check to make sure there were no spaces within the link, this issue could be fixed.
