
# Final Project : Design Pattern - Monopoly™ 🎲💸
### _Chloé Coursimault & Héloïse de Castelnau_
</p>

- [About The Project](#about-the-project)
- [Classes](#classes)
- [Design Pattern](#design-pattern)

<!-- ABOUT THE PROJECT -->
## About The Project

This is our final Project for the "Design Pattern" course. The goal for this project was to understand the importance and the stakes of embedding Design patern through an implementation of the **Monopoly** in C#


<p align="center">
  <img  src="https://upload.wikimedia.org/wikipedia/en/f/f9/Monopoly_pack_logo.png">
</p>


### Rules
A set of Players is given, each with name and initial position. Dices are rolled and players’ positions on the Game Board will change. The game is played on a circular game board, composed of 40 positions on the board. Each player rolls two dices and moves forward by a number of positions equal to the sum of the numbers told by the two dices.

<details>
  <summary>Here are some required features</summary>
  <ol>
    <li><a>Takes a set of given players.</a></li>
    <li><a>The boardgame should be composed of 40 squares and permits circular turns.</a></li>
    <li><a>Must include 2 specific squares: Jail and Go To Jail.</a></li>
    <li><a>Permits to roll dices.</a></li>
    <li><a>The position of the player must change after the throw of 2 dices.</a></li>
    <li><a>If the player gets 3 doubles during his turn, he goes to jail.</a></li>
    <li><a>A player turn ends after the position of the player changed.</a></li>
    <li><a>If a player is in jail, he needs to get a double or to skip his turn three times to get out. After getting out of jail, the player can’t roll the dices another time, even if he got a double.</a></li>
  </ol>
</details>



### Built With

<img alt="C" title="Csharp" width="40px" src="https://img.icons8.com/color/48/000000/c-sharp-logo.png">|<img title="visual-studio" alt="visual-studio" width="40px" src="https://img.icons8.com/fluency/48/000000/visual-studio-2019.png">|
|--|--|



## Classes

Before beginning to code, we established a first list of the different classes we needed to implement a simplified version of the MonopolyTM game:
*  A player class: it permits to implement different players.
*  A square class: it is useful to create the different type of squares needed to build the boardgame.
*  A boardgame class: it generates a boardgame constituted of different squares.
*  A dices class: it simulates 2 dices.
*  The program class, where the main is located



## Design Pattern 

As we mentioned it earlier in the introduction, we were meant to use one or more design patterns in our code to apply what we have learned during the semester. We implemented them as follows: 
*  A singleton pattern concerning the pair of dices: this way, only one instance will be created during the game and those dices will be callable from any class.
*  A factory pattern regarding the squares: as we need different types of squares to be implemented in the boardgame, we will use this pattern to create them efficiently.
*  A singleton pattern about the boardgame: only one instance will also be created at the beginning of the game, and it will be used to get the corresponding square at a certain position.
*  An iterator pattern regarding the boardgame: it will be used to display each square it is composed of at the beginning of the game.
*  An iterator pattern about the players: it will permit to display the statistics of each player at the end of the game and to manage the roll of players’ turns.

**Here is the corresponding UML diagram**
<p align="center">
  <img width="700" height="700" src="https://user-images.githubusercontent.com/92330168/148696940-38aae2af-e85c-44c7-bcc5-6b774b587a2b.png">
</p>
