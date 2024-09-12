Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 


To-Do:

1. Task: Redoing and fine-tuning our existing english counterspeech classifier 
    - Counterspeech repo - https://github.com/centre-for-humanities-computing/Counterspeech/tree/main
    - Use multilingual model XLM-RoBERTA-large instead of English bert-base-uncased
        - Retrain the models (what server?)
        - ~~Test the models on smaller dataset and fewer epochs~~
    - Test a saved model on some data: how does it works?
    - Finetune the new model(s) on labeled danish examples (maybe 300 is enough?)
        - OR should i train the whole model on the original data + extended with a new small sample of danish data (since we have to retrain the model anyways)

2. Look into and test hugging face Debate model
- https://huggingface.co/mlburnham/Political_DEBATE_large_v1.0

3. Task: Compare classifiers 
- Compare the retrained classifier to the 2 hugging face ones (on the English data)
