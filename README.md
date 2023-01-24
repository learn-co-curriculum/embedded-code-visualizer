# Test Embedded Visualizer

## Learning Goals

- Learning Goal 1
- Learning Goal 2

## Introduction

Embedding Java Visualizer in a lesson.

## Link to external debugging session

[Link to debugging session at pythontutor.com](https://pythontutor.com/visualize.html#code=public%20class%20StringUtility%20%7B%0A%20%20public%20static%20boolean%20containsVowel%28String%20str%29%20%7B%0A%20%20%20%20String%20vowels%20%3D%20%22aeiou%22%3B%0A%20%20%20%20for%20%28char%20c%20%3A%20str.toLowerCase%28%29.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20for%20%28char%20v%20%3A%20vowels.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20%28c%20%3D%3D%20v%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%20%20%0A%20%20public%20static%20void%20main%28String%5B%5D%20args%29%7B%0A%20%20%20%20System.out.println%28StringUtility.containsVowel%28%22HELLO%22%29%29%3B%20%20//true%0A%20%20%7D%0A%7D&cumulative=false&heapPrimitives=true&mode=edit&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false)

## Embedded debugging session

text before

<iframe width="800" height="500" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=public%20class%20StringUtility%20%7B%0A%20%20public%20static%20boolean%20containsVowel%28String%20str%29%20%7B%0A%20%20%20%20String%20vowels%20%3D%20%22aeiou%22%3B%0A%20%20%20%20for%20%28char%20c%20%3A%20str.toLowerCase%28%29.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20for%20%28char%20v%20%3A%20vowels.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20%28c%20%3D%3D%20v%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%20%20%0A%20%20public%20static%20void%20main%28String%5B%5D%20args%29%7B%0A%20%20%20%20System.out.println%28StringUtility.containsVowel%28%22HELLO%22%29%29%3B%20%20//true%0A%20%20%7D%0A%7D&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=true&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>


text after