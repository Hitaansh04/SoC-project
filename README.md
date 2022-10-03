# SoC-project
We started SoC learning with the know how's of Time Series and datas and learnt a lot of new definitions such as metrics/events/ cross sectional data. Also,I saw what to look for in time series datas at first sight such as trends, cyclic fluctuations and seasonal patterns. Later,I was introduced to a lot of traditional time series forecasting methods and where did they originate from such as Autoregression, moving average, seasons and based on this learnt various models such as ARMA and going all the way to the vectorised approach such as VARMAX. This week was particularly fun and challenging since I didn't have prior experience of working with so many libraries at once. We stepped up the pace in Week 3 going into the fundamentals of Deep learning and it's frameworks,also saw the common approaches to optimise an algorithm such as loss function/gradient descent.I also got introduced to tensorflow's Keras API and was surprised with how easier it was with Keras.

I started getting acquainted with Neural networks and the math behind it.It involved a bit of linear algebra and I finally got to know the meaning behind weights,biases, regularisation, forward and back propagation and also loss functions. To implement them using Tensorflow was particularly challenging and I had to practice more to get used to it. Overall, this was my progress so far till the checkpoint 1. 

Next, I made my first 3D CNN on CT-scans to classify lung-tumours. Before making the model,the scans involved a lot of pre-processing too to ensure all of them are aligned in the same manner. I was introduced to pooling methods and the number of features were so large that a single epoch took about 20 mins to process. I learnt from my mentor that a GPU would give much faster results. 

In week 6, I read the research paperhttps://www.sciencedirect.com/science/article/pii/S0957417419301915
thoroughly and understood the thought process behind coming up with such an implementation of the timed-series data. I realized what were the shortcomings of traditional baseline algorithms. I also saw how maximum feature extraction can be made possible through pooling. In the end, I made a two page docx summarizing all my learnings through the paper. 

By week 7, it was finally time to start working on the actual Project. The entire week was spent on data pre-processing / data-cleansing / feature engineering the dataset. I started working primarily with the Dow-Jones Index . I correlated multiple columns from different datasets and kept those in my final dataframe which had the least correlation amongst them.

Furthermore, applied scaling and normalization techniques , so that all values lie between -1 and 1. Lastly, began building my model with the customized dataframe of mine as the dataset.
Building the model was an extensive process and consumed a lot of time as I tried to ensure that the shape of the input was a valid one in each layer. I tried and tested various filter sizes and came to the conclusion that (8,8,8) sized filter is best suited. 

Later, I tried a different approach for data gathering by generating each input chosen randomly out of an option from 5 market indices and I found out there was a significant betterment on the training data. Lastly, I put the model through the test set and achieved an F-score of 0.5477 which is just slightly short of the one on the research paper which had 0.56 as it’s F-score.


