Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 



To-Do:

1. Task: **Creating a dataset of reference tweets to prepare for hand coding and evaluate different classifiers on task** 
    - ~~Look into danish (and english/multilingual) classifiers relevant for pro-social/counterspeech~~
    - ~~Classifier competition: apply existing classifiers to the tweet/reply dataset~~
    - ~~Finetuning LLM on counterspeech (CONAN) data~~
    - Maybe handcode a small dataset myself and finetune a hugging face counter speech classifier
    - Apply perspective API
    - compare the classifiers against our handcoded labels, and generally how they perform
    
2. Task: Redoing and fine-tuning our existing english counter speech classifier 
    - Check out repo - understand the contents
        - https://github.com/centre-for-humanities-computing/Counterspeech/tree/main/src
    - Use multilingual model like XLM-RoBERTA instead of English bert-base-uncased
    - Retrain the model (what server?)
    - Finetune on labeled danish examples (maybe 300 is enough?)
    - Finetune on labeled english examples (how many?)
