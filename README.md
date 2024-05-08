# rl-intro

In Reinforcement Learning, we are trying to solve a problem that is framed as an MDP - a Markiv Decision Process. An MDP is comprised of states $s \in S$, actions $a \in A$, a transition dynamics function $T$ mapping states $s$ and actions $a$ to follow-up states $s'$, i.e. $T:S \times A \rightarrow S$  (or $T:S \times A \times S \rightarrow R$ if the dynamics are stochastic), a reward function $r:S \times A \times S \rightarrow R$, as well as a discount factor $\gamma$ and an initial state distribution $d:S \rightarrow R$.

In the following, we will derive one of the most well known MDPs of RL literature - the so called mountain-car environment. In it, a car needs to drive up a mountain to a specified goal location, however the engine is not strong enough to simply drive it up directly - instead, the car needs to build up momentum by going forward and backward alternatingly until it can drive up the hill. See the image below to get in idea of the environment:

<p align="center">
    <img src="https://github.com/hasanselimyagci/rl-intro/blob/main/mountain_car_continuous.gif">
  </p>
