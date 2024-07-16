Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 

To-Do:

1.  **Apply rec-nition & A-ttack on main Danish tweet corpus task**
    - Apply attack 
    - Save the scored dataset as csv on the o-drive (when on uni)
    
2. **Creating a dataset of reference tweets to prepare for hand coding and evaluate different classifiers on**
    - run the creating_dataset script again
    - create and save the 40% hateful, 40% prosocial, 20% random dataset
    - Pull the reference tweets for all the 10.000 replies using the twitter API
        - use ‘referenced_tweets_id’: what id this row is a reply or retweet of (I think???)
        - Look into documentation for this: https://developer.x.com/en/docs/twitter-api/data-dictionary/introduction (
            - academictwitteR (see mail)
    - Create a subset dataset of 200 paired tweets ready for hand-coding
        - will be coded in 3 labels
    - Look into danish (and english/multilingual) classifiers relevant for pro-social
        - [danish-foundation-models/munin-7b-alpha](https://huggingface.co/danish-foundation-models/munin-7b-alpha)
        - [perspectiveapi.com](https://www.perspectiveapi.com/)
        - Others?
    - Classifier competition: apply classifiers to the tweet/reply dataset 😎
        - compare the classifiers against our handcoded labels, and generally how they perform
    
3. Redoing and fine-tuning our existing english counter speech classifier
    - Check out repo - understand the contents
        - https://github.com/centre-for-humanities-computing/Counterspeech/tree/main/src
    - Use multilingual model like XLM-RoBERTA instead of English bert-base-uncased
    - Retrain the model (what server?)
    - Finetune on labeled danish examples (maybe 300 is enough?)
    - Finetune on labeled english examples (how many?)
