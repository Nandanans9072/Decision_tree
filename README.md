# **🧩 `Decision Tree Builder (Gini Index)`**

Build decision tree classifiers from categorical datasets using the Gini index. This notebook works with any categorical dataset and provides both textual and graphical tree representations.

🚀 How It Works

Compute Gini Index: Calculates the impurity for each possible attribute split.

Choose Best Attribute: Selects the attribute with the lowest Gini (most homogeneous split).

Recursive Tree Building: Creates child nodes until:

All samples belong to one class, or

No attributes remain for splitting.

Leaf Nodes: Store the predicted class based on majority voting.

✨ Features

Multi-way splits for categorical attributes.

Handles small to medium datasets.

Textual Tree: Easy to read hierarchical structure.

Graphical Tree: Visualize using Graphviz in Colab or Jupyter.

📊 Example Use Cases

Predict Job Offers based on CGPA, Practical Knowledge, Communication Skills.

Predict Sunburn risk based on Hair, Height, Weight, and Lotion usage.

🔧 Usage

Load your dataset into a pandas DataFrame.

Specify the target column.

Build the tree:

tree = build_tree(data, target='Job_Offer')
print_tree(tree)          # Text view
graph = visualize_tree_graphviz(tree)
display(Source(graph.source))  # Visual view
