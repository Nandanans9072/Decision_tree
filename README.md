# Decision_tree
Decision Tree Builder with Gini Index
This notebook demonstrates how to build a decision tree classifier from categorical datasets using the Gini index for splitting.

You can use ant type od dataset


How It Works

Gini index is computed for each attribute split.

Attribute with lowest Gini (most homogeneous split) is selected.

Recursively build child nodes until leaves are pure or no attributes left.

Leaf nodes store the predicted class (majority class).


