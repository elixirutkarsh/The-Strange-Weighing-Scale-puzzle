# The-Strange-Weighing-Scale-puzzle
Problem Statement:
You have a strange weighing scale with only one side. The scale doesn't display the actual weight of an object, but it has a special property: when you place any two objects on the scale, it will indicate whether the objects have the same weight or if one is heavier than the other. However, the scale does not tell you which object is heavier. You are given 9 identical-looking coins, and you know that one of them is counterfeit, either heavier or lighter than the rest. Your task is to identify the counterfeit coin using the scale, with the minimum number of weighings possible.

Solution:
Divide the 9 coins into three groups of three coins each, labeled A, B, and C. Weigh groups A and B against each other on the scale.

If A = B, it means the counterfeit coin is in group C. Move on to the next step.
If A > B, it means the counterfeit coin is in group A. Move on to the next step.
If A < B, it means the counterfeit coin is in group B. Move on to the next step.
Now, take the group containing the counterfeit coin (either A, B, or C) and pick any two coins from that group. Weigh these two coins against each other on the scale.

If the two coins balance each other, it means the remaining coin in that group is the counterfeit one. You have identified it.
If one coin is heavier than the other, the heavier one is the counterfeit coin.
