# Project - BipedalWalkerHardcore with TD3-FORK    

### Environment  

Solving the environment require an average total reward of over 300 over 100 consecutive episodes.    
Training of BipedalWalkerHardcore is considered as difficult task.   
In particular, it is very difficult to train BipedalWalkerHardcore by DDPG and TD3.   

__BipedalWalkerHardcore-v2__ has been bumped to __BipedalWalkerHardcore-v3__ with fixes of [Jan 31, 2020](https://ai.stackexchange.com/questions/13848/has-anyone-been-able-to-solve-openais-hardcore-bipedal-walker-with-their-implem).    

["To expand on why DDPG doesn't solve it, when although buggy, 
BipedalWalkerHardcore-v2 is solvable: The solution landscape to this problem 
is as full of pits as the environment itself. 
To learn to leap over a pit in the environment for example, 
the agent must perform a complex sequence of actions 
that is difficult to discover by random chance. 
Each time it fails, it learns that being close to a pit is highly likely 
to result in a large penalty, and in an effort to maximise it's rewards, 
will often remain stationary with a naive method like DDPG as the rewards 
for doing that are higher than trying and falling into the pit once more. 
In short, vanilla DDPG lacks enough exploration power 
to find the complex series of actions required before it converges 
on not going near the pit. Not to mention all of the other things 
it needs to learn to be successful."](https://ai.stackexchange.com/questions/13848/has-anyone-been-able-to-solve-openais-hardcore-bipedal-walker-with-their-implem).

In this directory we solve the environment in __6783 episodes__ ib __18 h 47 m__   
by usage of the __TD3-FORK__ algorithm, see the basic paper [FORK: A Forward-Looking Actor For Model-Free Reinforcement Learning](https://arxiv.org/abs/2010.01652).

![](images/2-image_bph_1.png)


### Training History

1. Score 303.7,  Achieved in 6783 episodes

![](images/plot_avgscore_BipedalWalkerHardcore_6783epis.png)

       Average number of steps:    
![](images/plot_avgnumsteps_BWH_6783epis.png)

