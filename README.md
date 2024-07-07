<p align="center">
<img src="00_logo.svg" />
</p>

# Gomori

Gomori is a *2 Player* Tactical-Card-Game played with a default 52-Card-Deck influenced by _Connect 4_, _Reversi_ and _Triple Triad_.

## Setup

<p align="center">
  <img src="01_setup.svg" alt="Figure 1: The playing field." />
  <p align="center"><i>Figure 1: The playing field.</i></p>
</p>

- The 52-Card-Deck is *split into two* 26-Card-Decks by color -- one deck containing the *black suits*
  (<span style="color:#f1f1f1">clubs (♣)</span>, and <span style="color:#f1f1f1">spades (♠)</span>),
  the other one containing the *red suits* (<span style="color:#cf3b3b">diamonds (♦)</span> and
  <span style="color:#cf3b3b">hearts (♥)</span>). Each player plays their own deck.
- The game is played on a loosely defined *4x4 field* (as long as there are no 4 fields in an axis,
  the field can be extended in either direction).
- Each player draws *5 cards* from their deck -- the remaining cards are used as draw pile.
- The player playing the black suits begins.
- Gathered cards of each player are placed upside down clearly distiguishable on the respective players side of the field.

## Goal

The player with the most gathered cards wins.

## Rules

### Gathering Cards

<p align="center">
  <img src="02_gathering_00.svg" alt="Figure 2: Rows, columns, and diagonals of the playing field." />
  <p align="center"><i>Figure 2: Rows, columns, and diagonals of the playing field.</i></p>
</p>

- If *four cards of same suit* lie in one <span style="color:#ae63a4">_row_</span>,
  <span style="color:#43bdd8">_column_</span> or <span style="color:#f5c62b">_diagonal_</span> line,
  the player who just laid the fourth one *takes the cards* (including stacks)
  *except the one laid last* (including its stack) and stacks them face-down on their gathered cards stack.

<p align="center">
  <img src="03_gathering_01.svg" alt="Figure 3: The five of clubs finishes the second column to be filled with all clubs." />
  <p align="center"><i>Figure 3: The five of clubs finishes the second column to be filled with all clubs.</i></p>
</p>

### Playing Cards

- *Number cards* (2-10) can be played on
  - <span style="color:#ae63a4">empty fields</span>,
  - <span style="color:#43bdd8">face-down cards</span> or
  - <span style="color:#f5c62b">cards of the same rank -- regardless their suit</span>.

<p align="center">
  <img src="04_playing_numbers.svg" alt="Figure 4: The five of clubs can be played on the empty fields, the five of hearts and the face-down card." />
  <p align="center"><i>Figure 4: The five of clubs can be played on the empty fields, the five of hearts and the face-down card.</i></p>
</p>

- *Face cards* (jacks, queens, and kings) can be played on
  - <span style="color:#ae63a4">empty fields</span>,
  - <span style="color:#43bdd8">face-down cards</span>,
  - <span style="color:#f5c62b">cards of the same rank -- regardless their suit</span> -- or
  - <span style="color:#7587c2">cards of the same suit</span>

Always, When *face cards* are played on other cards (regardless if face-up or face-down) they get activated. See [Activating Face Cards](#activatingface-cardsandturningcardsface-down).

<p align="center">
  <img src="05_playing_face_cards.svg" alt="Figure 5: The jack of clubs can be played on the empty fields, the jack of hearts, the face-down card and also all other cards of clubs." />
  <p align="center"><i>Figure 5: The jack of clubs can be played on the empty fields, the jack of hearts, the face-down card and also all other cards of clubs.</i></p>
</p>

- *Aces* can be played <span style="color:#ae63a4">everywhere</span> -- on
  - empty fields,
  - face-down cards
  - cards of any rank and suit.

<p align="center">
  <img src="06_playing_aces.svg" alt="Figure 6: Aces can be played everywhere." />
  <p align="center"><i>Figure 6: Aces can be played everywhere.</i></p>
</p>

### Activating Face-Cards and Turning Cards Face-Down

Face Cards have each an additional effect, that gets activated when played on another card.
These effects have to be executed and are executed _before_ any other action including gathering cards.

<p align="center">
  <img src="07_activating_face_cards.svg" alt="Figure 7: The Jack turns horizonally and vertically, the Queen diagonally. Already turned face-down cards are not turned face-up again." />
  <p align="center"><i>Figure 7: The Jack turns horizonally and vertically, the Queen diagonally. Already turned face-down cards are not turned face-up again.</i></p>
</p>

- The Jacks: All face-up cards lying horizontally and vertically next to the jack are turned face-down
- The Queens: All face-up cards lying diagonally next to the queen are turned face-down
- The Kings: One card anywhere on the field by the current players choice is turned face-down -- the king itself can also be chosen

### Playing more cards

<p align="center">
  <img src="08_playing_more_cards.svg" alt="Figure 8: The five of clubs is stacked onto a face down card, so another card has to be played." />
  <p align="center"><i>Figure 8: The five of clubs is stacked onto a face down card, so another card has to be played.</i></p>
</p>

- Always when one cards is stacked on top of another card, the current player plays another card if possible
- This is chained until either
  - a card is played on an empty field or
  - the player has no more cards on their hand or
  - the player has no legal move left to play another card.
- If a line of four is completed by stacking one card on top of another, the other three cards of the line are taken _before_ the current player plays the next card.

### End of turn

<p align="center">
  <img src="09_end_of_turn.svg" alt="Figure 9: The hand is filled up to five cards." />
  <p align="center"><i>Figure 9: The hand is filled up to five cards.</i></p>
</p>

- If no more cards can or may be played the players turn ends.
- At the end of turn the player fills up their hand to the amount of five cards from their draw pile.

### End of game

<p align="center">
  <img src="10_end_of_game.svg" alt="Figure 10: The hand cannot be filled up to five cards. The game ends immediately." />
  <p align="center"><i>Figure 10: The hand cannot be filled up to five cards. The game ends immediately.</i></p>
</p>

- If the current player cannot fill up their hand at the end of turn for the draw pile being empty, the game ends immediately and the gathered cards are counted for each player.
- The game also ends, if both players cannot play any card in consecutive turns.

## Trivia

The name of the game comes from combining the words _Go_ and _Memory_, as the first version of the game had elements of both of them. Though all these gameplay-elements have been removed from the game at later stages, the name stayed the same.

## Version and License
- Version 1.0.2
- CC-BY-SA-4.0, Philipp Wittershagen
