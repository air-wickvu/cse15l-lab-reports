Part 1:

Chosen Task: Challenge In TestDocSearch.java, copy the test called testSearchCount, rename the new test to testSearchCount2 and change the query string being tested to tax rather than taxation. 

Sequence: 

1.  `vim TestDocSearch.java<Enter>` 
- ![image1](/images/week7-screenshot1.png)
- Description: Entering vim editor with the file TestDocSearch.java 

2. `/@Test<Enter>`
- ![image2](/images/week7-screenshot2.png)
- Description: Searching for @Test

3. `nn<shift+v>`
- ![image3](/images/week7-screenshot3.png)
- Description: Pressing n to find the next occurrence of @Test, then entering Visual mode

3. `jjjjjy`
- ![image4](/images/week7-screenshot4.png)
- Description: Selecting lines of code, then yanking 

4. `kp`
- ![image5](/images/week7-screenshot5.png)
- Description: Cursoring up, then pasting yanked lines of code

5. `/test<Enter>`
- ![image6](/images/week7-screenshot6.png)
- Description: Searching for /test 

6. `ea2<Esc>`
- ![image7](/images/week7-screenshot7.png)
- Description: Moving the cursor to the end of the word, appending the number 2, then exiting the insert mode. 

7. `/ation<Enter>` 
- ![image8](/images/week7-screenshot8.png)
- Description: Searching for the full word, taxation, but i am using partial words /ation to save keystrokes.

8. `xxxxx` 
- ![image9](/images/week7-screenshot9.png)
- Description: Deleting characters to achieve wanted word. 

9. `:wq<Enter>` 
- ![image10](/images/week7-screenshot10.png)
- Description: Saving file then quitting vim. I reentered vim to show the file correctly saved the edits. 


Part Two: 

1. Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?

2. What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)