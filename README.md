# Tree-Augmented-Naive-Bayes-TAN-Classifier-for-Multi-Label-Classification


## Prologue

Implementation code of Tree Augmented Naive Bayes (TAN) classifier for multi-label classification tasks in a large sparse dataset using  mutual information and Kruskal's algorithm.  We perform data preprocessing, feature selection, TAN structure construction, parameter estimation, and classification. We evaluate the classifier's performance in terms of Time and Precision@1 


## Requirements

- Python 3.x
- NumPy
- scikit-learn
- Joblib

Install the required packages using:

- pip install numpy scikit-learn joblib

similarly install other requirements


## Usage

Run the script with the following command:

- python B22AI059_3.py <train_file> <test_file>


- `<train_file>`: Path to the training data file.
- `<test_file>`: Path to the testing data file.

## Example
 - python B22AI059_3.py eurlex_train.txt eurlex_test.txt

Note: Ensure that your data files are in the correct format as described below.

## Output

The script outputs:

- Precision@1: Percentage of test samples where the top predicted label matches one of the true labels given in test dataset of each sample.
- Execution Time: Total time taken to run the script.

Note that in the code You can change values of parameters like max_parents , no. of bins , no. of features selected and can do various experiment.


Sample Output:

Training data Loading...
Training data: 5000 samples, 10000 features, 50 labels
Test data loading...
Test data: 1000 samples
Selecting top 300 features...
Computing label priors...
Data matrix formulations ...
Discretizing the features...
Computing Mutual Information...
Building TAN structure...
Calculating bin edges...
Training and parameter updation...
Training completed.
Starting of parallel prediction...
Evaluating predictions and Precision@1...
Precision@1: with 1 max parents = 28 %
Total execution time: 240 seconds

## License

This Assignment was done by Yashraj Chaturvedi (B22AI059) for course Artificial Intelligence, Autumn 2024, IIT Jodhpur
