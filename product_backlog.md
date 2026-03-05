# Summer 2026 Course Registration System – Initial Product Backlog
**Virginia Commonwealth University**  

---

## User Story #1: Search Available Courses  
**Priority:** High  

**User Story:**  
As a student, I want to search for available courses by semester, subject, and instructor, so that I can find classes that fit my academic plan and schedule.

**Description:**  
This feature will allow students to filter and view course offerings based on semester, department, course number, and instructor. The system must display course details including credit hours, meeting times, and seat availability. Success is achieved when students can quickly locate accurate and updated course information.

**Priority Justification:**  
This story is assigned High priority because searching for courses is highly important to the registration process. Without the ability to locate available classes, students cannot enroll. This functionality directly impacts student experience and is necessary for all other registration actions.

---

## User Story #2: Add Course to Schedule  
**Priority:** Medium  

**User Story:**  
As a student, I want to add a selected course to my schedule, so that I can enroll in classes required for my degree.

**Description:**  
This feature enables students to select a course and attempt enrollment. The system must verify prerequisites, check seat availability, and confirm successful registration. Success is achieved when the course is added to the student’s schedule and enrollment records are updated accurately.

**Priority Justification:**  
This story is ranked Medium because while enrollment functionality is highly valuable, it depends on foundational capabilities such as course search and account authentication. It is essential but builds upon other core system components.

---

## User Story #3: Student Login and Authentication  
**Priority:** High  

**User Story:**  
As a student, I want to log in to the course registration system securely, so that my personal information and enrollment records are protected. 

**Description:**  
This feature allows students to authenticate using a secure username and password. Functionality includes account creation, login validation, password recovery, and session management. Constraints include enforcing secure password standards and preventing unauthorized access. Success is achieved when students can reliably log in and access their accounts without security breaches.

**Priority Justification:**  
This story is ranked High because login and authentication are foundational to all student-facing functionality. Students cannot search for courses, enroll, or view their schedules without first accessing a secure account. It ensures data privacy, protects sensitive information, and enables other core features to function correctly, making it critical for the system’s overall operation.

---

## User Story #4: Drop a Registered Course  
**Priority:** Medium  

**User Story:**  
As a student, I want to drop a course I previously registered for, so that I can adjust my schedule if my plans change or if I cannot attend the course.

**Description:**  
This feature enables students to remove a course from their current schedule. Functionality includes updating enrollment records, freeing up seats for other students, and confirming the drop action. Constraints include adherence to university deadlines and preventing drops after the add/drop period. Success is achieved when the course is removed from the student’s schedule, enrollment numbers update correctly, and the system confirms the action.

**Priority Justification:**  
This story is ranked Medium because while the ability to drop courses is valuable for student flexibility, it builds on foundational features such as account authentication and enrollment functionality. It is important for managing course loads and maintaining accurate enrollment records but is not as critical as core login or enrollment capabilities.

---

## User Story #5: View Current Class Schedule  
**Priority:** Medium  

**User Story:**  
As a student, I want to view my current class schedule, so that I can plan my summer courses and avoid conflicts.

**Description:**  
This feature displays a student’s enrolled courses, including course name, section, instructor, meeting times, and modality. It allows easy navigation and printing of the schedule. Constraints include ensuring up-to-date enrollment data and preventing display of courses not officially registered. Success is achieved when students can view their complete, accurate schedule at any time.

**Priority Justification:**  
This story is ranked Medium because while viewing a schedule improves user experience and helps students manage their time, it depends on foundational capabilities like account login and course enrollment. It is essential for planning and conflict prevention but builds upon other core system components.

---

## User Stories #6: Validate Prequisite and Enrollments Eligibity 
**Priority:** High 

**User Story:**
As a student, I want to automatically verify that I have completed necessary foundational courses, so that I don't enroll in advanced technical or compliance training without the required prior knowledge.

**Description:**
This story includes the logic to cross-reference a user’s transcript against a course’s “prerequisite” field before allowing enrollment. It constraints users from bypassing requirements unless an admin override is applied. Success is defined as a 100% reduction in “accidental” enrollments in advanced courses by unqualified users.


**Priority Justification:**
This is a high priority because it ensures regulatory compliance and protects the bank from audit failures. By automating eligibility, the bank avoids the high operational cost of instructors teaching students who lack foundational knowledge. This feature is a critical technical dependency for accurate certification tracking and advanced reporting.


## User Stories #7: Waitlist for Full Courses
**Priority:** Medium

**User Story:**
As a student, I want to be put on a waitlist for a “Full” course, so that I can be automatically enrolled if a seat opens up or be notified of the next available session.

**Description:**
This functionality includes a First-In-First-Out (FIFO) queue for over-capacity courses and an automated notification trigger when a spot becomes available. A key constraint is that the waitlist must have a maximum capacity. Success looks like maintaining 100% seat utilization for all high-demand workshops 

**Priority Justification:**
This story is a medium priority as it optimizes resource utilization by ensuring no training seat go empty due to last-minute cancellations. While it significantly improves the employee experience and ROI for in-pesron sessions, it is not a “day-one” requirements for the system to function. It is best suited for a secondary release once core enrollment is stable.


## User Stories #8: Personalize Dashboard Layout
**Priority:** Low

**User Story:**
As a system user, I want to rearrange the widgets on my home dashboard, so that I can quickly access the information most relevant to my specific role.

**Description:**
This story includes “drag-and-drop” functionality for dashboard components and the ability to toggle specific data widgets on or off. A key constraint is that “Mandatory Notifications” cannot be hidden. Success is achieved when layouts persist across user sessions. 

**Priority Justification:**
Personlization is a low priority because it is “nice-to-have” UX improvement with not direct impact on core business logic or regulatory requirements. Since the feature is independent of the enrollment and grading engines, it carries no technical dependencies. It can be deferred to a later polishing phase without affecting the system’s primary goals. 


## User Stories #9: Receive Enrollment Confirmation Notification
**Priority:** Medium 

**User Story:**
As a student, I want to receive a confirmation notification after successfully enrolling in a class, so that I know my registration was processed correctly and I have proof of enrollment.

**Description:**
The story includes automatically sending an on-screen confirmation after a student successfully enrolls in a course. The notification will summarize key course details and only trigger once the enrollment is fully processed into the system. Success is achieved when students receive accurate confirmation immediately and registration related inquiries decrease. 

**Priority Justification:**
The story provides strong value by reassuring students during registration and reducing support requests to administrative staff. However, it does not block enrollment functionality and depends on the core registration system, placing it at Medium priority rather than High.


## User Stories #10: Export Class Schedule as PDF
**Priority:** Low

**User Story:**
As a student, I want to export my class schedule as a PDF, so that I can download, print, or share it for personal planning or documentation purposes. 

**Description:**
This story allows students to download a PDF version of their current class schedule in a printable format. The PDF must reflect real-time schedule data and work across all device types. Success is achieved by accurate and quick generation of a user-friendly, readable document. 

**Priority Justification:**
This feature improves convenience but does not impact core enrollment operations. It only really depends on completed schedule functionality and has no time sensitivity, therefore it is Low priority.


