## RStudio-Autopilot-diabetes

Description:

In this notebook, we are going to train a Machine Learning classification model using Amazon SageMaker Autopilot, on the diabetes dataset found here: https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008#
The goal of this problem is to classify whether a patient is going to be readmitted to the hospital due to diabetes related problems, given various test results, previous diagnosis, demographics and previous admission related data. More information on the dataset can be found in the url posted above and the articles sited on the site.

We will carry out the following tasks in this notebook:

1. Set up required packages, Amazon SageMaker Python SDK, role, session and Amazon S3 bucket
2. Download the data, do simple preprocessing and store the data in an S3 bucket for model training
3. Setup and run the SageMaker AutoPilot job with a number of candidates. Each candidate consists of some auto feature engineering steps and a machine learning algorithm picked to run a trial
4. Select the best candidate out of all the models trained based on a objective metric
5. Run batch inference using the best candidate on the test data set
6. Display various metrics like accuracy, sensitivity, accuracy, F-1 score and confusion matrix
7. Plot the receover operating characteristic (ROC) curve using the best model on the test dataset

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

