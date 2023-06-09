# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

This project will serve people who create digital monthly calendars and want to make them more easily. My motivation to take on this project stems from the idea of professors and students using my DSL together. I imagine professors giving a text file that contains all important due dates for their class to their students written in my language. Since the text file will be written in my language, it can then be able to be passed through an application that reads the file and adds the items to a calendar. This would allow students to easily create a visual representation for all assignments that they have due over the course of the semester, instead of having to create their own manually or referring to a calendar created by the professor on the class website or syllabus.  

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

My idea will meet the needs of students and anyone who creates a digital calendar on their computer. As a student, at the beginning of each semester, I go through the syllabuses for each of my classes and create a calendar that contains due dates for all of my upcoming assignments. Since I learn and remember things visually, I like to create a monthly where I can see everything at once. Thus far, I have manually created a calendar in excel for each semester I have been in college. This process takes upwards of two hours and involves setting the dates for each school week, scraping each syllabus for assignment due dates, and determining what is worthy of putting on my calendar (some professors make this easier/more clear than others as they clearly outline what is due on their syllabus), and color coding assignments by class. 
  
If I can help myself, and others who face this problem, I would be able to create a long-term calendar by first initializing a desired length for their calendar and then by passing in a file with items they want to add. What makes my DSL unique and helpful is that it will allow users to easily add details when inputting their items instead of altering them manually afterward. These include:
  - Reoccurance: The user can specify if they want the item to reoccur by week, month, etc.
  - Color: the user can easily manipulate the color of the item by specifying it in the input
  - Bold/underline/italicizate
I will likely write two DSLs: one that handles entering events, and another that works with the look and feel of the program


### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

Since my domain is limited to creating a calendar, a DSL is appropriate as it will allow me to create a language of text inputs that can be translated into a visual output of a calendar. This will be a great opportunity for me to practice writing a DSL as I will need to determine how I want inputs to be structured and what types of parameters the inputs can include. It addresses the need because it will allow users to create a calendar based on text input which will hopefully save many people time. My DSL will hopefully serve as a useful tool to automate the tedious process of creating an online calendar one element at a time. The domain is niche yet widely used which is why I believe that a DSL is appropriate and needed.

### Why you?

_What excites you about this idea? How did you come up with it?_

I'm excited by this idea because it is something that I would actually use and I know other people who would benefit from it too. I came up with the idea after interviewing a CMC environmental science major, who told me about how they rely on their computer for scheduling their work. After thinking about what they said, I thought about how I interact with my computer in the same way and realized that I had a few pain points in this area. Currently, as a Google Calendar user, I have to manually input each event into the calendar which can become tedious when I have multiple similar events (study times) to enter at once. Also, Google calendar doesn't have a great full-month view which I like to use. I am excited to potentially create a solution to these pain points as I will use my project if it is built well. I find it extremely motivating to work on something that I will actually use. 

### Domain

_Describe the project's domain in five words._

Easy full-semester time management

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

The user would interact with the language by initially creating a calender by setting the start and end dates. Then they would have the ability to program events by specifying the day they want to edit and choosing to either add, remove or alter items that they want to schedule. The calendar would be viewed in months (that's how I view my time management) and would help students visualize and map out their semester. Programming would look like users editing, adding, and checking things off their calendars. The right way to interact with the problem domain would be to input items into the calendar as soon as one knows about them and cross them off once they are complete. Also, I want the user to be able to cross off entire days once they have passed or if there is a holiday ahead that requires no work. My DSL will hopefully be so easy to use that these tasks will take little time to do.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs it displays a calendar with the user's inputted items. The program interacts with the user by prompting them with the option to add, move, delete, or check off an item to their calendar. Errors might occur if there are two of the same item on the same day or if the day is in the past. They will be communicated to the user with a message after they input the request. In addition to that errors might occur if things such as dates, event types, or customization requests aren't entered with the correct syntax. These errors will be communicated to the user by displaying an error message and pointing out where the program got confused.

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to add/remove events, customize the text in the calendar, and block off days specified by the user.
I think it will be possible but harder to create the calendar interface and sync it to other services such as excel or google calendar.
It will likely be very difficult to add a handler for reoccurring items but it would be a feature that would make my DSL unique and particularly useful.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are quite a few DSLs in the calender domain, here are a few:
https://wiki.tcl-lang.org/page/Gregor%3A+A+DSL+for+building+semester+calendars
https://github.com/shannonjanehogan/google-calendar-dsl
https://github.com/JettChenT/timeblok

I think that these DSLs adequately address the need of everyone who created them and provide a way to auto-populate a calender from text which is my end goal. I found the first link particularly relevant to my project as it was created by a professor at George Washington University for semester-long scheduling. This idea directly reflects my desire to make my DSL targeted toward students. Also, the other two GitHub links seemed like personal projects that people created to create a calendar using their desired syntax. These projects will be great resources for me to look through and gain inspiration. However, I think that it is important for me to write my own, even though others exist because I will be the primary user and I want the syntax to meet my specific wants and needs. Also, I am hoping to have my DSL auto-populate a google sheet which the existing calendars do not.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing complicated semantics that doesn't require a lot
of language design)?_

My initial thought was I would say %50/%50 but after further thought, I believe it to be %75/%25. This is based on the fact that I will be writing two DSLs which should give me plenty of opportunity to directly engage in language design. However, this is tailored to the scope of this class assignment, if I wanted to I could add a lot of features that would require me to work with the systems aspects. 

### Scope

_How big an idea is this? How ambitious is this project?_

I believe that this idea is very doable as a project over the remaining time that we have this semester. There is a chance that this project takes me slightly longer than I am currently expecting it to take but this is ok. Since I will have to start by writing the internal DSLs for my program, and then get the application up and running, I will be able to use this class as a resource to write my DSLs. After that, I can finish the systems aspects of the project on my own time or during the end of the semester if time permits.

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

This is a good idea for a project because it is something I would use, and often. It would allow me to create my DSL and create a product I can hopefully share with others too. It might not be a good idea because it will require me to work a decent amount on the systems side of things which is not the main focus of this class. Also, many people are comfortable and used to using existing scheduling systems. However, I believe the pros of this project far outweigh the cons as I am passionate about working on it, I get the chance to write not one but two DSLs, and it would allow me to practice writing a functional application which is something I've been wanting to gain more experience doing.
