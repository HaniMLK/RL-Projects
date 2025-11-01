**Double Gyre flow navigation using Reinforcement Learning algorithms**

The Double Gyre is Time-Dependent
The flow oscillates left–right periodically.
If the agent is trained with a fixed or narrow range of time phases, its learned policy becomes phase-dependent.
Observation now: [x, y, u, v, sin(ωt), cos(ωt)] → the policy becomes time-aware.

Action mode switch:

  action_mode="discrete" → same 8+stay (DQN-ready).
  action_mode="continuous" → Box([-1,1]^2) PPO-ready
