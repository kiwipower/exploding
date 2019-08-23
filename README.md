# exploding

## Requirements (unattended)

Implement a computer version of the game described in phase 1 and then phase 2. The code should be production quality.

In a real scenario you would probably have questions about the requirements. For this exercise, please some reasonable assumption and document it.


### Phase 1: Basic roulette ruse

* There are one player and 47 cards. One of the cards is explosive and the rest are blank.
* All the cards are shuffled and arranged face down in a draw pile.
* The player draws cards one after the other. If the card is blank, it has no effect, and can be discarded. If the card is explosive, the player loses.


### Phase 2: Defuse cards

* We have three additional _Defuse_ cards, making a total of 50 in the deck.
* Game set up:
  1. Give one defuse card to the player.
  2. Put the remaining two defuse cards with the rest in the draw pile, shuffle and arrange face down.
* The player's turn consists of two steps:
   1. Draw one card
   2. There are three alternatives:
      * Blank card: the turn finishes.
      * Explosive card, if the player has a defuse card: 
        1. Discard the defuse card onto the discard pile.
        2. Return the explosive card to the draw pile.
        3. Re-shuffle the draw pile.
      * Explosive card, if the player does not have a defuse card: The player loses.


## Extension ideas

Just to think about, we might ask some or parts of them in person.

### Variable number of cards of each type

### Variable number of players

### See the future and Skip

* We have two new types of cards: _See the future_ and _Skip_
* The full deck now has:
  * _Explosive_: As many cards as number of players minus one
  * _Defuse_: As many cards as the number of players plus two
  * _See the future_: 5 cards
  * _Skip_: 4 cards
  * Blank: 37 cards
* _See the future_ card: allows a player to reveal the top three cards of the draw pile.
* _Skip_ card: allows a player to skip drawing one card from the draw pile.
* The players start with eight cards in their hand. The number of cards in the hand vary during the game, without limits.
* Game set up:
  1. Give one defuse card to each player.
  2. Excluding the other defuse cards and the explosive card, give another seven cards to each player, randomly taken from the deck.
  3. Shuffle all the other cards and arrange them face down in a draw pile.
* Each player's turn consists of two steps. Note that drawing happens _at the end_ of the turn.
  1. Play as many cards as wished from the hand, placing them face up on top of the discard pile. The player can continue playing cards until a skip card is used, until she runs out of cards or until she decides so. If a skip card was used, the turn finishes and the next player goes. Otherwise, the turn continues in the step below.
  2. Draw a card. If the card is explosive, a defuse card can be used like in the Phase 2 game, otherwise the player that drew it loses and the other one wins.
