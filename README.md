# rllab-gym-wrapper
This is the *gym* goal-based robotic environment wrapper designed for *rllab*.  
Since *rllab* does not support goal-based environment,
if you want to implement RL algorithms under *rllab* to perform *gym* goal-based robotic tasks,
you'll need to wrap corresponding *gym* environments to be *rllab*-based,
although *rllab* is no longer under active development and is maintained under [garage](https://github.com/rlworkgroup/garage).


# Usage

```
from gym_env import GoalEnv
from env_utils import normalize_goal_env

env = normalize_goal_env(GoalEnv(env_name))
```
- `env_name` is the *gym Robotics* environment name.
- `env` is a *rllab*-based environment.

and it should be good to go.
