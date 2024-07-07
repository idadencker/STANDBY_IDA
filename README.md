Link to my notion page 'STANDBY' containing notes on e.g. the the facebook experiment study design, formulated research questions, data dictionary explaning variables in the json files and the 'desired_data_structure.xlsl'  : https://www.notion.so/STANDBY-e7809ca5ae104139a002c415fdfbdcc8?pvs=4 

To-Do:

1.  **Apply rec-nition & A-ttack on main Danish tweet corpus task**
    - Save the scored dataset as csv on the o-drive (when on uni)
    - OBS: @user1234 is part of the ‘text’ column that algorithms is applied to: should these be removed prior?
    
2. **Creating a dataset of reference tweets to prepare for hand coding and evaluate different classifiers on**
    - ~~New folder in GitHub for this task~~
    - ~~Load scored csv file into new python script~~
        - ~~filter to replied_to~~
        - ~~Look into examples of attack and recognition examples: how does the classifier perform?~~
        - ~~limit to approx 10.000~~
            - ~~Approaches to limiting:~~
                - ~~¼ are scored 0-0 for attack-recnition; ¼ are scored 1-0 for attack-recnition, ¼ are scored 0-1 for attack-recnition, ¼ are scored 1-1 (possible that there are no/few examples that have both attack AND rec-nition labels) for attack-recnition~~
                - ~~wordembeddings: based on cosine similarity for a hateful sentence and a prosocial sentence (tf-idf, bert, roberta, fasttext)~~
                    - ~~Calculate a similarity number (vector) for each row based on scoring of a hateful sentence measuring how close the tweet is to the word embedding for that hateful sentence~~
                    - ~~Calculate a similarity number (vector) for each row based on scoring of a prosocial sentence measuring how close the tweet is to the word embedding for that prosocial sentence~~
                    - 40% hateful, 40% prosocial, 20% random
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
