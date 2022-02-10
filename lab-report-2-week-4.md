# 1.
![Screenshot (270)](https://user-images.githubusercontent.com/97714738/153325728-7b6ea480-4247-481d-8d84-95422277b15e.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file2.md)

Symptom:
![Screenshot (271)](https://user-images.githubusercontent.com/97714738/153336949-99debe61-e842-4273-81e9-1cf6d0c64af4.png)

The bug was that the code could not properly differentiate the difference between a link and an image, since they both are within parentheses. Therefore, when the code was run on the test file the output included the image along with the links (symptom). By adding an indicator that recognized if the text in the markdown file was an image (! before the text), the bug was fixed.


# 2.
![Screenshot (266)](https://user-images.githubusercontent.com/97714738/153323334-c787b6f9-c5ed-404d-8774-47b75101cdbd.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file3.md)

Symptom:
![Screenshot (272)](https://user-images.githubusercontent.com/97714738/153337454-68ba11d3-02c2-4d4a-85a4-4b8f2577c61d.png)

The symptom was the code outputs an IndexOutOfBoundsException because the code tried to output a substring with -1 as one of the parameters. Because there was text after the links in the markdown file some of the variables, like nextOpenBracket, were being set to -1. We fixed this issue by adding an if statement that prevented the code from creating a substring if any of the variables were -1.


# 3.
![Screenshot (268)](https://user-images.githubusercontent.com/97714738/153325460-c82f8e8c-bf95-41bd-9a27-a4572cf3dd66.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file8.md)

Symptom:

![Screenshot (274)](https://user-images.githubusercontent.com/97714738/153339173-e8ee7b36-df0c-4e47-a592-e7a697dc6446.png)


The symptom was the code outputs an IndexOutOfBoundsException. This was caused by the link being at the first index in the markdown file, so when looking for the image indicator, the index goes to -1. The change to the code made it so that the program doesn't check to see if the image indicator exists if the nextOpenBracket variable equals 0.
