# ./checkpoint-reversion
When starting the bot, there will be run folders "rlgym-ppo-run-[X]". Pay attention to the folders within, move run folders with the lower numbered folders into `./checkpoint_reversion` befor running the bot again. This allows the learning continuation.

**NOTE**
The bigger the number in the run folder, the newer the iteration is. -potential scripting advantage

# ./Rewards Log
Keep track of rewards and other settings between each run (and commit) here. Follow a file format of `log-[yyymmdd]-[revision].md`.

# Reseting the Bot
Delete everything in `./data` and `/wandb` before running again.

# Resources
- **Learner Settings**: [learner_settings.md](https://github.com/ZealanL/RLGym-PPO-Guide/blob/main/learner_settings.md)
- **Rewards**: [rewards.md](https://github.com/ZealanL/RLGym-PPO-Guide/blob/main/rewards.md)

# Watching realtime
Change `render` inside learner settings in `example.py` to `True` to watch the sim in realtime