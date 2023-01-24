#  Embedding Code Visualization In A Lesson

## Learning Objectives

- Generate a link to a code visualization session
- Embedded a code visualization directly in a lesson

## Code Visualization

The Code Visualizer available at [https://pythontutor.com/](https://pythontutor.com/) is
for debugging and visualizing the execution of Python, Java, Javascript, C, and C++ programs.

1. Go to [https://pythontutor.com/](https://pythontutor.com/)
2. Click the link to the appropriate programming language.
3. Enter the code to visualize in the editor panel. 
4. Press "Visualize Execution".
   - You can use the "Next>" button to advance the program execution to a particular line of code. 

## Generating a link to a code visualization

Scroll down until you see the buttons to generate a permanent link or embed code. 

![generate buttons](https://curriculum-content.s3.amazonaws.com/6676/java-mod2-strings/generate_buttons.png)

You can add the link into a module lesson using Markdown or HTML.   

[Link to debugging session at pythontutor.com](https://pythontutor.com/visualize.html#code=public%20class%20StringUtility%20%7B%0A%20%20public%20static%20boolean%20containsVowel%28String%20str%29%20%7B%0A%20%20%20%20String%20vowels%20%3D%20%22aeiou%22%3B%0A%20%20%20%20for%20%28char%20c%20%3A%20str.toLowerCase%28%29.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20for%20%28char%20v%20%3A%20vowels.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20%28c%20%3D%3D%20v%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%20%20%0A%20%20public%20static%20void%20main%28String%5B%5D%20args%29%7B%0A%20%20%20%20System.out.println%28StringUtility.containsVowel%28%22HELLO%22%29%29%3B%20%20//true%0A%20%20%7D%0A%7D&cumulative=false&heapPrimitives=true&mode=edit&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false)


## Embedding the visualization into a lesson

You can also embed the visualization in a module lesson by copying the iframe element.

<iframe width="800" height="500" frameborder="0" src="https://pythontutor.com/iframe-embed.html#code=public%20class%20StringUtility%20%7B%0A%20%20public%20static%20boolean%20containsVowel%28String%20str%29%20%7B%0A%20%20%20%20String%20vowels%20%3D%20%22aeiou%22%3B%0A%20%20%20%20for%20%28char%20c%20%3A%20str.toLowerCase%28%29.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20for%20%28char%20v%20%3A%20vowels.toCharArray%28%29%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20%28c%20%3D%3D%20v%29%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%20%20%0A%20%20public%20static%20void%20main%28String%5B%5D%20args%29%7B%0A%20%20%20%20System.out.println%28StringUtility.containsVowel%28%22HELLO%22%29%29%3B%20%20//true%0A%20%20%7D%0A%7D&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=true&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

## Visualizing Method Execution and the Call Stack

The visualizer is particularly helpful in showing concepts like the call stack, parameter passing, etc.

[Visualizing Method Calls](https://pythontutor.com/visualize.html#code=import%20math%0A%0A%23A%20function%20can%20call%20another%20function%20%0A%0Adef%20calc_circle_area%28circle_diameter%29%3A%20%0A%20%20%20%0A%20%20%20circle_radius%20%3D%20circle_diameter%20/%202.0%20%0A%20%20%20circle_area%20%3D%20math.pi%20*%20circle_radius%20*%20circle_radius%20%0A%20%20%20return%20circle_area%20%0A%20%20%20%0Adef%20pizza_calories%28pizza_diameter%29%3A%20%0A%20%20%20calories_per_square_inch%20%3D%2016.7%20%20%20%0A%20%20%20%0A%20%20%20%23Call%20calc_circle_area%20function%20to%20get%20area%20of%20the%20pizza%20%0A%20%20%20pizza_area%20%3D%20calc_circle_area%28pizza_diameter%29%20%0A%20%20%20total_calories%20%3D%20pizza_area%20*%20calories_per_square_inch%20%0A%20%20%20return%20total_calories%20%0A%20%20%20%0A%23main%20algorithm%0Aprint%28'12%20inch%20pizza%20has%20%7B%3A.2f%7D%20calories.'.format%28pizza_calories%2812.0%29%29%29%0Aprint%28'14%20inch%20pizza%20has%20%7B%3A.2f%7D%20calories.'.format%28pizza_calories%2814.0%29%29%29&cumulative=false&curInstr=10&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false)


## Visualizing Memory Allocation

The visualizer helps with memory allocation for primitive data types versus reference types (objects).

[Visualizing Object State](https://pythontutor.com/visualize.html#code=public%20class%20PizzaTopping%20%7B%0A%20%20%20%20private%20String%20name%3B%0A%20%20%20%20private%20int%20likes%3B%0A%0A%20%20%20%20public%20static%20void%20main%28String%5B%5D%20args%29%20%7B%0A%20%20%20%20%20%20%20%20PizzaTopping%20topping1%20%3D%20new%20PizzaTopping%28%29%3B%0A%20%20%20%20%20%20%20%20PizzaTopping%20topping2%20%3D%20new%20PizzaTopping%28%29%3B%0A%20%20%20%20%20%20%20%20topping1.name%20%3D%20%22Mushroom%22%3B%0A%20%20%20%20%20%20%20%20topping1.likes%20%3D%2010%3B%0A%20%20%20%20%20%20%20%20topping2.name%20%3D%20%22Sausage%22%3B%0A%20%20%20%20%20%20%20%20topping2.likes%20%3D%2015%3B%0A%0A%20%20%20%20%20%20%20%20PizzaTopping%20favoriteTopping%20%3D%20topping2%3B%0A%20%20%20%20%20%20%20%20favoriteTopping.likes%2B%2B%3B%0A%20%20%20%20%20%20%20%20System.out.println%28%22My%20favorite%20topping%20is%20%22%20%2B%20favoriteTopping.name%29%3B%0A%0A%20%20%20%20%20%20%20%20System.out.println%28topping1.name%20%2B%20%22%20has%20%22%20%2B%20topping1.likes%20%2B%20%22%20likes%22%29%3B%0A%20%20%20%20%20%20%20%20System.out.println%28topping2.name%20%2B%20%22%20has%20%22%20%2B%20topping2.likes%20%2B%20%22%20likes%22%29%3B%0A%0A%20%20%20%20%7D%0A%7D&cumulative=false&curInstr=16&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=java&rawInputLstJSON=%5B%5D&textReferences=false)



## Resources

[https://pythontutor.com/](https://pythontutor.com/)