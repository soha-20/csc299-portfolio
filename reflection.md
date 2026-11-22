# Reflection for developed game project

## 1. What fresh session asked

- the fresh confirmed the format again and again, if I wanted it to be in browser or a separate window,
- it kept asking about grim reaper's position which was kind of confusing to me as I did not understand the tile system it was asking. So, I instructed that grim reaper should chase the player, the way normally the player is being chased.


## 2. What made change in the previous requirement

- I first made the requirements in a way that there should be a dark mazed theme in the game. Later on, the controls were not that really good in terms of player movement, so I instructed it to be a graveyard. 
- The hurdle were not working well in terms of blocking the player's way in the previous maze, so graveyard helped to resolve that issue. 

## 3. test that checks nothing useful

- def test_R10_a_remembered_jump_that_runs_out_with_no_key_held_does_nothing():
 It was meant to guard against the crash you reported, but it never reached the code path that crashed. When I ran it against the code from before the fix, it passed. So it could never have caught the bug coming back.

 ## 4. Commits
  
- there are few commits that are not detailed and specific like "Updated CLAUDE.md". It does not tell for which round I made updates, so later on it became hard for me to identify the round.

## 5. Function 
- def test_R13_the_reaper_closes_in_while_the_player_hesitates():
   
   my_answer: I think this function does the job when the player pauses, it speeds up the pace up Grim reaper and it starts getting closer to the player. 

Correct: It actually if the player has stopped moving, but keeps the reaper coming towards him as the grim reaper does not wait.
Wrong: It does not do anything with the reaper's speed, it keeps a check on shrinking distance. 
