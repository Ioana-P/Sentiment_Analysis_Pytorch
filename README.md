# Sentiment Analysis Pytorch
Training and deploying a Sentiment Analysis model in Pytorch using AWS Sagemaker. The data used was IMDB's Movie review dataset (https://ai.stanford.edu/~amaas/data/sentiment/), which consists of 50,000 instances of binary labelled movie reviews.

My foci for this project were a) developing my **understanding of successful model deployment on AWS Sagemaker** and b) practicing writing a **neural network model in pytorch** and the appropriate data preprocessing functions for it. Given that this is a widely-used, canonical dataset, model performance was less of a priority (although the 85% accuracy certainly feels pleasing). To that end I'm including below a mind-map of the architecture  (Figure 1).



![mind-map](https://github.com/Ioana-P/Sentiment_Analysis_Pytorch/master/fig/sentiment_analysis_aws_flow.jpg)

Fig 1 - Mind map showing how a Sagemaker notebook instance containing a Pytorch model interacts with an API, Lambda function and webapp




A basic webapp, API and Lambda function were written for this project as well but are non-functioning as having these hosted on Sagemaker incurs significant costs. If you're interested in replicating the project, the code here was tested while the S3 buckets and notebooks were still fully functioning so everything should run if cloned to a Sagemaker notebook instance perfectly, asuming all files are copied over. 




References:
Data - 
Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011). 
