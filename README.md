Backend: API FOR MENTOR AND STUDENT ASSIGNING 

  1. Overview :

       -  The backend for this project is developed using Node.js and Express, with MongoDB as the database.
       -  It includes APIs to manage mentors and students, as well as to handle their assignments.

  3. APIs Overview :
    
       -  Create Mentor API
            
            Method: POST /api/mentors
          
            Description: Adds a new mentor to the system.

       -  Create Student API :

            Method: POST /api/students
          
            Description: Adds a new student to the system.

       -  Assign Students to Mentor API
            
            Method: POST /api/mentors/:mentorId/assign
          
            Description: Assigns multiple students to a mentor. Students already assigned to a mentor won’t appear in the list.

       -  Change Mentor for a Student API

            Method: POST /api/students/:studentId/change-mentor
          
            Description: Reassigns a student to a new mentor.

       -  Get Students for a Mentor API
          
            Method: GET /api/mentors/:mentorId/students
          
            Description: Retrieves all students assigned to a specific mentor.

       -  Get Previous Mentors for a Student API

            Method: GET /api/students/:studentId/previous-mentors
          
            Description: Retrieves the history of mentors for a particular student.


  4. Backend Setup Process :

       -  Create an Express server : Use Express to handle HTTP requests and define routes.

       -  Connect to MongoDB : Use Mongoose to define schemas for mentors and students.

       -  Set up routes and controllers : Create separate routes for mentors and students. Assign business logic in controllers and services.

       -  Handle Errors : Implement error-handling middleware to handle database errors or validation issues.

       -  Start the server : Use app.listen() to start the server at a specific port (e.g., 5000).

