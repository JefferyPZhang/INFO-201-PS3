# INFO 201 Problem Set: Control structures, Accessing Files, RMarkdown
October 23, 2023

1
1 Working with files
1.1 Find files in folder
1. What is the current working directory of the R instance that is compiling your homework
document? Use R to find it.
2. What is the folder (absolute path) of the rmarkdown document you use for your current
homework?
3. Now create a folder on your Desktop where you put
• At least 3 pdf files
• At least 3 image files
• At least 3 other files
How did you call that folder? What is the relative path of that folder with respect to the
working directory (in Q 1)?
4. Include a screenshot of the folder (in a file explorer) into this document as image. Use the
markdown tools to include the image!
Note: if your group is using different computers to answer the other questions below, then
please include the screenshot for all the computers you use!
5. Now use the relative path you wrote in Q 3 to list all files from within R. Store the list of files
into a variable, but also print it!
6. Do you see the same files as in the image?
7. Do you see the complete file name in the file explorer image?
1.2 Work with the files
1. Now write a loop that walks over all the files your found above. In the loop:
• Add the relative path of the folder to it
• If the file is an image (file name ends with jpg/png/heic), then load it and plot using
plot(). Print the file name above the plot!
• If the file is a pdf (file name ends with .pdf), then load the 2nd page of if and plot. Print
the file name underneath the plot
• If the image is something else, then print its name with a remark like “cannot be dis-
played”
2 Control structures
1. Take the vector of file names in your sample folder you created above. Transform each file
name into a sentence where you tell the file type for each file. The output should look like:
picture.jpg is an image file
2
document.pdf is a pdf file
output.log is something else
. . .
Do this using ifelse(), do not use loops or indexing!
2. Do you have any .png files included? Compute the number of png files, and print the corre-
sponding sentence. Depending on the number of png files, you should print either:
There are no png files
or
There is a single png file
or
There is n png files
where n is the number of png files!
3 Markdwon and RMarkdown
3.1 Markdown
1. Use markdown second level header for the title of the main question, and third level header
for the subquestion
2. Use markdown fourth level headers for each numbered item.
3. Create a bullet list of (at least 3) colors
4. Create a numbered list of (at least 3) cities.
5. Create a pre-formatted text (at least 3 lines)
6. Write a sentence that includes both bold and italic text.
7. Include an image in the text using markdown
3.2 RMarkdown
1. Count the number of images, pdf-s and other files in the folder above.
2. Print a sentence like
There are n files in the folder name folder, n1 images, n2 pdfs, and n3 other files.
The numbers n, n1, n2 and n3 should be the counts that you computed above, and the folder
name should be the folder name. Folder name should be in italics, and the counts in bold!
Use inline markdown to print it, so that the text will look a seamless sentence.
