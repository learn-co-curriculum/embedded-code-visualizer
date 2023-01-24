#  Embedding Java Visualizer In A Lesson

https://github.com/learn-co-curriculum/java-tmp

## https://pythontutor.com/java.html

- Add link to browser-based debugging session 
- Embedded debugging session directly in lesson


1. Go to [https://pythontutor.com/java.html](https://pythontutor.com/java.html)
2. Enter Java Code.  Press "Visualize Execution".
3. Scroll down until you see the buttons to generate a permanent link or embed code.


Add the url into a lesson using a Markdown link or html anchor element.   

[Link to debugging session at pythontutor.com](https://pythontutor.com/visualize.html#code=public%20class%20StringUtility%20%7B%0A%20%20public%20static%20boolean%20containsVowel%28String%20str%29%20%7B%0A%20%20%20%20String%20vowels%20%3D%20%22aeiou%22%3B%0A%20%20%20%20for%20%28char%20c%20%3A%20str.toLowerCase%28%29.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20for%20%28char%20v%20%3A%20vowels.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20%28c%20%3D%3D%20v%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%20%20%0A%20%20public%20static%20void%20main%28String%5B%5D%20args%29%7B%0A%20%20%20%20System.out.println%28StringUtility.containsVowel%28%22HELLO%22%29%29%3B%20%20//true%0A%20%20%7D%0A%7D&cumulative=false&heapPrimitives=true&mode=edit&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false)

Embed the code in a lesson by copying the iframe element.

<iframe width="800" height="500" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=public%20class%20StringUtility%20%7B%0A%20%20public%20static%20boolean%20containsVowel%28String%20str%29%20%7B%0A%20%20%20%20String%20vowels%20%3D%20%22aeiou%22%3B%0A%20%20%20%20for%20%28char%20c%20%3A%20str.toLowerCase%28%29.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20for%20%28char%20v%20%3A%20vowels.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20%28c%20%3D%3D%20v%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%20%20%0A%20%20public%20static%20void%20main%28String%5B%5D%20args%29%7B%0A%20%20%20%20System.out.println%28StringUtility.containsVowel%28%22HELLO%22%29%29%3B%20%20//true%0A%20%20%7D%0A%7D&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=true&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>



## https://cscircles.cemc.uwaterloo.ca/java_visualize/ 

Link does not work if Java code contains double quotes!

Embedded:

<iframe style="width: 100%; height: 480;" src="https://cscircles.cemc.uwaterloo.ca/java_visualize/iframe-embed.html?faking_cpp=false#data=%7B%22user_script%22%3A%22public%20class%20StringUtility%20%7B%5Cn%20%20public%20static%20boolean%20containsVowel(String%20str)%20%7B%5Cn%20%20%20%20String%20vowels%20%3D%20%5C%22aeiou%5C%22%3B%5Cn%20%20%20%20for%20(char%20c%20%3A%20str.toLowerCase().toCharArray())%20%7B%5Cn%20%20%20%20%20%20%20%20for%20(char%20v%20%3A%20vowels.toCharArray())%20%7B%5Cn%20%20%20%20%20%20%20%20%20%20%20%20if%20(c%20%3D%3D%20v)%20%7B%5Cn%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%5Cn%20%20%20%20%20%20%20%20%20%20%20%20%7D%5Cn%20%20%20%20%20%20%20%20%7D%5Cn%20%20%20%20%7D%5Cn%20%20%20%20return%20false%3B%5Cn%20%20%7D%5Cn%20%20%5Cn%20%20public%20static%20void%20main(String%5B%5D%20args)%7B%5Cn%20%20%20%20System.out.println(StringUtility.containsVowel(%5C%22HELLO%5C%22))%3B%20%20%2F%2Ftrue%5Cn%20%20%7D%5Cn%7D%22%2C%22options%22%3A%7B%22showStringsAsValues%22%3Atrue%2C%22showAllFields%22%3Afalse%7D%2C%22args%22%3A%5B%5D%2C%22stdin%22%3A%22%22%7D&cumulative=false&heapPrimitives=false&drawParentPointers=false&textReferences=false&showOnlyOutputs=false&py=3&curInstr=0&resizeContainer=true&highlightLines=true&rightStdout=true" frameborder="0" scrolling="no"></iframe>