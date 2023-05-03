# prompt-engineering-course-notes
Notes from ChatGPT Prompt Engineering for Developers course 

Link to course (free): https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/


* Intro
    * principles: 
        * clarity + specificity (what, how - tone), 
        * giving LLM time to think
* L2: guidelines
    * Notebook: https://s172-31-7-142p49608.lab-aws-production.deeplearning.ai/notebooks/l2-guidelines.ipynb 
    * principle 1: clarity (clear != short)
                * tactic1: use delimiters (“””, ```, —, <>, xml tags <tag></tag>
                * tactic2: use structured output (json, html)
                * tactic3: check conditions, assumptions required to do the task, fail gracefu
                * tactic4: few shot prompting (many examples)
    * principle: give it a time to think
        * tactic1: split task into smaller, specific 
        * tactic2: instruct model to work out it’s own solutions
    * Model limitation
        * hallucinations
            * reduce: find relevant snippet, then answer question
* Iterative prompt development
    * Notebook: https://s172-31-10-136p47160.lab-aws-production.deeplearning.ai/tree
    * add context: 
        * limit the length of the output
        * target audience
        * expected format
            * general structure (e.g. end with call to action)
            * insert table
            * html ?
    * evaluate against the larger batch of example
* Summarizing
    * https://s172-31-9-59p32412.lab-aws-production.deeplearning.ai/notebooks/l4-summarizing.ipynb
    * specify the target audience
    * extract the relevant info
    * loop over multiple items
* Inferring
    * https://s172-31-9-147p57812.lab-aws-production.deeplearning.ai/notebooks/l5-inferring.ipynb
    * extract labels, name, sentiment - previously with custom ML/NLP models, LLM generalise well
    * identify emotions, detect anger
    * extract json: product, brand
    * combine many entities + json  
    * extract topics
* Transforming
    * https://s172-31-6-55p28640.lab-aws-production.deeplearning.ai/notebooks/l6-transforming.ipynb
    * translate 
        * to X
        * identify language
        * translate to slang, formal, informal - multiple outputs from one prompt
        * loop over many examples
    * tone of voice
        * slang to business language
        * convert document formats: json to html
    * proofread and correct
        * spell check, grammar errors
        * Redlines package to identify diffs between texts
        * APA style, target audience literacy
* Expanding
    * https://s172-31-15-196p53874.lab-aws-production.deeplearning.ai/notebooks/l7-expanding.ipynb
    * brainstorming but also spam
    * personalised email 
        * different response based on sentiment
        * good practice: sign transparently as “ai assistant”
    * temperature parameter
        * 0 - low chance of deviating from the most expected answer (use for high predict
* Chatbot
    * https://s172-31-1-68p47876.lab-aws-production.deeplearning.ai/notebooks/l8-chatbot.ipynb
    * list of messages vs single prompt as “user”
    * system, assistant <—>  user
    * no memory by default, unless we pass all the previous messages
    * example: pizza order chatbot
        * system: process steps, menu



