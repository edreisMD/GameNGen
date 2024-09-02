
#### 1. Train Agent Play

I encounter some problems intalling the requirements. I needed to install cmake, sdl2, and boost first using brew on Mac:

Mac:
```bash
brew install cmake boost sdl2 openal-soft
```

```bash
pip install -r requirements.txt
```

Create a `scenarios/` folder.
Go to [Scenarios examples](https://github.com/Farama-Foundation/ViZDoom/tree/master/scenarios) and download the files basic.cfg and basic.wad to the scenario folder.
You can get other scenarios from there.

References:
- Doom RL Tutorial [Medium Article](https://lkieliger.medium.com/deep-reinforcement-learning-in-practice-by-playing-doom-part-1-getting-started-618c99075c77) by [Leandro Kieliger](https://lkieliger.medium.com/?source=post_page-----618c99075c77--------------------------------)
- Doom RL Tutorial [Notebook](https://nbviewer.org/github/lkiel/rl-doom/blob/develop/standalone_examples/Basic%20Scenario.ipynb)
- [Stable Baselines 3](https://stable-baselines3.readthedocs.io/en/master/index.html)
- [VizDoom](https://github.com/mwydmuch/ViZDoom)
