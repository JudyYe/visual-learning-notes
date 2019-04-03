## intro
- specialist AI vs generailizst human, strong,supervision, limited uspervision; not adapitve, lifelong
- what are human special. 'What do babies think' `TED 2011`
    + 乌鸦：combiniation of task
    + goal eploit vs goal-less exploration
    + how to define exploration???

## baby exploration
- meansure of learning scale?? formulate curiocity, objective-less.
- prediction error as curiosity?? 
- how to gain momentum?? 
    +  Intrinsic curiosity module !!!
    +  ??? how to match curiosity to task-specific reward???
    + network taking in (action, current stte, next state)
    + too big space
        * care things that can affect agent
        * care things that agent can affect

- QA go-back mechanism to avoid keep going or oscillation
- QA keep leving may become as the out-sourcing reward
    + death is removed 
- no external reward, only curiosity


## align to task specific 
- reward fine-tuning 
    + require dense reward
    + for real world, sparse reward: adding in dense curiosity
- Imitation learning
    + tedious for export
    + one goal per time

## vision intuition
- motion comes first

## future work
- multi-robot curiosity: two-gent with dependent curiocity to avoid local minimum
- curiosity in real world, life-long learning 
