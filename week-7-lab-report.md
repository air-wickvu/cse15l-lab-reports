Part 1:

Chosen Task: Challenge In TestDocSearch.java, copy the test called testSearchCount, rename the new test to testSearchCount2 and change the query string being tested to tax rather than taxation. <br/>
Full Sequence: 
1.  `vim TestDocSearch.java<Enter>` 
2. `/@Test<Enter>`
3. `nn<shift+v>`
4. `jjjjjy`
5. `kp`
6. `/test<Enter>`
7. `ea2<Esc>`
8. `/ation<Enter>` 
9. `xxxxx` 
10. `:wq<Enter>` 

Sequence with Screenshots: 

1.  `vim TestDocSearch.java<Enter>` 
- ![image1](/images/week7-screenshot1.png)
- Description: I am entering vim editor with the file `TestDocSearch.java` 

2. `/@Test<Enter>`
- ![image2](/images/week7-screenshot2.png)
- Description: Searching for `@Test` with `/` 

3. `nn<shift+v>`
- ![image3](/images/week7-screenshot3.png)
- Description: Pressing `n` twice to find the next occurrence of `@Test`, then entering Visual mode with `<shift+v>`

4. `jjjjjy`
- ![image4](/images/week7-screenshot4.png)
- Description: Selecting lines of code with `j`, then yanking with `y` 

5. `kp`
- ![image5](/images/week7-screenshot5.png)
- Description: Cursoring up with `k`, then pasting yanked lines of code with `p` 

6. `/test<Enter>`
- ![image6](/images/week7-screenshot6.png)
- Description: Searching for `test` with `/`  

7. `ea2<Esc>`
- ![image7](/images/week7-screenshot7.png)
- Description: Moving the cursor to the end of the word with `e`, appending `2` to the end with `a`, then exiting Insert mode. 

8. `/ation<Enter>` 
- ![image8](/images/week7-screenshot8.png)
- Description: Searching for partial string, `ation` with `/`, to find the full word, taxation. 

9. `xxxxx` 
- ![image9](/images/week7-screenshot9.png)
- Description: Deleting characters to achieve wanted word with `x`, tax. 

10. `:wq<Enter>` 
- ![image10](/images/week7-screenshot10.png)
- Description: Saving file then quitting vim with `:wq`. I reentered vim to show the file correctly saved the edits. 


Part Two: 

Report how long it took you to make the edit in seconds in both styles, and any difficulties or details that came up in doing so: 

For editing the file on the local server then scp the file to the remote server took me about 7-8 minutes. A difficulty I had was to correctly set the destination path for the edited file, this caused me to take longer as I had to login into the remote account and confirm the path. A notable detail I noticed was the time required to transfer the file and to login into the remote took a majority of the time.

When I edited the file on the remote server, I was able to make the changes and run the test directly on the remote at about 5-6 minutes. I didn't face any difficulties but I did notice this method is much more efficient and I plan on using this method in the future when the situation arises. I was able to avoid the possible issue of correctly setting the destination path for the updated file.  

1. Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?

I would prefer being logged into the ssh session then making the edits remotely because it would save time overall. The reason is I would avoid entering the local computer, making the edits, then updating the file on the remote computer therefore I would save time. Also, it would be more efficient for when I am making changes to the code, and need to quickly test the changes on the remote. 


2. What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)

If the project has security preferences that do not allow me to clone the project to my local computer, I would be forced to make the edits remotely therefore influencing my decision. Another factor is if the project itself is very large in terms of data size, it would be inefficent to clone the project to the local computer then pushing the updates everytime. At the end of the day, I think learning both methods could be useful for when specific situations occur as it would allow you to be adapative and apply the method deemed most efficient. 