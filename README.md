# Computer Science Portfolio

This will be a portfolio of assignments and projects completed during my time at Westminster University(WU) and will include reflections and information about the assingments and projects that I would like to show off.

## [minijava](https://github.com/PapaZ810/minijava2)

  Minijava was a project in the compilers class at WU that had the students design and implement the front end of a compiler to take minijava code and convert it into Java virtual machine assembly so that a different program, jasmin, could convert it into a .class file. This .class file could then easily be run and the output from the program could be seen. I had a lot of fun with this project and learning about compilers in general, but it did require a lot of work to create. The project was broken up over the last two months of the semester, with the first two getting the basics down on how parsing, lexing and adding semantic actions worked both in Java and how we were going to write them for our project. Overall, I enjoyed seeing the incremental progress of putting this compiler together, getting more and more of it working. It was really great when I could first write a normal looking Java program and get it to compile with no errors. Having to figure out precisely how jasmin wanted the assembly code and implementing that into the generator was difficult but extremely rewarding. 

![A picture of the code required to cast integers to doubles and vice versa as well as from numbers to Strings](/Cast.png)

A picture of the code required to cast integers to doubles and vice versa as well as from numbers to Strings. The full extent of the code is linked in the section header.

## [JPEG Image Compression Script](https://github.com/PapaZ810/ImageCompression)

  This project started off as a final project for the Linear Algebra class at WU but evolved over the past couple of years to be much more streamlined in code style. Most of the work that I put into it was to make it faster, as it originally took over a minute to compress a 3.5MB file down to 800KB. I didn't have time to make it much faster and considered the task of multithreading the script to be quite daunting at the time, but after I presented my work to the class I gained a renewed energy to work on it that unfortunately didn't get very far. After that, I left it for over a year while I focused on other classwork, and in the Fall of 2023 I came back to it, with more experience and ideas for how to complete this. The first step was to see if there was any way to make my code any cleaner. In the first version there were a lot of nested for loops and I was curious if there were any ways to manipulate the arrays in place. And, of course, there were! Using these optimizations I was able to significantly improve the quality of the code, going from someone who only knew Java to a proper programmer. My main idea for making the program faster was to multithread it, using multiple different cores on the device to speed up the lengthy operations I was doing on the images. But after a lot of work on converting the script to use four threads, the script was slower to complete on the same image. I then made two more branches that used two and eight threads but they were still slower. I made a massive breakthrough when I learned about vectorized array operations, turning one of the last nested for loop functions into just two lines. Not only did this improve the look of the code, but it made the script run much faster, going from over a minute to compress that previously mentioned 3.5MB file to just 6 seconds. I still have some bugs to iron out, most notably that the Fourier conversion doesn't really work and it's the main part of the compression. 

![A picture showing the difference between the non-compressed picture and the compressed picture.](/Windows.png)

![Another picture showing the difference between the non-compressed picture and the compressed picture.](/House.png)

Here are a couple of examples of the results of the script. Full code and all branches linked in the section header.

## [ZenSpelling](https://github.com/westmini-software-engineering-2024sp/ZenSpelling)

  ZenSpelling was a project myself and a few classmates completed as part of our class work in Software Engineering CMPT 322. It's a web-based spelling game for 1st-5th grade students to improve their spelling skills by building a garden. The game was built in Django using JQuery to transfer data to the frontend and p5.js to draw the canvas that holds the tiles on the game board. Students can track their progress in the game throught the profile screen and they can earn medals through exceptional gameplay. The game tracks the amount of time you played the game, how many questions you answer incorrectly and how many questions you answer correctly in a row and shows you all of those datapoints when you complete a game. It will also give the student medals based on those metrics after the game completes. It also saves the metrics to the database to be viewed by the student on the profile page and by the Teacher through the admin panel. I mainly worked on the database side of the game, but working in a team for this project got me to learn a lot about the AGILE process and about how effective communication can greatly improve productivity. 

---

Here are some pictures from the game!

![The login page](/ZenSpellingLogin.jpg)

### The login page where all students are required to log in to the app to log all metrics to the database.

![The profile page](/ZenSpellingProfile.jpg)

### The profile page shows all of the metrics for the students so that they can track their progress. It also has a section for a planned feature that we never got to, saving the gardens from students' games to their profile. We had planned it for a future release but never got to it.

![The game setup page](/Setup.jpg)

### The game setup page allows the student to customize their game how they want. The page offers different multiple different game board sizes and support for question sets. Question sets are a way for teachers to customize which questions the student receives to better augment their learning. It was also served as a way for students to focus on their worst words to spell them better, but that was also not automatically built in.

![The game page](/ZenSpellingGamePage.jpg)

### This is the game page where all the gameplay happens. Tiles are dragged from the left side of the screen onto the board and a question pops down from the top of the screen. Once the question is answered, a sound plays and according to whether or not the student got the question right. If they answer incorrectly, the tile that the student placed will change into a weed. The weed can be removed by clicking on it. This will pop up with another question and if that question is answered correctly, the weed will disapear. Once the allotted questions have been answered, the student is taken to the complete screen. The complete screen shows the metrics for the game that the student completed and any medals they earned.

## [SLC Chapter of the Japanese American Citizen's League Client Website](https://github.com/cmpt375-2024spring/client-project-jacl)



## [Chatroom](https://github.com/PapaZ810/Chatroom)

Chatroom was a project from Greg's Network class in Fall of 2023. Chatroom was the final project in the class in which we as a class decided on a network protocol to implement a chatroom server and client. 
