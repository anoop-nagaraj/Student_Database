# Student_Database
A C++ student database application that manages courses, students and enrollments, supports file persistence, and can import test data from a network service using JSON.

#Requirements

| Req-Id | Description                                                                                                         |
| ------ | ------------------------------------------------------------------------------------------------------------------- |
| NFR1   | The system shall be implemented in modern C++ using object-oriented design.                                         |
| NFR2   | Classes shall be immutable where possible and avoid unnecessary setters.                                            |
| NFR3   | The system shall provide a console based user interface for testing and interaction.                                |
| NFR4   | All data shall be stored persistently in a single semicolon separated file.                                         |
| NFR5   | The system shall restore a consistent state after loading, including correct continuation of generated student IDs. |
| NFR6   | Network communication and JSON parsing shall use the Poco library.                                                  |
| FR1    | The system shall implement a student database managing students, courses and enrollments.                           |
| FR2    | A unique matriculation number shall be generated automatically when creating a student.                             |
| FR3    | The user shall be able to add and list courses.                                                                     |
| FR4    | The user shall be able to create students including address information.                                            |
| FR5    | The user shall be able to add enrollments and assign or remove grades.                                              |
| FR6    | The user shall be able to search students by name substring and print full student information.                     |
| FR7    | The user shall be able to update student data while keeping the matriculation number fixed.                         |
| FR8    | Updating an address shall create a new address object instead of modifying the existing one.                        |
| FR9    | The system shall write all database content to file in the order: courses, students, enrollments.                   |
| FR10   | The system shall load the database from file and reconstruct all objects completely.                                |
| FR11   | The system shall connect to a remote server and request generated user data via socket stream.                      |
| FR12   | Received JSON data shall be parsed and converted into student records.                                              |
| FR13   | The user shall be able to import multiple generated students in one operation.                                      |
| FR14   | The system shall terminate the server connection cleanly after data retrieval.                                      |

![System Diagram](images/Student_DB.PNG)
