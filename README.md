Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 



1. Task: Redoing and fine-tuning our existing english counterspeech classifier 
    - Can i do some changes to improve model performance
    - Add docsstrings (save for when out of GPU)
    - Try other transformer models as base (see mail)
        - e.g. DEBATE model: https://huggingface.co/mlburnham/Political_DEBATE_large_v1.0
    - Finetune the 2 models on danish data (when available)
        - (consider: should i train the whole model on the original data extended with a new small sample of danish data OR take the trained model and then fine-tune on danish)

2. Task: Compare counter speech  classifiers 
    - Compare the 2 retrained classifiers to the 2 hugging face ones (on the English data)
    - Compare to other ones if there are any?
