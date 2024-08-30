Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 


To-Do:

1. Task: Redoing and fine-tuning our existing english counterspeech classifier 
    - Check out repo - understand the contents
        - https://github.com/centre-for-humanities-computing/Counterspeech/tree/main/src
        - 3 models:
            - 01_Model without reference
                - Base model
                - Takes just a reference text (with no context of previous replies) and makes the predictions
            - 02_Model with reference
                - Builds on the base model
                - the model has more information to base its prediction upon as it can see patterns in the reference text and how this may influence the reply tweet text.
            - 03_Model with reference and text
                - Builds upon the second model
                - the model has more information to base its prediction upon as it can see patterns in the reference text AND THE REFERENCE LABELS and how this may influence the reply tweet text. (e.g., a hateful reference tweet is typically responded to with an 'Agree' tone in the reply or vice versa)
    - Use multilingual model like XLM-RoBERTA instead of English bert-base-uncased
        - Retrain the model (what server?)
        - ~~Test the models on smaller dataset and fewer epoch~~
            - Keeps crashing on 2 scripts, why?
    - Finetune the new model on labeled danish examples (maybe 300 is enough?)
        - OR should i train the whole model on the original data + extended with a new small sample of danish data (since we have to retrain the model anyways)
    
2. Task: Compare classifiers 
    - Compare the retrained classifier to the 2 hugging face ones (on the English data)
