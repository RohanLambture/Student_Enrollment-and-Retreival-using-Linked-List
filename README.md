Problem: Student Management System

You are tasked with implementing a Student Management System that can organize student records based on various entities such as departments, courses, hostels, and clubs. The system should allow adding and deleting students from these entities efficiently.

Class Definitions:

1.StudentRecord Class:
   - Represents a student record with attributes `studentName` and `rollNumber`.
   - Provides methods to get and set these attributes.

2. Node Class
   - Represents a node in a linked list with attributes `next` (points to the next node) and `element` (points to a `StudentRecord`).
   - Provides methods to get and set these attributes.

3.Entity Class
   - Represents an entity (e.g., department, course) with attributes `name` and `iterator` (points to the head of a linked list).
   - Provides methods to get and set these attributes.

4.LinkedList Class
   - Inherits from `Entity`.
   - Contains methods to add and delete students efficiently from the linked list based on student name.
   - It also contains a method to add students to the system, considering various entities.

Functions:

1.add_theEntity(string Entity, StudentRecord S1)
   - Adds a student to the specified entity. If the entity does not exist, it creates a new entity and adds the student to it.

2.read_input_file(string file_path)
   - Reads student information from a file (`file_path`) and populates the system.
   - It skips lines with headers like "Name" or "Name."
   - For each student, it adds the student to the overall student list and various entities based on the information provided.

Main Functionality:

1.Adding Students:
   - Students can be added to the system by reading information from a file using `read_input_file`.
   - The system automatically adds students to different entities such as departments, courses, hostels, and clubs.

2.Deleting Students:
   - Students can be deleted from the system by name using the `delete_student` method in the `LinkedList` class.

3.Checking Student Existence:
   - The system should efficiently check whether a student with a given roll number already exists before adding a new student.

4.Displaying Students in an Entity:
   - The system should allow displaying the list of students in a particular entity (e.g., a department or course).

Instructions:

- Implement the classes and functions as described above.
- Test the system by adding students from a sample file.
- Implement a user interface or a set of test cases to demonstrate the functionality of adding and deleting students.
