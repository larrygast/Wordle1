# Wordle game in React Native

## Improvements:
- save current progress in AsyncStorage? perhaps?
    - right now the game can be closed and relaunched and you can start from scratch which will let you cheat

- Keep track of score and streaks
    - number of games played
    - win rate
    - current streak
    - max streak

- make it so only valid words can be entered

- Animations

## Issues to fix:
- If a letter is guessed and is in the word but already used in the correct position, it shouldn't render as yellow, it should be grey. 
- Right now, it renders as yellow even if the letter is also used in the correct position in the currently guessed word.
- Ex. for the word to guess is "Gusto"
    - gusso 
    - Gusto
- The first 's' in "gusso" should be green but the second one should be grey (since there is only one s in gusto). Currently it is yellow. 


    ## current logic
    - If the letter is not in the right position, but is in the word that we are guessing, it will be yellow.

    ## new logic
    - If the letter is not in the right position AND isn't guessed correctly somewhere else in the word, it will be yellow
    - UNLESS the letter occurs twice in the word





