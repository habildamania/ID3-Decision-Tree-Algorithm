# ID3-Decision-Tree-Algorithm
The original source code of this file belongs to Google Developers. The Source code provided by google developers is free to use and modify. I have modified the source code and added some ancillary features to it.
1. The original code provided by google developers was a decision tree using CART algorithm. I have modified it to make use of the ID3 algorithm. 
2. The measure of impurity has been changed from Gini Index to Entropy.
3. The Toy Dataset has been replaced by the Car Evaluation Dataset from UCI's Machine Learning Repository.
4. Sci-kit Learn's train test split is used to randomly split 80% of the Dataset for training and 20% for testing.
5. Each node has been assigned a unique node ID and additional information such as depth of the node and header information is being displayed at the node.
6. A function called Get_InnerNodes and Get_InnerLeafNodes is defined to display the inner nodes and the leaf nodes by their unqiue node ID.
7. A function called compute accuracy is defined to caculate the accuracy obatined on the test dataset.
8. Prunning is an important feature of any decision tree. Prunning decreases the complexity of the model, thereby avoiding overfitting. It also discards useless branches which thereby increases the accuracy of the model. Prunning was missing from the original Source Code. A function Named Prune_tree is added which Performs Post Prunning on the decision tree. It takes a user defined set of nodes and makes them the leaf of the tree thereby prunnning all its children nodes. 
9. By choosing the right set of nodes to pune, the accuracy on test is observed to increase before and after prunning.
