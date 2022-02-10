# 1.
![Screenshot (267)](https://user-images.githubusercontent.com/97714738/153323319-d05bc26b-2e94-448c-8bf4-8b593edabf27.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file2.md)

The bug was that the code could not properly differentiate the difference between a link and an image, since they both are within parentheses. Therefore, when the code was run on the test file the output included the image along with the links (symptom). By adding an indicator that recognized if the text in the markdown file was an image (! before the text), the bug was fixed.


# 2.
![Screenshot (266)](https://user-images.githubusercontent.com/97714738/153323334-c787b6f9-c5ed-404d-8774-47b75101cdbd.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file3.md)

The symptom was the code outputs an IndexOutOfBoundsException because the code tried to output a substring with -1 as one of the parameters. Because there was text after the links in the markdown file some of the variables, like nextOpenBracket, were being set to -1. We fixed this issue by adding an if statement that prevented the code from creating a substring if any of the variables were -1.

# 3.
![Screenshot (268)](https://user-images.githubusercontent.com/97714738/153325460-c82f8e8c-bf95-41bd-9a27-a4572cf3dd66.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file8.md)

The symptom was 
