# 1.
![Screenshot (265)](https://user-images.githubusercontent.com/97714738/153322364-2a6e8a58-e327-499e-8b38-6764e2802e6f.png)

[Test File](https://github.com/aconsiglio03/markdown-parse/blob/main/test-file2.md)

The bug was that the code could not properly differentiate the difference between a link and an image, since they both are within parentheses. Therefore, when the code was run on the test file the output included the image along with the links. By adding an indicator that recognized if the text in the markdown file was an image (! before the text), the bug was fixed.
