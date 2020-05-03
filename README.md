# Analyzing 10Gb of Yelp Reviews Data

I analyzed a subset of Yelp's business, reviews and user data. This dataset comes to us from [Kaggle](https://www.kaggle.com/yelp-dataset/yelp-dataset) and I upload this data into a publis s3 bucket: 
`s3://sta9760-spark-datasets2/*business.json`
`s3://sta9760-spark-datasets2/*review.json`
`s3://sta9760-spark-datasets2/*user.json`

The analysis uses AWS EWR infrastructre to operate on the large data set. It first set an EWR cluster on AWS and corresponding spark application, and create a jupyper notebook with pyspark kernel on top it. Then I set up the S3 bucket to store the large data set. 

After uploading up data, it uses pyspark to load the data into spark session from S3 bucket, and conducts transformation and action operation in pyspark to do each individual analysis. 

## S3 pages are here.
![notebook](https://github.com/SherlockZhang/Analysis_of_10GB_Yelp_data_Xin_Zhang/blob/master/assets/EWR_S3.png?raw=true)

## Cluster and Notebook Configs
![notebook](https://github.com/SherlockZhang/Analysis_of_10GB_Yelp_data_Xin_Zhang/blob/master/assets/EWR_Cluster.png?raw=true)

![notebook](https://github.com/SherlockZhang/Analysis_of_10GB_Yelp_data_Xin_Zhang/blob/master/assets/EWR_notebook.png?raw=true)

