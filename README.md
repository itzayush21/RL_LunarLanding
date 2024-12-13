
# 🚀 Exploring Q-Learning with LunarLander in OpenAI Gymnasium: A Journey Into Reinforcement Learning 🌙🤖

I’m excited to share my latest experience working with Q-Learning on the LunarLander-v2 environment in OpenAI Gymnasium! This project was a deep dive into the world of Reinforcement Learning (RL) and gave me the opportunity to enhance my skills in training agents to perform tasks based on trial and error.

# 🔑 Key Highlights:

Q-Learning Algorithm: I implemented Q-Learning, a foundational RL algorithm, to teach the agent how to land a spaceship on the moon. By iteratively improving its policy based on rewards and penalties, the agent learns to maximize its long-term reward.
Gymnasium: Using OpenAI Gymnasium, I could set up a simulated environment where the LunarLander learns by interacting with its surroundings. It was thrilling to watch the agent explore various actions like throttle control, balancing, and steering, all while striving to land safely and reduce damage.
Key Insights:
The learning process focuses on balancing exploration and exploitation, with the agent constantly trying new strategies while refining existing ones.
The epsilon-greedy policy allows the agent to choose actions based on both random exploration and learned knowledge, creating a dynamic decision-making process.



# Lunar-Lander-V3

**Description**
This environment is a classic rocket trajectory optimization problem. According to Pontryagin’s maximum principle, it is optimal to fire the engine at full throttle or turn it off. This is the reason why this environment has discrete actions: engine on or off.

There are two environment versions: discrete or continuous. The landing pad is always at coordinates (0,0). The coordinates are the first two numbers in the state vector. Landing outside of the landing pad is possible. Fuel is infinite, so an agent can learn to fly and then land on its first attempt.

To see a heuristic landing, run:

**Action Space**

There are four discrete actions available:

0: do nothing

1: fire left orientation engine

2: fire main engine

3: fire right orientation engine


**Observation Space**

The state is an 8-dimensional vector: the coordinates of the lander in x & y, its linear velocities in x & y, its angle, its angular velocity, and two booleans that represent whether each leg is in contact with the ground or not.

**Rewards**

After every step a reward is granted. The total reward of an episode is the sum of the rewards for all the steps within that episode.

For each step, the reward:

is increased/decreased the closer/further the lander is to the landing pad.

is increased/decreased the slower/faster the lander is moving.

is decreased the more the lander is tilted (angle not horizontal).

is increased by 10 points for each leg that is in contact with the ground.

is decreased by 0.03 points each frame a side engine is firing.

is decreased by 0.3 points each frame the main engine is firing.

The episode receive an additional reward of -100 or +100 points for crashing or landing safely respectively.

An episode is considered a solution if it scores at least 200 points.





![Screenshot 2024-12-13 203327](https://github.com/user-attachments/assets/ed8c7fce-ea18-4099-b8a3-4f5012b22706)





![Screenshot 2024-12-13 203344](https://github.com/user-attachments/assets/6338fff6-f394-49c4-990b-9dbd00fd14cd)






![Screenshot 2024-12-13 203357](https://github.com/user-attachments/assets/d9731566-cd56-4102-af5a-ab33cb08da67)


