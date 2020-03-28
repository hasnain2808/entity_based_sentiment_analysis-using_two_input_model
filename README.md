# entity_based_sentiment_analysis-using_two_input_model

Compared to Image Classification this was a relatively new topic for me(sentiment analysis was not but entity based sentiment analysis was)<br>
I started by reading online that is why I came to know of various approaches and transformer based approach being the best<br>
My approach is as follows:<br>
Convert each of the input review and target entity to glove vectors<br>
Then the train and validation set were prepared<br>
The model that I designed by myself has two inputs (one for the review and other for the entity)<br>
After adding two bidirectional Lstm per input the values were concatened and followed by fully connected layer<br>
The initial intention was to use a attention layer like used with Question answering module(Calculate the attention of the entity with each word in the review)  but as I had only 3 hours for this question I was not able to complete it<br>
THe model is performing 80% accurate on the val set but is only outputting 2 to get that high level
