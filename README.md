Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 


To-Do:

1. Task: Redoing and fine-tuning our existing english counterspeech classifier 
    - Counterspeech repo - https://github.com/centre-for-humanities-computing/Counterspeech/tree/main
    - New code for model without ref (multiclass) + test it
    - New code for model with ref (multiclass) + test it
    - When those works as intended:
        - Train the 2 models on bigger ucloud machine (full data + more epochs)
    - When danish data is avialable:
        - Finetune the 2 models
        - (consider: should i train the whole model on the original data + extended with a new small sample of danish data (since we have to retrain the model anyways))

1. Look into and test hugging face Debate model
- https://huggingface.co/mlburnham/Political_DEBATE_large_v1.0
- Apply the political debate model to data
    - try finetuning large on counterspeech data

1. Task: Compare classifiers 
- Compare the 2 retrained classifiers to the 2 hugging face ones (on the English data) (+ possibly other ones)
