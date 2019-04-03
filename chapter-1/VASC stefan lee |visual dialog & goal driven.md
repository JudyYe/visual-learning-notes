# Stefan Lee
`[website](https://www.cc.gatech.edu/~slee3191/)` `Feb 5th` `VASC`

## visual dialog
- agent & human talking
- formulate
    + image I
    + human dialog history Q1, A1, Q2 A2, ...Qt-1, At-1 --> Qt

- Method
    1. Exact match with GT human response like VQA. More than Yes / No
    2. Retrieval metrics
- Dataset
    + ~120k images. 
    + ~1.2M dialog QA pairs
- Model
    + encoder: Memory Network
        LSTM to remember the previous question and answer
    + decoder: language Generative model
    + __turns out to learn mimic human dialog__
        eg. qualitive results
        'I cannot tell'
        'Yes / No'
- short coming
    + downstream tasks are ignored
    + __agent never drives the dialog__

## learning cooperative visual dialog agents with DRL. ICCV'17
- __Q-bot__: ask A & regress on fc 
- __A-bot__: answer Q
- auto encoder communicates with language(Q, A)
- Training
    + start with supervised setting
    + roll back one round so that the question are reasonable
- Results
    + pretty good of RL
    + all we ask is to play a game, not constraining repetition, etc
- takeaway
    + __need ENVIRONMENT and GOALS, NOT JUST DATASET!__

## (EQA) embodied Question Answering, Das arxiv 2017
- + navigation
    + eg. what is left to shower room?
- dataset
    + SUNCG, 2017 CVPR, tianyuandong FAIR
- setup
    + generate Q and A programmatically
        * finite question type(4)
    + Fill in \<hole\>
- Model (Vision + Language + Actions)
    + vision
        * autoencoder , segmentation, depth
    + language
        * LSTM - future work to be better
    + Action
        * hierarchical navigator
            - planner - direction
            - controller - velocity
        * ACT + Q (proposed) 
            - _fancy pipeline_
- fail
    + longer sequence - now works for around 30 steps
    + stuck in rooms
    + stop too far
- future
    + first navigation and then VQA at the top
    + maybe generate some questions to specify the navigation?????

## wrap up
- vision
    + Richer, sturcured representation
    + low-shot, zero-shot learning
- NLP
    + external knwledge bases
    + online 
- naviation
    + receiving goals via language
    + long-range sequential RL
    + goal-directed dialog & perception
- robotics
    + real 
































