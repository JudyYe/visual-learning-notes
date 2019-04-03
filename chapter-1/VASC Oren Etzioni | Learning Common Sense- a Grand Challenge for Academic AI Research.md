# Learning Common Sense: a Grand Challenge for Academic AI Research
Allen School `[website](http://allenai.org/team/orene/` `Feb 23th` `VASC`

---
# How is a graduate student to make a 'dent in the universe'?
---

What are the problems for graduate students since we have Google and Fb?

##AI mission
click ads->common good??

# monivataion
- 3 easy steps: 
    + gather lots of training data
    + apply deep learning
    + observe impressive gains....
- BUT
    + although performance in specialized domains is often very impressive
    + hardly any of them have certain commonsense knowledge.
    + context failure
    + cheat
- eg. Aristo
    + knowledge for middle school science
    + typical questions require takes formula / term to real world(e.g. gravity). It is harder to put the term in real world for AI (we assume people have commen sense.)
- other reasons
    + robustness: adversarial examples, zeo-shot learning
    + data efficiency
    + generality: transfer learning
    + performance: NLP, robotics, medical diagnosis... plug in common knowledge, performance should boost.
    + safety: Avoid hard only if they know what is harmful.

- what is common sense 
    + knowledge about the world that most people have, but most AI systems do not
    + 'common-sense facts and methods are only very partially understood today(1983)... '
    + No AI system can answer simple question: wha'ts biger, the sun or a giraffe?
    + 


##lessons from Cyc (1984)
- Implicit knowledge is critical!
- size matters scalability
    + size of facts matter
- But you need to know how to use it. e.g. reasoning
- consistency is not realistic
- Set of related techniques:
    + crowd sourcing
- time to revisit the grand challenge
- __benchmark / performance metric is essential__ it is not clear how to / what to measure here


## common-sense benchmark
- questions
    + breath: what topics are covered?
    + depth: what is sophistication of knowledge?
    + language: hould benchmark factor out linguistic challenges and focus on commen sense aspect??? (eg. paraphrases)? benchmark you do not need to understand language. 
    + vision: is visual / robotics common included?
- How ?
    + Allen Inst: _commensoense leader board_
    + duality: common fact and question
    + some try: eg
        * machine reading
            - Open information extraction(2007)
            - text runner openie.allenai.org
            - _BUT suffer from attention deficit disorder.. do not build comprehensible knowledge base to reason about them_
        * Verb physics
            - _Reporting bias_ no body says that "I am larger than a chair, blah blah"
        * Vision as biasis for common sense (imsitu.org)
        * Reason about science
            - are elephnts bigger than butter flies ? Bagherinezhad, AAAI'16

- conclusion
    + common sense is critical for AI
    + progress limited, though DL 
    + we need a benchmark and crisp metrcs
    + new idea on acquisition
    + lauching project _Alexandria???????????_

## Acquisition of Common Sense Knowledge
- Crowd sourcing
    + accumulate common sense
    + active learning, economic variable
    + difficulty
    + coverage
    + crowd sourcing game
- challenge - fundamental problems
    + right representation for common sense knowledge?
    + right problem?
- Ill structured problem
    'AI requies the investigation of ill structured problem'
    + ill-structured problem s are fundamental road rock to AI
    + HOW to optimize is a CS problem. But figuring out __WHAT__ to optmize is not 
        * e.g. 'people breathe air'

---
- Emebbding are good example of some common sense - task unrelated
    +   Agent communicate in natual language
- Too hard?
    + how u define problem
    + work starts to emmerge 




