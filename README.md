# My-Decision-Tree--INF264-Project-1
This is my handin to the first mandatory assignment for the INF264 (Introduction to machine learning) course at UiB 

The program is all run within the jupyter notebook file. (My decision tree Ketil Fagerli Iversen.ipynb)
Remember to have the data_banknote_authentication.txt file in the same folder as where the jupyter notebook is saved.

The jupyter notebook already creates, prints, predicts and computes the accuracy on several decision trees.
However if you want to create your own tree and run your own data through it, do the following.

-To create a decision tree using my implementation:

1. Run all the cells in order and wait (possibly for a while) for everything to run
2. Open up a new cell at the bottom
3. Type something like;

My_custom_tree = learn(training_features, training_labels, impurity_measure, prune)

Where training_features are the training features, training_labels are the training labels, impurity_measure can either be 'entropy' or 'gini',
and prune can either be True or False. 'My_custom_tree' is just a placeholder name and you can name it whatever you like.
Running this will make a decision tree and store it in My_custom_tree. 




-To print the decision tree, type the following into an empty cell:

tree_printer(My_custom_tree)




-To predict the label of a single datapoint, type the following

predict(example, My_custom_tree, print_progress)

Where example is a single row of feature data (can also be feature data + the column with the actual label, it doesnt matter)
print_progress is by default set to False, but you can set it to true for it to give you how it got to its conclusion




To get the accuracy of the decision tree, type the following

predict_data_accuracy(data_features, data_labels, node)

Here data_features are the features of the dataset, data_labels the corresponding labels and then node is the decision tree,
subtree, or node you wish to do the prediction on.


