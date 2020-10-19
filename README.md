# rllab-gym-wrapper
This is the *gym* goal-based robotic environment wrapper designed for *rllab*.  
If you want to implement RL algorithms under *rllab* to perform *gym* goal-based robotic tasks,
you'll need to wrap corresponding *gym* environments to be *rllab*-based.


# Usage

```
from gym_env import GoalEnv
from env_utils import normalize_goal_env

env = normalize_goal_env(GoalEnv(env_name))
```
- `env_name` is the *gym* environment name.
- `env` is a *rllab*-based environment.
