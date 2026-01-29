---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Data Storage"
date: 2025
published: true
labels:
  - C++
summary: "A project made for ICS 212"
---

For this project it was made in Visual Studio Code using C++. This project was about making a system that would store student and course information using classes. The user is able to create a list of cources and students and also assign courses to a student. This project served as a way to for us to practice data management and also obtaining and using user input.

This project was done by myself, it helped me to gain a better understanding of user interface.

Here is some code that illustrates how user input is read:

```cpp
std::string input;
while(1){
  std::cout << "1. Add Student\n2. Add Course\n3. Register Student for Course\n4. View all Students\n5. Delete a Student\n6. View Enrolled Students in a Course\n7. Search for a Student\n";
  std::cout << "Choice: ";
  std::getline(std::cin,input);
  std::cout << "\n";
  if(input == "1"){
    if(addStudent(studentNum,students)){
      studentNum++;
    }
  }else if (input == "2"){
    if(addCourse(courseNum,courses)){
      courseNum++;
    }
  }else if (input == "3"){
    registration(studentNum,students,courseNum,courses);
  }else if (input == "4"){
    viewallStudents(studentNum,students);
  }else if (input == "5"){
    if(deleteStudent(studentNum,students,courseNum,courses)){
      studentNum--;
    }
  }else if (input == "6"){
    viewenrolledStudents(courseNum,courses);
  }else if (input == "7"){
    findStudent(studentNum,students);
  }
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
