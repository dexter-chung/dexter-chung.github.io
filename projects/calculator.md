---
layout: project
type: project
image: img/java_logo.png
title: "Stack Calculator"
date: 2024
published: true
labels:
  - Java
summary: "A calculator that uses the Stack Class to process operators and numbers"
---

<div class="text-center p-4">
  <img width="200px" src="../img/eclipse_logo.png" class="img-thumbnail" >
</div>

This program was made for my ICS 211 in which was made in eclipse using Java. For the basics on how it works, it will prompt the user to input either a number or a operator. If a number is given then it will be placed onto the top of a stack. If a operator was given then it will try to take the two numbers from the top of the stack and use them with the operator to produce a new number which returns to the top of the stack. 

For this project it was a individual assignment so I did it by myself. This project helped me 

Here is some code that illustrates how it reads user input and what it does based on that:
```cpp
while(true) {
	String input = scanner.nextLine().trim();
	if(input.equals("=")) {
		System.out.print("exiting calculator");
		break;
	}
			
	try {
		if("+-*/%^".contains(input)) {
			process(input);
		}else if(isNumber(input)){
			double value = Double.parseDouble(input);
			stack.push(value);
			System.out.println(value);
		}else {
			System.out.println("invalid input");
		}
	}catch (Exception e) {
		System.out.print("error " + e.getMessage());
	}
}
```
