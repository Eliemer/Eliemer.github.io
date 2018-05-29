## Card++

[View on Github](https://github.com/Eliemer/Card-plus-plus)

[Download](https://github.com/Eliemer/Card-plus-plus.git)

### Introduction

  As part of our Structures and Properties of Programming Languages course we have been
tasked with the creation of a new programming language which in our case would result
in being able to create card games in a short amount of time, with little experience in
programming required. It will be called Card++.

### Statement of Problem

  Card games have always been a big part of human history, As such we want to give
people a tool to be able to continue this tradition via computer programs. We want to 
create a language that would facilitate the development of any card game imaginable, for the scope 
of this project we will begin by limiting our Card++ to only be able to use
the 52 casino suite cards, but it is preferable that expansion of features, such as being
able to define your own unique cards, be easy to implement and maintain.

### Language Details 

  We want Card++ to be as high level as possible, readability is high priority as we want
anyone to be able to pick up our language and start creating. A key feature of our language
is that of definition blocks. These blocks contain clear workspaces in which to work different
aspects of the game in. For example, at the start of your code, you declare a Deck{...} block
in which you list all available cards in the entirety of your game, poker for example, contains
52 casino suite cards, thus each item in the Deck{...} block would contain a number (from
Ace to King) and a suite (hearts, clubs, spades, diamonds). These blocks contain different
aspects of your game code, and are segregated for better readability.

  Another key aspect of our language is that every action revolves around three things:
Player resources (money, energy, etc.), Turn control (skip turns, reverse turn order), or Fields.
This last one is a critical part of our vision. A field is essentially a container for cards. These
fields may have special properties to them, such as the Deck field being invisible to every
player, that is to say, no one can view the values of the cards withing. Other common
fields include a Player’s hand, The playing field, and card graveyards. Common actions that
manipulate fields include: Drawing cards, (move 1 From Deck to Player); Playing cards,
(move 1 From Player to Game). Actions that manipulate player resources may include
betting, or actions be conditioned to a value, say a mana bar. Thus, from this framework of
actions we can implement anything we’d like the player to do.

### Simple Keywords

* Card: A tuple representing an instance of a game card
* Draw: Adds an instance of a game card to a Field
* Move: Adds a particular instance of a game card to a Field
* Flip: Changes a card's visibility to certain Players
* Shuffle: Mixes all cards' locations in a given Field
* Rules: Boolean statements describing a particular scenario or condition in the game

### About Creators

The creators of the project are a group of students of the University of Puerto Rico at Mayagüez. 
They are:

  * Jonathan Irizarry
  * Eliemer Velez
  * Ariel Torres

This project was developed as part of the Programming Languages course ICOM4036 directed by Dr. Wilson Rivera.
