Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 


To-Do:

1. Task: **Creating a dataset of reference tweets to prepare for hand coding and evaluate different classifiers on task** 
    - Look into danish (and english/multilingual) classifiers relevant for pro-social
        - [danish-foundation-models/munin-7b-alpha](https://huggingface.co/danish-foundation-models/munin-7b-alpha)
        - [perspectiveapi.com](https://www.perspectiveapi.com/)
        - Ælectra models
        - Others?
        - https://github.com/fnielsen/awesome-danish
        - https://kennethenevoldsen.github.io/scandinavian-embedding-benchmark/
    - Test Zero-shot classification
    - Classifier competition: apply classifiers to the tweet/reply dataset 😎
        - compare the classifiers against our handcoded labels, and generally how they perform
        - when labeled: Multilingual-E5-large-instruct to classify tweets into containing prosocial/counterspeech or not
    
2. Task: Redoing and fine-tuning our existing english counter speech classifier 
    - Check out repo - understand the contents
        - https://github.com/centre-for-humanities-computing/Counterspeech/tree/main/src
    - Use multilingual model like XLM-RoBERTA instead of English bert-base-uncased
    - Retrain the model (what server?)
    - Finetune on labeled danish examples (maybe 300 is enough?)
    - Finetune on labeled english examples (how many?)
