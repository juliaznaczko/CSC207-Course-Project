General Description:
A student-matching website based on their courseloads to take courses together. A student creates an account with their student UofT email, then uploads their current courseload from acorn. Based on a certain score calculation algorithm, the user will see either users that are the closest matches to their courseload.
Additionally, the user can choose further filters for themselves (Gender, Year of Study, etc…) to find the most suitable match. The student will be able to send an invitation to their matches, and if the other student accepts it, they will be able to chat on the platform to discuss meeting plans.
Implementation Details:
User/Student:

A user will have the following in their profile:
Photo
(Initially a username, after matching full name is visible)
Year of Study
Program(s)
Gender/pronoun
Bio/About yourself 
Languages spoken
Website
Either accesses acorn or has a drop-down menu of course codes 
Potential drop-down menu of interests
Accessing acorn is quicker for the user however the drop down menu allows the student to choose which courses they want to be considered, allowing for better matches based on student needs.

Algorithm 

* Courses, Program, year- required fields, must enter at least one course and at least one program
* Courses and programs are implemented with Set to prevent doubles
* Maybe offer a slider so that user can adjust the weight of each section which are each represented by a different colour and all add up to 1, defaults for sections found below. (Ex: user can choose to discount the interests completely for the sake of calculation
* use static variables for the weight of each section, use the variable instead of the direct value to allow for change

  * 0.3 Program (min: 1, max: 3)
    * 0.25 Name of Program (Ex: Computer Science)
    * 0.05 Type (Ex: Major)
  * 0.3 Current Courses (min: 1, max: 6)
  * 0.2 Year
  * 0.1 Interests (max-5)
  * 0.1 Languages Spoken (max-2)

User uses drop-down menu to select each thing with a type option
Each item selected counts as *Weight of Section (1/total)* number of item entered in Section
* Example: Student A chooses 3 Courses (a,b,c), Student B chooses 2 courses (c,d). Discarding the other sections, for Student A, Student B is a 0.3(1/3) = 0.1 match. For Student B, Student A is a 0.3(1/2) = 0.15 match.

User Data for algorithm:
- {username: julia.znaczko, Year: 2, Programs: [Data Science - Specialist, French - Minor], Current Courses: [STA257, CSC207], Interests: [Dancing, Drawing], Languages Spoken: [English]}

When clicking on a recommended user, Data that gets accessed:
- {username: julia.znaczko, name: Julia Znaczko, bio: “Hi I’m Julia”, contactInfo: [instagram: @julia.znaco, discord: null, phoneNumber: null]}

What we need: 
- List of course codes
- List of programs 

Project Major Parts : 

1 ) Data / Data management 

2) User interaction 

3) Algorithm 

4 ) user interface 


First half : data and user interaction, UI diagram, algorithm outline

Second half : algorithm and user interface 
3 people per Part 














An application that reminds you to stand up every five minutes
Resume rater
App that compiles internships based on location
Gravity simulator 
Internet connection tester 
Money organization program 
University library availability program ( tells you how many available seats is a given library)
