## Academic Management System
### PROJECT EXPLANATION:
I have designed an academic management system to calculate the final mark output of students in an academy. I have also designed a bonus mark allocation to the students who have done something extra curricular in their academic session. The ones who have done something against the academy’s agenda should also be punished so I have also allocated negative marks to those students. The final results are published considering all the activities of the students including the academic performance extra-curricular activities and also the negative marks for bad behaviour.

![draw]([https://user-images.githubusercontent.com/76884959/172964022-504314b0-1c60-4d68-9478-7ed1fde24074.png](https://github.com/Dark-knight-02/JAVA-PROJECT-MA-104-ASSIGNMENT/blob/main/Untitled%20Diagram.drawio.png))


### Functions of class:
#### Abstract class Registration:
Defines the attributes that are needed for a candidate to register. Contains an abstract method which displays the information.

#### Class Student:
Inherits Registration. Contains additional attributes of professor name and roll number, which are things assigned after registration. Also, the `displayStudent()` method is defined here. A method
`assignProf()` helps to assign a professor based on the subject of student.

#### Class ExamProfile:
Inherits Student class. Contains information if the student is eligible for penalty or grace marks, and
also the test scores of the student. Also, the `showScore()` method displays the score.

#### Interface Achievement:
Contains the marks that are to be rewarded or deducted as grace/penalty.

#### Class Result:
Inherits Examprofile class and implements Achievement. It has a constructor to initiate the class, as well as a method calculatedResult() which calculates the marks based on the conditions. Also, method displayResult() displays the final result of the student.
When a new object is initiated, the constructor assigns the values to the attributes, most of which are inherited from other classes. The method `calculatedResult()` uses control statements to calculate the final marks of the student based on the attributes. The method `displayResult()` uses inherited methods `assignProf()`, `displayStudent()`, `showScore()`, `calculatedResult()` to display the final result.

### Output:
![Output]([https://user-images.githubusercontent.com/76884959/172964002-3da7f82a-9cd9-4ef4-b0a0-e7e39ca80e03.png](https://github.com/Dark-knight-02/JAVA-PROJECT-MA-104-ASSIGNMENT/blob/main/output.png))


#### Note:
>For more info visit MA104.pdf
