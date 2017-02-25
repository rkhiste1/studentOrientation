CS542 Design Patterns
Fall 2016
PROJECT Assignment 3 README FILE

Due Date: Friday, October 28, 2016
Submission Date: Friday, October 28, 2016
Grace Period Used This Project: 0 Days
Grace Period Remaining: 0 Days
Author(s): Rasika Makarand Khiste, Balakrishna Lellapalli
e-mail(s): rkhiste1@binghamton.edu, blellap1@binghamton.edu


PURPOSE:

[
  The purpose of this assignment is to apply design patterns and
  principles to develop a tool for student orientation program.
]

PERCENT COMPLETE:

[
  We believe we have completed 100% of this project.
]

PARTS THAT ARE NOT COMPLETE:

[
  None
]

BUGS:

[
  None
]

FILES:

[
  Included with this project are below files:

  1. Driver.java: Main class file that takes arguments, validate them, and calls methods of other classes
  2. CarbonFootprint.java: Abstract class for CarbonFootprint.
  3. CarbonFootprintCO2.java: Class that extends CarbonFootprint measured in CO2 tons
  4. Cost.java: Abstract class for cost.
  5. CostDollars.java: Class that extends cost measured in dollars.
  6. Duration.java: Abstract class for Duration.
  7. DurationMinutes.java: Class that extends duration measured in minutes.
  8. Efforts.java: Abstract class for efforts.
  9. EffortsCalories.java: Class that extends efforts measured in calories
  10. BookStore.java: Abstract class for buying books activity.
  11. BookStoreFactory.java: Factory that create objects for bookstore options
  12. BookStoreOptions.java: Enum for bookstore options.
  13. MandoBooks.java: Class for Mando bookstore that extends bookstore
  14. UniversityBookStore.java: Class for University bookstore that extends bookstore
  15. BusRide.java: Class for Bus ride that extends campus tour
  16. CampusTour.java: Abstract class for campus tour activity.
  17. CampusTourFactory.java: Factory that create objects for campus tour options
  18. CampusTourOptions.java: Enum for campus tour options
  19. OnFoot.java: Class for on foot campus tour that extends campus tour
  20. CourseRegistration.java: Abstract class for course registration activity
  21. CourseRegistrationFactory.java: Factory that create objects for course registration options
  22. CourseRegistrationOptions: Enum for Course registration options
  23. RegistrarOffice.java: Class for registration via registrar office that extends CourseRegistration
  24. RegistrationSystem.java: Class for registration via registration system that extends CourseRegistration
  25. AdministratorOffice.java: Class for selecting dorm via administrator's office that extends Dorm
  26. Dorm.java: Abstract class for dorm selection activity
  27. DormFactory.java: Factory that create objects for dorm options.
  28. DormOptions: Enum for dorm options.
  29. OnlineContext.java: Class for selecting dorm via online contest that extends Dorm
  30. IStudentOrientationPlanner.java: Interface for student orientation plan
  31. IWorkshop.java: Interface for workshop of builder
  32. StudentOrientationPlanner.java: Class that generates student orientation planner
  33. Workshop.java: Class that builds orientation checklist throught different activities.
  34. Results.java: Class responsible for storing and displaying result
  35. StdoutDisplayInterface.java: Interface to display result on standard output screen
  36. Logger.java: Class to write message to standard out depending on DEBUG_VALUE
  37. build.xml: file responsible to build, compile, compress and run the project
  38. README.txt: The file you are currently reading
  
]

SAMPLE OUTPUT:

[

balakrishna@balakrishna-XPS-13-9343:~/Documents/lellapalli_balakrishna_khiste_rasika/studentOrientation$ ant -buildfile build.xml run
Buildfile: /home/balakrishna/Documents/lellapalli_balakrishna_khiste_rasika/studentOrientation/build.xml

jar:
    [mkdir] Created dir: /home/balakrishna/Documents/lellapalli_balakrishna_khiste_rasika/BUILD/jar
      [jar] Building jar: /home/balakrishna/Documents/lellapalli_balakrishna_khiste_rasika/BUILD/jar/studentOrientation.jar

run:
     [java] 
     [java] ______ StudentOrientationPlanner ______  
     [java] BookStore : MandoBooks [Cost = $525.0, Carbon Footprint = 10.0CO2, Duration = 200.0minutes, Efforts = 50.0calories]
     [java] CampusTour : BusRide [Cost = $2.0, Carbon Footprint = 50.0CO2, Duration = 120.0minutes, Efforts = 50.0calories]
     [java] Course : RegistrationSystem [Cost = $10000.0, Carbon Footprint = 10.0CO2, Duration = 10.0minutes, Efforts = 15.0calories]
     [java] Dorm : OnlineContext [Cost = $20400.0, Carbon Footprint = 10.0CO2, Duration = 30.0minutes, Efforts = 50.0calories]
     [java] 
     [java] Total Cost = 30927.0, Total CarbonFootPrint = 80.0, Total Duration = 360.0, Total Efforts = 165.0

BUILD SUCCESSFUL
Total time: 0 seconds

]

TO COMPILE (While in project directory):

[
  ant -buildfile build.xml all
]

TO RUN (While in project directory):

[
  ant -buildfile build.xml run
]

CHOICE OF DATA STRUCTURES / DESIGN PATTERN (s):

[
 1. Builder Pattern, Used to construct different activities (Book Store, Campus Tour, Course Registration, Selecting Dorm)
 2. Simple factory, Used for creating object based on user preference 
    (Example: Object for University Book Store/ Mando Book store, Object for Bus Ride / Walk, Object for online Course Registeration/ Registrar office etc)
]

EXTRA CREDIT:

[
  N/A
]


BIBLIOGRAPHY:

This serves as evidence that we are in no way intending Academic Dishonesty.

[
  Head First Design Patterns by O'Reilly Media
]

ACKNOWLEDGEMENT:

[
  
]
