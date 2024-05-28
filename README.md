  ### Functional Requirements for Student Academic Records Database

#### 1. **User Management**
   - **Add Student**: The system shall allow administrators to add new student records including personal details (e.g., full name, faculty, specialization, degree, form of study, enrollment year, photo).
   - **Update Student**: The system shall allow administrators to update existing student records.
   - **Delete Student**: The system shall allow administrators to delete student records.
   - **View Student**: The system shall allow administrators to view student records.

#### 2. **Subject Management**
   - **Add Subject**: The system shall allow administrators to add new subjects including details such as subject name, credits, number of exams, hours, credit date, exam date, and examiner.
   - **Update Subject**: The system shall allow administrators to update existing subject records.
   - **Delete Subject**: The system shall allow administrators to delete subject records.
   - **View Subject**: The system shall allow administrators to view subject records.

#### 3. **Professor Management**
   - **Add Professor**: The system shall allow administrators to add new professor records including personal details (e.g., professor name, photo).
   - **Update Professor**: The system shall allow administrators to update existing professor records.
   - **Delete Professor**: The system shall allow administrators to delete professor records.
   - **View Professor**: The system shall allow administrators to view professor records.

#### 4. **Academic Book Management**
   - **Add Academic Book Entry**: The system shall allow administrators to add new academic book entries that link students to their subjects, practices, projects, professors, and grades.
   - **Update Academic Book Entry**: The system shall allow administrators to update existing academic book entries.
   - **Delete Academic Book Entry**: The system shall allow administrators to delete academic book entries.
   - **View Academic Book Entry**: The system shall allow administrators to view academic book entries.

#### 5. **Practice Management**
   - **Add Practice**: The system shall allow administrators to add new practice records including details such as practice name, duration in weeks, place, supervisor, and mark.
   - **Update Practice**: The system shall allow administrators to update existing practice records.
   - **Delete Practice**: The system shall allow administrators to delete practice records.
   - **View Practice**: The system shall allow administrators to view practice records.

#### 6. **Diploma Project Management**
   - **Add Diploma Project**: The system shall allow administrators to add new diploma project records including details such as type of project, project theme, submission date, defense date, supervisor, and mark.
   - **Update Diploma Project**: The system shall allow administrators to update existing diploma project records.
   - **Delete Diploma Project**: The system shall allow administrators to delete diploma project records.
   - **View Diploma Project**: The system shall allow administrators to view diploma project records.

#### 7. **Reporting and Analytics**
   - **Generate Student Report**: The system shall allow administrators to generate detailed reports for individual students, including academic performance and practice and project details.
   - **Generate Subject Report**: The system shall allow administrators to generate reports on subjects, including student performance across different subjects.
   - **Generate Professor Report**: The system shall allow administrators to generate reports on professors, including their involvement in different subjects, practices, and diploma projects.
   - **Generate Practice Report**: The system shall allow administrators to generate reports on student practices.
   - **Generate Diploma Project Report**: The system shall allow administrators to generate reports on diploma projects, including submission and defense dates, supervisors, and marks.

#### 8. **Search and Filter**
   - **Search Students**: The system shall allow administrators to search for students using various criteria (e.g., name, faculty, specialization).
   - **Search Subjects**: The system shall allow administrators to search for subjects using various criteria (e.g., subject name, examiner).
   - **Search Professors**: The system shall allow administrators to search for professors using various criteria (e.g., name).
   - **Search Practices**: The system shall allow administrators to search for practices using various criteria (e.g., student, place, supervisor).
   - **Search Diploma Projects**: The system shall allow administrators to search for diploma projects using various criteria (e.g., student, supervisor, project theme).

#### 9. **Data Validation and Integrity**
   - **Ensure Data Consistency**: The system shall ensure data consistency by validating that linked records (e.g., student, subject, professor, practice, project) exist before creating academic book entries.
   - **Unique Constraints**: The system shall enforce unique constraints on identifiers (e.g., student ID, subject ID, professor ID, practice ID, project ID).

#### 10. **User Roles and Permissions**
   - **Admin Role**: The system shall provide an admin role with full permissions to manage all aspects of the database.
   - **Viewer Role**: The system shall provide a viewer role with permissions to view records but not modify them.

These requirements should provide a comprehensive framework for the functionalities needed in a student academic records database system.

### System Behaviors for Student Academic Records Database

#### 1. **User Authentication and Authorization**
   - **Login**: The system shall prompt users to enter their credentials to log in.
   - **Authentication**: The system shall verify the entered credentials against stored user information.
   - **Authorization**: The system shall grant or deny access to specific functionalities based on user roles (e.g., Admin, Viewer).

#### 2. **Data Entry and Management**
   - **Student Data Entry**: When an administrator inputs new student data, the system shall validate the fields (e.g., ensuring mandatory fields are filled, data types are correct) before saving the record to the database.
   - **Subject Data Entry**: The system shall allow administrators to enter new subject information, ensuring all required fields are completed.
   - **Professor Data Entry**: The system shall enable administrators to add professor details, including name and photo.
   - **Academic Book Entry**: The system shall link students with their academic records, including subjects, practices, and projects.
   - **Practice Data Entry**: Administrators shall input details of student practices, including duration and supervision.
   - **Diploma Project Data Entry**: The system shall record details of student diploma projects, including themes and submission dates.

