1. Part One 
2. Part Two 

Choose two of the bugs from different files above. For each, show:
File: ArrayExamples.java <br/>
*The failure-inducing input (the code of the test)
- two index array <br/>
*The symptom (the failing test output)
- would print duplicate numbers. The last index would not update the first index. <br/>
*The bug (the code fix needed)
- the fix was to use a divide and conqueror approach. Also, I created a temp variable of type int to store the current value of the loop. <br/> 
*Then, explain the connection between the symptom and the bug. Why does the bug cause that particular symptom for that particular input?
- the connection between the symptom and the bug is the last index was not stored anywhere therefore would not be reversed. The bug causes the particular symptom because it would not correctly index the last index. 

