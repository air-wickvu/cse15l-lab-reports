1. Part One <br/>
Simple Search Engine Code: 
```import java.io.IOException;
import java.net.URI;
import java.util.*; 

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    ArrayList<String> items = new ArrayList <String>(); 

    public String handleRequest(URI url) {
        System.out.println("Path: " + url.getPath());

        if(url.getPath().contains("/add")){ 
            String[] parameters = url.getQuery().split("=");
            items.add(0,parameters[1]);
            return parameters[1];
        } else if(url.getPath().contains("/search")){
            
            String[] parameters = url.getQuery().split("=");
            ArrayList<String> matchedWords = new ArrayList<String>(); 

            for(int i= 0; i<items.size();i++){
                if(items.get(i).contains(parameters[1])){
                    matchedWords.add(0,items.get(i));
                }
            } 
            return matchedWords.toString();    
        }
    return "404 Not Found!";
    }   
}


class NumberServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
![screenshot1](https://github.com/air-wickvu/cse15l-lab-reports/blob/main/images/week-3-lab-report-image1.png)
- Which methods in your code are called: handleRequest is being called 
- What the values of the relevant arguments to those methods are, and the values of any relevant fields of the class: the relevant argument is the query specifically "/add" and "pineapple" 
- If those values change, how they change by the time the request is done processing: the values do not change unless I add in a different string. 

![screenshot2](https://github.com/air-wickvu/cse15l-lab-reports/blob/main/images/week-3-lab-report-image2.png)
- Which methods in your code are called: handleRequest is being called from the SearchEngine.java file 
- What the values of the relevant arguments to those methods are, and the values of any relevant fields of the class: the relevant argument is the query specifically "/add" and "apple" 
- If those values change, how they change by the time the request is done processing: the values do not change unless I add in a different string. 

![screenshot3](https://github.com/air-wickvu/cse15l-lab-reports/blob/main/images/week-3-lab-report-image3.png)
- Which methods in your code are called: handleRequest is being called 
- What the values of the relevant arguments to those methods are, and the values of any relevant fields of the class: the relevant argument is the query specifically "/add" and "fruit" 
- If those values change, how they change by the time the request is done processing: the values do not change unless I add in a different string.

![screenshot4](https://github.com/air-wickvu/cse15l-lab-reports/blob/main/images/week-3-lab-report-image4.png)
- Which methods in your code are called: handleRequest is being called 
- What the values of the relevant arguments to those methods are, and the values of any relevant fields of the class: the relevant argument is the query specifically "/query" and for my example searching for the subscript "app" in the list. 
- If those values change, how they change by the time the request is done processing: the values that do not match will not be printed. 

2. Part Two 

Choose two of the bugs from different files above. <br/>
File: ArrayExamples.java <br/>
- The failure-inducing input (the code of the test): two index array <br/>
- The symptom (the failing test output): would print duplicate numbers. The last index would not update the first index. <br/>
- The bug (the code fix needed): the fix was to use a divide and conqueror approach. Also, I created a temp variable of type int to store the current value of the loop. <br/> 
- Then, explain the connection between the symptom and the bug. Why does the bug cause that particular symptom for that particular input?: the connection between the symptom and the bug is the last index was not stored anywhere therefore would not be reversed. The bug causes the particular symptom because it would not correctly index the last index. 

