---
layout: project
type: project
image: img/java_logo.png
title: "Turn Based Game"
date: 2015
published: True
labels:
  - Java
summary: "A game that I developed for AP Computer Science "
---

This project was developed in Intellij using Java. It is a simple turned-based game in which you fight enemies to level up. The player are first prompted to choice one out of four classes which has their own unique mechanic. After the user player chooses a class and enemy is created in which the player has to fight, the enemy and the player would alternate turns whether that be to attack or defend until one of them is defeated. The game ends when the player's hp is less than or equal to zero.

For this project I did it completely by myself. What I learned from this project is the importance of organization and also putting comments in code.

Here is some code that illustrates how the user chooses thier class:

```cpp
while (Class == 0){
  System.out.println("Choose your Class" + "\n0) Mage" + "\n1) Rogue" + "\n2) Knight" + "\n3) Archer");
  option2 = scan.next();
  if (option2 .equals ("0")){
    player = new Mage("Mage");
    Class = 1;
    player.setmage();
    System.out.println(player);
   } else if (option2 .equals ("1")){
    player = new Rogue("Rogue");
    Class = 1;
    player.setrogue();
    System.out.println(player);  
  } else if (option2 .equals ("2")){
    player = new Knight("Knight");
    Class = 1;
    player.setknight();
    System.out.println(player);
  } else if (option2 . equals ("3")){
    player = new Archer("Archer");
    Class = 1;
    player.setarcher();
    System.out.println(player);
  }
}
```
