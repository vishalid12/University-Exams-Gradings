University Exams & Grading System - Java Assignment II

Name: Vishali D
Roll No: 717825I361
Department: B.Tech AIDS (Section C)
Subject: Java Programming (23CSR306)
Specification: 32 - University Exams & Grading

Problem Statement (As per Assignment II)

Design and implement a Java console application for a University Exams & Grading system that manages courses, students, assessments, exam schedules, marks, grades and transcripts. The application should demonstrate object-oriented principles and maintain consistent evaluation rules.

Requirements
Menu Display: Add Course, Add Student, Create Assessment, Schedule Exam, Record Marks, Publish Grades, Generate Transcript, Exit.
Class Requirements: Course, Student, Assessment, ExamSchedule, MarkEntry, Grade, Transcript.
Business Rules:
Students can be evaluated only for registered courses.
Marks aggregation follows configured weightages across assessments (weightages of a course must total 100).
Grades are derived from total marks using a defined grading policy.
Transcripts include course list, grades, and GPA/CGPA calculations.
Resits or improvements follow eligibility rules and update records.
Validation: Handles invalid IDs, duplicate entries, invalid credits/weightage, marks outside 0-100 and non-numeric input without crashing.
Expected Output: Grade sheet per course and student, transcript with GPA/CGPA, and assessment-wise analytics (counts, averages).
Grading Policy
Total Marks	Grade	Points
90 and above	O	10
80 - 89	A+	9
70 - 79	A	8
60 - 69	B+	7
50 - 59	B	6
40 - 49	C	5
Below 40	F	0

GPA / CGPA = sum of (grade points x credits) / sum of credits.
Resit / improvement: below 40 = RESIT, 40 to below 90 = IMPROVEMENT, 90 and above = none needed.

Project Structure
UniversityGradingSystem/
└── src/
    ├── CourseStudent.java            # Course, Student, Assessment, ExamSchedule,
    │                                 # MarkEntry, Grade, Transcript classes
    ├── UniversityService.java        # Business rules and report generation
    └── UniversityGradingSystem.java  # main() - menu-driven interface
Menu
===== UNIVERSITY EXAMS & GRADING SYSTEM =====
1. Add Course
2. Add Student
3. Register Student for Course
4. Create Assessment
5. Schedule Exam
6. Record Marks
7. Publish Grades
8. Show Grade Sheet
9. Generate Transcript
10. Assessment Analytics
11. Resit / Improvement Eligibility
12. View Exam Schedule
0. Exit
How to Compile and Run (Eclipse IDE)
File > New > Java Project > UniversityGradingSystem
Copy CourseStudent.java, UniversityService.java and UniversityGradingSystem.java into src
Right-click UniversityGradingSystem.java > Run As > Java Application

Requires JDK 8 or later.

Command line (optional):

bash
javac *.java
java UniversityGradingSystem
Suggested Order of Use

Add Course > Add Student > Register Student for Course > Create Assessment (weightages total 100) > Record Marks (all assessments) > Publish Grades > Show Grade Sheet / Generate Transcript / Assessment Analytics

Execution Output
Menu display
Validation / error-handling examples
Course added, students added, registration, assessment creation, exam scheduling, marks recorded, grades published
Grade sheet per course
Transcript with GPA/CGPA, assessment analytics, exam schedule, resit / improvement eligibility

(Screenshots are available in the screenshots/ folder.)







































Developed by Vishali D - 717825I361 - B.Tech AIDS



DOCX# University-Exams-Gradings
