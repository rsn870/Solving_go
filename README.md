# Solving_go
Trial_1:
# Q learning with 100% Heuristic Reward, epsilon greedy policy
(Look at the raw file for a better view)
'''
Req Steps:

  Design ENV ....(Done)  
  
  Create Class with(Input = board size, reward_fn):
      Initial parametres:
          learning rate
          q table
          list of actions
          epsilon
'''          
      Policy_Fn(epsilon greedy)(Input = self, current state of borad)
'''      
      Fn for learning(Input = self, current state of borad):
          choose action based on policy
          calculate reward
          update Q table
          repeate
'''
      Fn for displaying current states and rewards(Input = self, current state of borad)
      
      
      
  Fn to run the model on ENV against opponent
      .Opponent can be different AI(Preferably Alpha GO itself??)
      .Opponent can be same AI(But this is inefficient at beginning)
      .Switch AI at different stages of development => save model repeatedely after some iterations to allow for switching?
      .Also allow for starting the game in a random/predecided state rather than only empty board
      .Finally display reward
      
 Fn to use above fn to train class over multiple sets of games.
 (Is this req for Heuristic Reward? Only real reward seems to demand this fn)
