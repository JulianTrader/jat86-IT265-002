

# Game Design Document (GDD)

## Gamball

**Change Log**  
*Physical Prototype*

- Changed design of board during the building of the physical prototype. Initially one small hole for the ball to go through, now much longer for more space, variety, and player choice.   
- Changed how items work. Originally called “Power Ups”, that would be used on the opponent to give them a variety of effects. Now called “Items” to be used on the user to give them a variety of effects. This change was made to streamline the items a little more and make tem
a little less confusing and make more sense in gameplay.
- Added dice to determine turn order.

*Digital Prototype*

- Swapped red and green for more clarity. Originally green was \-10 points and red was \+100, points are now swapped. Their positions on
the board are also swapped.

## Table of contents

1. [Introduction](#1.-introduction)  
   1. [Scope of the document](#1.1.-scope-of-the-document)  
   2. [Elevator pitch](#1.2.-elevator-pitch)  
2. [Game overview](#2.-game-overview)  
   1. [Game concept](#2.1.-game-concept)  
   2. [Audience](#2.2.-audience)  
   3. [Genre](#2.3.-genre)  
   4. [Setting](#2.4.-setting)  
   5. [Player](#2.5.-player)  
   6. [Game flow summary](#2.6.-core-loop)  
   7. [Look & Feel](#2.7.-look-&-feel)  
3. [Gameplay](#3.-gameplay)  
   1. [Objectives](#3.1.-objectives)  
   2. [Progression](#3.2.-progression)  
4. [Mechanics](#4.-mechanics)  
   1. [Rules](#4.1.-rules)  
   2. [Physics](#4.2.-physics)  
   3. [Player interaction](#4.3.-player-interaction)  
      1. [Game options](#4.3.1.-game-options)  
   4. [Assets](#4.4.-assets)  
5. [Graphics and audio](#5.-graphics-and-audio)  
   1. [Visual system](#5.1.-visual-system)  
      1. [Player camera](#5.1.1.-player-camera)  
   2. [Interface](#5.2.-interface)  
6. [Story and narrative](#6.-story-and-narrative)  
   1. [Backstory](#6.1.-backstory)

## 1\. Introduction {#1.-introduction}

### 1.1. Scope of the document {#1.1.-scope-of-the-document}

This document is written for me and anyone else who may work on the game at some point in the future. It documents all of the main ideas of the game.

### 1.2. Elevator pitch {#1.2.-elevator-pitch}

Gamball is designed to be a fun competitive experience where things can get a bit random as well as chaotic. You will “gamble” against your opponents using balls and items to boost (or hurt) your odds of winning. Every move in the game is a risk, making the game a bit more intense where you’ll never know what will happen next. Unpredictable chaos is the name of the game.

## 2\. Game Overview {#2.-game-overview}

### 2.1. Game concept {#2.1.-game-concept}

The objective of the game is to win as many points as possible while trying to thwart the efforts of your opponent. The challenges rise in the unpredictability of the game and trying to make the most of it while also maintaining an advantage. Players should feel the pressure of the game as they think about their every move, whether they’re dropping balls or deciding whether or not to pull an item that can make or break their game. They’ll enjoy thriving in the chaos game brings as they play against each other and hope for the best.

### 2.2. Audience {#2.2.-audience}

The game is meant to appeal to a much more competitive audience of gamers in the age range of teenagers to young adults. They would like genres such as strategy and games of chance/randomness. Similar games would be plinko or pachinko. The game is heavily based on chance, and having that chance be in a multiplayer environment where people could compete against their friends and family would appeal more to these people.

### 2.3. Genre {#2.3.-genre}

This genre would be classified as turn-based strategy mixed with chance.

### 

### 2.4. Setting {#2.4.-setting}

The game takes place in a futuristic casino where players can compete with others to win big. Players can now take advantage of the latest technology to manipulate the game in their favor or out of their opponent's. However, it's still gambling so there's no telling what might happen, a player may end up sabotaging themselves instead of their opponent. Much of entertainment has been made to be casinos, so for better or for worse everyone must play at a casino. Gambling has become a competitive sport and now it's pretty much all there is.

### 2.5. Player {#2.5.-player}

The player has one goal: to play and win big. They are an up and coming gambler who is determined to become the Master of the Casino. They've been on a hot streak on the path to becoming the master and now it's the closest they've ever been to taking the title. The game is multiplayer and can go up to four players, where all players are competing for the same title of Master of the Casino.

### 2.6. Core loop {#2.6.-core-loop}

The core loop of the game is at the beginning of each turn, players can choose whether or not they want to pull an item card that may or may be beneficial to them. They will then choose to drop up to three balls on the board; this will end their turn.

### 2.7. Look & Feel {#2.7.-look-&-feel}

The game will have a dark and colorful vibe, like bright lights in a dark room. It should feel like the player is in a casino, and all parts of the style would reflect that. The game would only showcase the gameboard and anything surrounding it, as the camera would show a topdown view of the board for a clear view of the balls and their movement on the board. Any music in the game would sound like music that may be heard in a casino or similar. 

## 3\. Gameplay {#3.-gameplay}

### 3.1. Objectives {#3.1.-objectives}

The goal of the game is to gain more points than all opponents by the end of the game, while gambling their luck to hopefully score more points each round.

### 3.2. Progression {#3.2.-progression}

The game will follow the same general game loop up until the end of the game. During the last five turns, the game will enter “Fever Mode” where all points, positive and negative, are double their original value (e.g. \+100 \-\> \+200 or \-100-\>-200). This will allow for unlikely comebacks and create even more chaos in the game.

## 4\. Mechanics {#4.-mechanics}

Drop the balls: The initial base mechanic is to drop balls into a machine that will go into holes to score points... or lose points. The player can choose how many balls they would like to drop onto the board, they could choose up to three balls and can even choose to drop none.

Items: Before each turn, a player may choose to draw an item card. However this item may not always be beneficial to the user and may end up helping the opponent instead. The player will get to choose whether or not they would like to get an item and will have to use whatever they pull. 

Block: There will be specific blocks for specific colors, so you can't score in a specific hole (this includes the negative points as well)

x2 Points: There will be specific ones for specific colors, so you'll gain or lose double the amount of points during your turn.

Bad Ball: You can add another ball to the set of balls, but it will perform the opposite effect of whatever it lands on. (e.g. if a bad ball lands in \+50, then the player who dropped the ball would LOSE 50 points instead of gaining 50 points)

Great Ball: Adds another ball to the set that doubles the amount of points received wherever the ball lands, including the negative points.

Fever: Toward the end of the game, all points earned and lost will be doubled to up the stakes as the game comes to an end. This may also allow for some otherwise impossible comebacks that make the game just a bit more intense.

### 4.1. Rules {#4.1.-rules}

1. To begin the game, players must agree on a turn count to determine the length of the game.   
2. At the start of each turn, players can choose whether or not they want to draw an item card.  
3. Choose to drop from up to three balls (including 0\) onto the board and drop them through the hole.  
4. Whoever has the most points when the game is over is the winner.

### 4.2. Physics {#4.2.-physics}

The ball will use slightly modified semirealistic physics to roll around the board. In order to make the game more fun, there will be a bit of random force applied to the ball to add more variety to the ball’s movement.

### 4.3. Player interaction {#4.3.-player-interaction}

The player will interact with the balls they will drop and the item cards they can draw from.

#### 4.3.1. Game options {#4.3.1.-game-options}

The player will be able to choose how many players are in the game as well as how many rounds the game will last.

### 4.4. Assets {#4.4.-assets}

* Gamball Board  
* Balls (Basic Ball, Great Ball, Bad Ball)  
* Item cards

## 5\. Graphics and audio {#5.-graphics-and-audio}

### 5.1. Visual system {#5.1.-visual-system}

The game will be 3D using a 3D model for the game board and basic spheres for the balls. It will have a simple semirealistic artstyle. It would be pretty difficult to make this game work in 2D, so it will take a 3D form, relying on basic physics to get the game working. 

#### 5.1.1. Player camera {#5.1.1.-player-camera}

There will be one camera placed above the board to create a topdown view of the game to make everything easily visible and clear to the player.

### 5.2. Interface {#5.2.-interface}

The user interface will allow the player to make all of their decisions. It will consist of pop up boxes that the player will be able to click on to progress the game. During gameplay, there will be options for the player to begin their turn with either an item or to go straight to dropping balls. When dropping balls, there will be a few options to drop one, two, three, or no balls. 

## 6\. Story and narrative {#6.-story-and-narrative}

### 6.1. Backstory {#6.1.-backstory}

In a world where gambling has pretty much taken over all entertainment in the world, there is one who has proven to be the best among the people, known as the Master of the Casino. They have had a long reign over the casino and many have tried to top them to no avail. However there are few who have been on the come up as of late who may finally threaten the master's reign. The story begins as these juggernauts come face to face in a climactic match to find out who's the true Master of the Casino.
