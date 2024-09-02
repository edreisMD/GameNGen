# Train Agent Play

Planning to use the [VIZDoomBot](https://github.com/ViZDoomBot/stable-baselines-agent) library to train the agent to play the game.

Perhaps "stable-baselines-agent/simpler_basic/train.py" is a good starting point.
Necessary to create a multitude of variations of scenarios and run the training.
8 runs in parallel.
Configs from the paper:
- feature network: simple CNN
- map resolution: 160x120
- last actions: 32
- representation size: 512
- games parallelism: 8
- replay buffer size: 512
- discount factor γ = 0.99
- entropy coefficient: 0.1
- batch size: 64
- epochs: 10
- learning rate: 1e-4
- environment steps: 10M

REWARD FUNCTION descriptionfrom the paper:

"""
The RL-agent’s reward function, the only part of our method which is specific to the game Doom, is a sum of the following conditions: 
1. Player hit: -100 points. 
2. Player death: -5,000 points. 
3. Enemy hit: 300 points. 
4. Enemy kill: 1,000 points. 
5. Item/weapon pick up: 100 points. 
6. Secret found: 500 points. 
7. New area: 20 * (1 + 0.5 * L1 distance) points. 
8. Health delta: 10 * delta points. 
9. Armor delta: 10 * delta points. 
10. Ammo delta: 10 * max(0, delta) + min(0, delta) points. 

Further, to encourage the agent to simulate smooth human play, we apply each agent action for 4 frames and additionally artificially increase the probability of repeating the previous action.
"""