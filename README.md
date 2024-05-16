# Natural Language Processing with Disaster Tweets
https://www.kaggle.com/competitions/nlp-getting-started/overview

## Submission #1
- 3 Epochs
- No location data was included in the training data
- Score: 0.82102
    - Pretty solid score

## Submission #2
- 10 Epochs
- Uses location data
- Score: 0.83113
    - Not as high as I hoped
    - Likely due to faulty data in training

## Submission #3
- 10 Epochs
- Uses location data
- Cleaned Data
    - Removed duplicate rows (about 3% of original training data)
    - Removed locations that were not real places
- Score: 0.83481
    - Smaller impovement than expected
    - Cleaning the data did not impact the data as much as expected

## Ideas for improvement
- use the bert-base-cased model instead
    - Upper case could be meaningful data
    - Current model of bert-base-uncased only works with lower case text
- Place greater emphasis on the location during training
    - Small improvement after introducing location data to training implies that the location data is not being prioritized effeciently by the model
