# INTELCODE-INDIA-PRIVATE-LIMITED_Assigment



INTELCODE INDIA PRIVATE LIMITED












FULL-STACK DEVELOPER
CANDIDATES ASSIGNMENT







PRIVATE AND CONFIDENTIAL













Continue to next page

Congratulations!
You had been shortlisted as our competitive candidates for FULL STACK DEVELOPER position at INTELCODE INDIA PRIVATE LIMITED.
As for finalizing our most preferable candidates to join us as FULL STACK DEVELOPER, we would like to have a quick assignment for candidates to finish up. The assignment is on the next page.


Please fill up the forms below.



Candidate’s information:


Name	:  Gourav Pundir	

Identity No	:  	

Address	:





Contact number	:  	9149196959

Email address	:  	pundirgourav0@gmail.coom

Position	: FULL STACK DEVELOPER




Please proceed for the assignment after filling up your information above. You have 1 hour to answer the questions.
Thank you.

Section A: PHP Knowledge


Programming Languages:  Proficent with JavaScript.

Front-end Technologies: Basic Knowledge of css html and reactjs

Back-end Frameworks: Knowledge of Express framework.

Databases: knowledge of MongoDb and Mysql

Design Ability: A good sense of design and user experience and can create visually appealing and user-friendly websites.

Deployment and DevOps: such as Git.


2.Write a PHP code to create connection to the database?


























3.Which function is used in PHP to count the total number of rows returned by any query?




















4.How to create a session in PHP?













5.Write PHP statement to insert data into MySQL table.














Section B: Security and Technical Implementation

6.What is the advantage of Asynchronous JavaScript and XML (AJAX)?

1. The advantages of Asynchronous JavaScript and XML (AJAX) can be summarized as follows:

2. Dynamic updates: AJAX enables dynamic updates to web pages without requiring full page reloads.

3. Improved user experience: AJAX provides a smoother and more responsive user experience, allowing users to interact with the page more quickly and easily.

4. Faster page loads: AJAX reduces the amount of data transferred between the server and client, resulting in faster page loads.

5. Better performance: AJAX can improve the overall performance of a website, making it more efficient and responsive.


7.List the ways to improve your website load time and performance.

There are several ways to improve the load time and performance of your website:

1. Minimize HTTP Requests: Minimizing the number of HTTP requests that are made to the server can significantly reduce the load time of your website.
This can be achieved by using techniques such as combining files, using CSS sprites, and inline images.

2.Optimize Images: Large, high-resolution images can slow down your website. Optimize images by compressing them, reducing their size, 
and serving them in the appropriate format (e.g., JPEG for photographs, PNG for graphics).

3.Use a Content Delivery Network (CDN): A CDN can reduce the load time of your website by serving content from multiple servers around the world, 
reducing the distance that data has to travel.

4.Minimize the Use of Plugins: Too many plugins can slow down your website, as each plugin requires additional processing time and memory. 
Minimize the number of plugins you use, and ensure that they are optimized for performance.


8.What do you understand by RESTful Web Services?

RESTful Web Services:

1. Architecture style for building web services
2. Based on Representational State Transfer (REST) principles
3. Uses HTTP methods (GET, POST, PUT, DELETE)
4. Uses resource URIs to identify resources
5. Provides a scalable and flexible solution
6. Often used to build APIs and microservices
7. Enables communication and data exchange between applications.

9.How Application Programming Interfaces (APIs) integration works? Sketch by using a diagram.



10.What is software patch?

Software Patch:

1. Fixes or improves specific issues in software
2. Released by software vendors
3. Addresses bugs, security vulnerabilities, etc.
4. Can range in size from small to large
5. Delivered as standalone package or update
6. Easy to install
7. Common practice in software industry.


11.Why patches are important?

Reasons why patches are important:

1. Protect systems from security threats
2. Protect sensitive data from theft
3. Fix bugs and improve software functionality
4. Ensure software compatibility with other programs and systems
5. Provide performance enhancements and other improvements.


Section 3: MySQL

Table: student

student_id	student_name	university_id	matric_no
1	Muhammad Ali	1	A13CS0080
2	Ahmad bin Abu	3	B1110012
3	Farhan Ramli	5	A13KE1123
4	Chong Wei	2	C1234QW1
5	Hanis Zalikha	5	A14KE2234

Table: university

university_id	university_name
1	Massachusetts Institute of Technology (MIT)
2	University of Cambridge
3	Stanford University
4	Harvard University
5	University of Oxford

12.Write SQL statement to display student name, university name and matric number.

Solution:

SELECT student.student_name, university.university_name, student.matric_no
FROM student
JOIN university
ON student.university_id = university.university_id;

This query will return a result set that shows the student name, university name, and matric number for each student. 
The join operation combines the data from the two tables based on the matching university_id values.

Abu Bakar	Harvard University	A11BD0090
Table 1.1
13.Based on student information in Table 1.1 above, please write SQL statement to insert student information in table student.

solution:
INSERT INTO student (student_name, university_id, matric_no)
VALUES ('Abu Bakar', (SELECT university_id FROM university WHERE university_name = 'Harvest University'), 'A11BD0090');

14.Muhammad Ali moved from MIT to Harvard University, write SQL statement to update Ali’s
information in table student.

solution:
UPDATE student
SET university_id = (SELECT university_id FROM university WHERE university_name = 'Harvard University'), student_name = 'Muhammad Ali'
WHERE student_name = 'Muhammad Ali' AND university_id = (SELECT university_id FROM university WHERE university_name = 'Massachusetts Institute of Technology (MIT)');

university_name	total student
Massachusetts Institute of Technology (MIT)	1
University of Cambridge	1
Stanford University	1
Harvard University	0
University of Oxford	2
Table 1.2

15.Write SQL statement to display total student in every university as Table 1.2

Solution:

SELECT university.university_name, COUNT(student.student_id) AS total_student
FROM university
LEFT JOIN student
ON university.university_id = student.university_id
GROUP BY university.university_id;




- END OF ASSIGNMENT -