#### 3. **Data Updates**
   - **Edit Student Records**: When updating a student record, the system shall retrieve the existing data, allow modifications, and then save the updated information back to the database.
   - **Edit Subject Records**: The system shall allow updates to subject details, ensuring data integrity during the process.
   - **Edit Professor Records**: The system shall permit updates to professor information, including photo changes.
   - **Edit Academic Book Entries**: The system shall enable changes to academic book records, ensuring all linked records are updated accordingly.
   - **Edit Practice Records**: The system shall facilitate updates to practice details, ensuring consistency across related data.
   - **Edit Diploma Project Records**: The system shall allow administrators to update project details, including changes to supervisors or themes.

#### 4. **Data Deletion**
   - **Delete Student Records**: The system shall allow the deletion of student records, ensuring all associated data (e.g., academic books) is appropriately handled.
   - **Delete Subject Records**: The system shall permit the removal of subjects from the database.
   - **Delete Professor Records**: The system shall allow administrators to delete professor records, ensuring no orphan records are left in the academic book.
   - **Delete Academic Book Entries**: The system shall enable the deletion of specific academic book entries.
   - **Delete Practice Records**: The system shall permit the deletion of practice records from the database.
   - **Delete Diploma Project Records**: The system shall allow the removal of diploma project entries.

#### 5. **Data Retrieval and Viewing**
   - **View Student Details**: The system shall provide a detailed view of student information, including personal details and academic records.
   - **View Subject Information**: The system shall display detailed subject information, including exam schedules and credits.
   - **View Professor Information**: The system shall provide access to professor details, including associated subjects and practices.
   - **View Academic Book Entries**: The system shall display comprehensive academic records for each student.
   - **View Practice Records**: The system shall present detailed information about student practices.
   - **View Diploma Project Records**: The system shall show detailed information about student diploma projects, including themes and defense dates.

#### 6. **Search Functionality**
   - **Search Students**: The system shall allow users to search for students using various filters (e.g., name, faculty, specialization).
   - **Search Subjects**: The system shall enable searching for subjects based on criteria such as subject name and examiner.
   - **Search Professors**: The system shall allow users to search for professors using name or associated subjects.
   - **Search Practices**: The system shall provide search capabilities for practices based on student, place, or supervisor.
   - **Search Diploma Projects**: The system shall enable searches for diploma projects using criteria like student name, supervisor, or project theme.

#### 7. **Reporting and Analytics**
   - **Generate Reports**: The system shall generate various reports (e.g., student performance, subject summaries, professor involvement) based on selected criteria.
   - **Export Reports**: The system shall allow users to export reports in common formats (e.g., PDF, Excel).

#### 8. **Data Validation**
   - **Validate Input Data**: The system shall validate all input data for correct formats, mandatory fields, and logical consistency before saving to the database.
   - **Unique Identifier Checks**: The system shall ensure that identifiers (e.g., StudentID, SubjectID, ProfessorID) are unique within the database.

#### 9. **System Maintenance**
   - **Backup Data**: The system shall regularly back up the database to prevent data loss.
   - **Restore Data**: The system shall allow data restoration from backups in case of data corruption or loss.
   - **Database Optimization**: The system shall periodically optimize the database for performance improvements.

These behaviors will guide the system's interactions and ensure it meets the functional requirements efficiently and reliably.

## REST API Endpoints for Student Academic Records Database

### Students
- **GET /students**: Retrieve a list of all students.
- **GET /students/{id}**: Retrieve a specific student by ID.
- **POST /students**: Create a new student.
- **PUT /students/{id}**: Update a student by ID.
- **DELETE /students/{id}**: Delete a student by ID.

### Subjects
- **GET /subjects**: Retrieve a list of all subjects.
- **GET /subjects/{id}**: Retrieve a specific subject by ID.
- **POST /subjects**: Create a new subject.
- **PUT /subjects/{id}**: Update a subject by ID.
- **DELETE /subjects/{id}**: Delete a subject by ID.

### Professors
- **GET /professors**: Retrieve a list of all professors.
- **GET /professors/{id}**: Retrieve a specific professor by ID.
- **POST /professors**: Create a new professor.
- **PUT /professors/{id}**: Update a professor by ID.
- **DELETE /professors/{id}**: Delete a professor by ID.

### Academic Books
- **GET /academicbooks**: Retrieve a list of all academic books.
- **GET /academicbooks/{id}**: Retrieve a specific academic book by ID.
- **POST /academicbooks**: Create a new academic book entry.
- **PUT /academicbooks/{id}**: Update an academic book entry by ID.
- **DELETE /academicbooks/{id}**: Delete an academic book entry by ID.

### Practices
- **GET /practices**: Retrieve a list of all practices.
- **GET /practices/{id}**: Retrieve a specific practice by ID.
- **POST /practices**: Create a new practice.
- **PUT /practices/{id}**: Update a practice by ID.
- **DELETE /practices/{id}**: Delete a practice by ID.

### Diploma Projects
- **GET /diplomaprojects**: Retrieve a list of all diploma projects.
- **GET /diplomaprojects/{id}**: Retrieve a specific diploma project by ID.
- **POST /diplomaprojects**: Create a new diploma project.
- **PUT /diplomaprojects/{id}**: Update a diploma project by ID.
- **DELETE /diplomaprojects/{id}**: Delete a diploma project by ID.
