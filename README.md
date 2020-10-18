# Solving_go
Trial_1:
# Q learning with 100% Heuristic Reward, epsilon greedy policy
(Look at the raw file for a better view)
'''
Req Steps:

  Design ENV ....(Done)  
  
  Create Class with(Input = board size , reward_fn):
      Initial parametres:
          learning rate
          q table
          list of actions
          epsilon #Fix between 0-1
'''          
      Policy_Fn(epsilon greedy)(Input = self, current state of board)
'''      
      Fn for learning(Input = self, current state of board):
          choose action based on policy
          calculate reward 
          update Q table
          repeat
'''
      Fn for displaying current states and rewards(Input = self, current state of borad)
      
      #We do not mention self explicitly (only in the documentation !) since this will be a member function of the class (Use self only in the code)
      
  Fn to run the model on ENV against opponent
      .Opponent can be different AI(Preferably Alpha GO itself?? #Facebook has some nice models available at it's research website please have a look !)
      .Opponent can be same AI(But this is inefficient at beginning) (#I would suggest this is crucial for robustness)
       #Preferably train using supervision as in (1) for a few samples and then switch to 2 . Going right off the bat with 2 creates problems in practice.
      .Switch AI at different stages of development => save model repeatedely after some iterations to allow for switching?
      #Checkpointing is something we need to do anyways. Look it up if you like !
      .Also allow for starting the game in a random/predecided state rather than only empty board
      #Great Idea! Would make for some interesting scenarios
      .Finally display reward
      #Not needed per se. Store game data in disk for each game and then display. Images showing board state would be great
      #need to specify exactly what data to be stored. Complete set of moves? Only Rewards and actions or just final results
      
 Fn to use above fn to train class over multiple sets of games.
 (Is this req for Heuristic Reward? Only real reward seems to demand this fn)
 #This function is reward agnostic i.e You can switch between either
 #Yes, but if the reward is heuristic, completion of game is not a requirement per se
