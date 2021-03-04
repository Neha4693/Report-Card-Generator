Report Card Generator

This script was written as part of a coding challenge to generate a text file containing the “report
card” of all students

Summary of Assigment:
Inputs
You will be given four files as an input to your program. The description of each file is
written below. Here is a compressed folder with a simple example input.
courses.csv
This file contains the courses that a student takes. Each course has a unique id , a
name , and a teacher .
students.csv
This file contains all existing students in the database. Each student has a unique id ,
and a name .
tests.csv
This file contains all the tests for each course in the courses.csv file. The file has three
columns:
● id: the test’s unique id
● course_id: the course id that this test belongs to
● weight: how much of the student’s final grade the test is worth. For example, if a
test is worth 50, that means that this test is worth 50% of the final grade for this
course.
The sum of all the weights of all tests in a particular course should add up to 100. You
are allowed to throw errors in your report card generation script if this is not the case.
marks.csv
This file contains all the mark the student received for all the tests that they have
written.
The file has three columns:
● test_id: the test’s id
● student_id: the student’s id
● mark : The percentage grade the student received for the test (out of 100)
Note: Not all students are enrolled in all courses – this can be determined by the marks
that they receive. All students should have completed (taken every test for) each course
they are enrolled in. If a student takes no test in a course, then this student is not
enrolled in that course. If there are students that have not completed a course, you can
throw an error in your report card generation script.
Output
Given the example input, here is the text file that your program should generate . Your
goal is to write a program that generates a text file with the following characteristics:
● All student report cards – the order of the students should be based on student
id
Here is an example report card:

Student Id: 1, name: A
Total Average:      72.03%
    Course: Biology, Teacher: Mr. D
    Final Grade:    90.10%
    Course: History, Teacher: Mrs. P
    Final Grade:    51.80%
    Course: Math, Teacher: Mrs. C
    Final Grade:    74.20%

    
● The first line should contain the student id and the student’s name
● The second line is the average of all the courses the student is enrolled in
● Below that, a listing of all courses and the student’s grade in each course (this
will be determined by the mark they get in each test, and how much each test is
worth)
● The courses are ordered by course id


Deployment:

Open the program in a Python-supported editor and run the file in a Python interpreter.

Run the function report_card_generator with the parameter being the
name of the courses csv file, students csv file, tests csv file, marks csv file.

Sample function call;

report_card_generator('courses.csv', 'students.csv', 'tests.csv', 'marks.csv')

*Notes
- The 4 csv files must be in the same directory as the program file.


