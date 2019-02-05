Memoarrr! C++ Implementation

Viran Daluwatte & James Lim

--------------------------------------------------

Background:
Memoarrr! is a card memory game where players reveal face down cards in an attempt to
match them with other revealed cards. A description of the physical card game is provied
at https://boardgamegeek.com/boardgame/230383/memoarrr

Description:
This implementation is for a console version of the board game, implemented using object 
oriented programmincing methods in C++. In this version of the game, the cards are
represented by a 3x3 array representing the colour and animal on the card. The 5x5 grid
of cards will be represented with numbered columns, and rows identified by letters A 
through E.

Example..
rrr			zzz
rPr - Red Penguin	zzz - Face down card
rrr			zzz

  zzz yyy zzz zzz zzz 
A zzz yWy zzz zzz zzz 
  zzz yyy zzz zzz zzz 
  
  zzz bbb zzz zzz zzz
B zzz bTb zzz zzz zzz
  zzz bbb zzz zzz zzz
  
  zzz zzz     zzz zzz
C zzz zzz     zzz zzz - Full Grid
  zzz zzz     zzz zzz
  
  yyy zzz ppp zzz zzz
D yCy zzz pWp zzz zzz
  yyy zzz ppp zzz zzz
 
  zzz zzz zzz zzz rrr
E zzz zzz zzz zzz rOr
  zzz zzz zzz zzz rrr

   1   2   3   4   5
The game uses a main loop that executes the console and game through various objects and
classes. All code used to implement this game was created solely by us.

Expert Mode:
Two expert modes have also been implemented into the game: Expert Rules, and Expert
Display. These modes can be activated individually or together through the user's choice.

Expert Display mode uses the same rules as the base game, however the grid of cards will
not be shown to the user, and only face up cards and their position will be provided.

Example...
yyy yyy bbb bbb
yOy yWy bTb bPb
yyy yyy bbb bbb
A1  D1  B4  D3

Expert rules mode adds extra rules to the face animals of the cards which are implemented
when the card is turned over. Aside from these rules, all other base rules still hold. The
rules are as follows.
- Octopus: the card is exchanged with an adjacent card in the same row or column.
- Penguin: the player gets to flip any face up card back to face down.
- Walrus: the player blocks a face-down card such that the next player cannot reveal it.
- Crab: the player gets to flip a second card.
- Turtle: the next player skips their turn.

