[Back to Index](https://clingunis.github.io/cse15l-lab-reports/index.html)

# Lab Report 2 Week 4

## Debug Code Change #1

Code Change:
![Image](Images/ImageFix.PNG)

Failure-inducing Input File:

[Link to the file](https://raw.githubusercontent.com/clingunis/markdown-parse/main/test-file2.md)

Symptom Screenshot:

![Image](Images/ImageSymptom.PNG)

Description:

The failure-inducing input was a file with an image attachment. The symptom was that it returns the name of the image file along with the links in the list of links. We expect only links and not image file names. 
The bug is that our code did not account for the similar format of images and links, since images follow a similar bracket and parentheses syntax as links but with a '!' character before. The code change makes it so the program accounts for if there is a '!' character before the first open bracket and does not add the content between the parentheses to the list of links to return if there is a '!' character before the first open bracket.

