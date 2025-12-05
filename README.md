# codingskills_1_Project
This is a simple command-line Student Portal System written in C.
It supports student login, admin login, and modules such as profile, attendance, marks, fees, and timetable.
It also includes password masking using * during input.

FEATURES

Login System

Login using roll number and password

Password characters appear as *

Locks after 3 incorrect attempts

Supports STUDENT and ADMIN roles

Student Features

View Profile

View Attendance

View Marks

View Fee Status

View Today’s Timetable (based on department)

Admin Features

Add Student

View All Students

Delete Student by ID

Update Student CGPA

REQUIRED DATA FILES

The program requires the following text files in the same folder:

credentials.txt
Format:
roll,password,ROLE
Example:
AP24110011210,student123,STUDENT
ADMIN001,admin123,ADMIN

students.txt
Format:
id,name,department,cgpa
Example:
10,John,CSE,8.50

attendance.txt
Format:
id,totalDays,presentDays
Example:
10,90,82

markss.txt
Format:
id,m1,m2,m3,m4,m5
Example:
10,85,78,90,72,88

fees.txt
Format:
id,totalFee,paidFee
Example:
10,50000,30000

timetable.txt
Format:
department,Day,Subject1,Subject2,Subject3
Example:
CSE,Monday,Maths,DSA,DBMS

COMPILATION

Linux / macOS:
gcc student_portal.c -o codingskills_1_Project

Windows (MinGW):
gcc student_portal.c -o codingskills_1_Project

RUNNING THE PROGRAM

./codingskills_1_Project

IMPORTANT NOTES

Passwords are stored in plain text. For real applications, use hashing.

Input uses scanf, so avoid very long values.

Student ID is derived from the last two digits of the roll number.

Timetable uses the system date to detect today’s day.

AUTHOR

Karthik
Student Developer
