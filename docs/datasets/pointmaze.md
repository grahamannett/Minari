---
firstpage:
lastpage:
---

# Point Maze

The [Point Maze](https://robotics.farama.org/envs/maze/point_maze/) domain involves moving a force-actuated ball (along the X and Y axis) to a fixed target location. The observation consists of the (x, y) location and velocities. The dataset consists of one continuous trajectory of the agent navigating to random goal locations, and thus has no terminal states. However, for the purposes of being able to split the trajectory into smaller episodes, the trajectory is truncated when the randomly selected navigation goal has been reached.

The datasets for each maze version includes two different reward functions, sparse and dense.

The data is generated by selecting goal locations at random and then using a planner ([QIteration](https://towardsdatascience.com/fundamental-iterative-methods-of-reinforcement-learning-df8ff078652a))[2] that generates sequences of waypoints that are followed using a PD
controller. Because the controllers memorize the reached waypoints, the data collection policy is non-Markovian.

These datasets were originally generated by [D4RL](https://github.com/Farama-Foundation/D4RL/wiki/Tasks#maze2d)[1] under the Maze2D domain.

## References

[1] Fu, Justin, et al. ‘D4RL: Datasets for Deep Data-Driven Reinforcement Learning’. CoRR, vol. abs/2004.07219, 2020, https://arxiv.org/abs/2004.07219..

[2] Lambert, Nathan. ‘Fundamental Iterative Methods of Reinforcement Learnin’. Apr 8, 2020, https://towardsdatascience.com/fundamental-iterative-methods-of-reinforcement-learning-df8ff078652a


```{toctree}
:hidden:
pointmaze/open.md
pointmaze/umaze.md
pointmaze/medium.md
pointmaze/large.md
pointmaze/open-dense.md
pointmaze/umaze-dense.md
pointmaze/medium-dense.md
pointmaze/large-dense.md
```

