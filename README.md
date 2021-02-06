# Intrinsic motivation for robotic manipulation learning with sparse rewards

Machine Learning Algorithms have become increasingly efficient at solving complexreal-world problems. In particular, Reinforcement Learning algorithms are capable of learning behaviors applicable to robotics that can replace or work together with classical control models, thereby increasing their robustness, applicability and viability. However,it remains difficult to design reward functions that represent, for a reinforcement learning agent, the task it must perform. Recent research in this area proposes techniques such as curiosity and intrinsic motivation as an alternative to the use of extrinsic environmental rewards, proving to be efficient in guiding the agent to satisfactory exploration in game environments such as VizDoom and Super Mario Bros. This paper analyzes the impact of the intrinsic motivation technique on agent training in robotic simulation environments, as well as its general implications for aspects such as generalization, exploration and sampling efficiency. We found that this approach encourages increasing exploratory behaviors even after the goal tasks were learned. Furthermore, we found that adding information about other objects' states into the agent's observation is crucial for learning complex behaviors when no dense reward signal is provided. This, however, requires the agent to learn it's own dynamics before interacting with the rest of the environment.

To read the whole analysis, [click here](https://github.com/bryanlincoln/undergraduate-thesis/blob/master/Monografia.pdf) (Portuguese).

The code for this study is available [here](https://github.com/bryanlincoln/intrinsic-motivation).

## Results

### Learned policies

Pick And Place Task (left), Push Task (center) and Reach (right).

<img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/pick.gif" width="260" height="180"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/push.gif" width="260" height="180"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/reach.gif" width="260" height="180">

### Success Rate Charts

Pick And Place Task (left), Push Task (center) and Reach (right). Blue lines are results for vanilla PPO (baseline) and red lines for PPO + intrinsic motivation.

<img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/pick.png" width="260" height="200"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/push.png" width="260" height="200"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/reach.png" width="260" height="200">

### Entropy Charts

Pick And Place Task (left), Push Task (center) and Reach (right). Blue lines are results for vanilla PPO (baseline) and red lines for PPO + intrinsic motivation.

<img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/pick_ent.png" width="260" height="200"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/push_ent.png" width="260" height="200"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/reach_ent.png" width="260" height="200">

### Intrinsic Reward Charts

Pick And Place Task (left), Push Task (center) and Reach (right).

<img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/pick_int.png" width="260" height="200"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/push_int.png" width="260" height="200"> <img src="https://github.com/bryanlincoln/undergraduate-thesis/blob/master/fig/preview/reach_int.png" width="260" height="200">
