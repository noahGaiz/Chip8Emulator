My Project: 

How I got my Idea: 

Looking for an idea for a project, I used my interest to help me decide on an idea and searching online. 
Emulators were good projects ideas and seemed very achievable for my level of coding in my 2nd Year of my Computer Science Degree.
One of my interests being video games and the competitiveness from them, thinking what I could emulate, I researched into the history of computerized games. 
I found chip8 which was an interpreted language made in the mid 1900s. Chip8 was used for microprocessors and I gained interest and researched further.
My idea of making an emulator turned into a two-part project. One part would be written in chip8 which would be my game.
My game choice would be Pong, which is unoriginal, but it is a core part of the history of videogames. 
My second part of the project would be the emulator made in C. This emulator would be ran from the terminal and read in the chip8 program which would run the game. 

 

Problems I Ran Into: 

-One of the first problems that I ran into was researching into the emulator and learning how to load a program into the terminal. 
  I realized I needed to download Linux virtual machine on my laptop to be able to access the terminal. 
  My laptop for some unknown reason couldn't install a Linux virtual machine which had me stumped for a day or two.
  I realized while exploring the internet for ways to get a terminal the IDE I use to program also has a terminal (Visual Studio Code) so that resolved my issue. 

-My second problem I ran into was trying to convert Assembly language into Chip8. My project initially was meant to be one part
  Assembly code for the game and one part the C emulator. I was unable to find anywhere to convert assembly into Chip8, 
  so my resolution was to learn and program it in Chip8. 

-A problem I came across while writing my chip8 program was, my initial idea was to make pong but having issues working 
  with the overflow register in the language I reversed the aim of the game so the players must keep dodging until the other player gets hit by the ball. 

-A problem while making reverse Pong, I didnt haven enough registers fir 2 paddles and 2 balls so in the game the two balls 
  share the same y velocity variable so if one ball bounces of the ceiling or floor the other ball bounces too following its velocity. 
  This added difficulty to the game making it more playable. 

 

Part 1 (Chip 8 Program Pong) 

1st Day:
Researching and looking at manuals to learn Chip8 I started making progress making the sprites for the game. Before having an emulator made, 
I found an online compiler for chip8 which I have linked to the references. 

2nd Day
I started by figuring out the sprites and the placement of the sprites for the game when it initializes it. 

 

4th Day
After finding the placements for the sprites, I added a ball sprite that would spawn in the middle, at this point of coding the paddles are also moving but 
inconsistently as I haven't implemented a proper loop to cycle the game. 


7th Day
I have implemented boundaries for the paddles so they can't go off the screen. A minor issue is that the IDE I'm using “Octo” 
when playing on the screen for the y coordinate that is the highest it goes, it doesn't touch the top of the screen and I'm not sure 
if there is a way around it. At this moment of making the game I realized how hard it is to work with the overflow 
register in the programming language and reversed the aim of the game to dodge the ball. 

 8th Day
 Realizing the aim of the game is to dodge the ball , I decided to add another ball and bigger to add more difficulty to the game,
 I tried to implement a ball that would be twice as quick too but I was unable to do that as if the ball 
 moves quick it skips the border check and goes thorugh to the other side.

 
12th day
All I had left was to add the ball to paddle collision and I would have  the game done unless I wanted to add some extra parts 
to the game like add more functionality or change the normal ball to be faster perhaps.

15th Day
All that was required to check if the ball hit the paddle was these lines written right after the code for moving the left and right paddle. 
It checks if the overflow register(vf) is equal to 1 meaning if the images overlap in any way, then we reassign vf to equal any key 
in the chip8 keyboard and then when a key is pressed it jumps back to main and plays the game. 

I know this project isnt project and there is a couple lying around bugs but the circumstances of learning a new language 
and trying to learn it quickly and adapt. This has thought me quick learning and adaptability along with time management.It was
my first time using the virtual machine part of a langauge so it was very intriguing and insightful.
 

 


References: 
http://devernay.free.fr/hacks/chip8/C8TECH10.HTM#memmap 
https://tobiasvl.github.io/blog/write-a-chip-8-emulator/ 
https://github.com/JohnEarnest/Octo/blob/gh-pages/docs/BeginnersGuide.md 
https://en.wikipedia.org/wiki/CHIP-8 
https://www.youtube.com/watch?v=e-G6Dm5AX3I Used to help learn chip8 
