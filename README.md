# OpenGamenGen

*Open-source implementation of [GameNGen](https://arxiv.org/abs/2408.14837): Diffusion Models Are Real-Time Game Engines<sup>1</sup>*

## Steps
1. Train Agent Play
2. Collect data at scale
3. Train the diffusion model

### 1. Train Agent Play

Planning to use the [VIZDoomBot](https://github.com/ViZDoomBot/stable-baselines-agent) library to train the agent to play the game.
See specific [README](./opengamengen/train_agent_play/README.md) for more details.

Tutorial on getting started with Doom RL using Stable Baselines 3 and VizDoom.
- See [Tutorial](./opengamengen/train_agent_play/tutorial_get_started_doom_rl/README.md) on folder `train_agent_play/tutorial_get_started_doom_rl`.

Resources:
- VizdoomBot - [GitHub](https://github.com/ViZDoomBot/stable-baselines-agent) / [Website](https://vizdoombot2021.netlify.app/)
- Doom RL Tutorial [Medium Article](https://lkieliger.medium.com/deep-reinforcement-learning-in-practice-by-playing-doom-part-1-getting-started-618c99075c77) by [Leandro Kieliger](https://lkieliger.medium.com/?source=post_page-----618c99075c77--------------------------------)
- Doom RL Tutorial [Notebook](https://nbviewer.org/github/lkiel/rl-doom/blob/develop/standalone_examples/Basic%20Scenario.ipynb)
- [Stable Baselines 3](https://stable-baselines3.readthedocs.io/en/master/index.html)
- [VizDoom](https://github.com/mwydmuch/ViZDoom)

### 2. Collect Data

### 3. Train the diffusion model


## References:

```bibtex
@misc{valevski2024diffusionmodelsrealtimegame,
        title={Diffusion Models Are Real-Time Game Engines}, 
        author={Dani Valevski and Yaniv Leviathan and Moab Arar and Shlomi Fruchter},
        year={2024},
        eprint={2408.14837},
        archivePrefix={arXiv},
        primaryClass={cs.LG},
        url={https://arxiv.org/abs/2408.14837}, 
  }
```