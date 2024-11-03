java c
AD699: Data Mining for Business Analytics 
Individual Assignment #4 
Fall 2024
You will submit two ﬁles:
(1) a PDF with your write-up, along with
(2) the script you used to generate your results.Task 1: Association rules For this portion of the assignment, we will be using data from Groceries, a dataset that can be found with the arules package.   Each row in the ﬁle represents one buyer’s purchases.    This link provides some helpful templated examples for generating association rules:
http://r-statistics.co/Association-Mining-With-R.html 
1.     Describe “Groceries” by answering following questions:
● What is the class of “Groceries”? 
● How many rows and columns does Groceries contain?
2.   Generate an item frequency barplot for the grocery items with support rate greater
than 8.5%. Include a screenshot of your results, along with the code you used to do this. Orient this plot horizontally, and ﬁll the bars with any color of your choice.
3.   Now,  create a subset of rules that contain your grocery item (you can ﬁnd your item  in the  spreadsheet in Blackboard). Select any one rule with your item on the left-hand side, and any one rule with your item on the right-hand side, and explain them in the way you would explain them to   your roommate (I’m assuming your roommate is a smart  person  who  is  unfamiliar  with  data  mining). Remember,  every  rule has four components: support, coverage, conﬁdence, and lift.For  each  of your  chosen  rules  (your grocery item on the left-hand  side, and your grocery item on the right-hand side), include a screenshot of your rules, along with the code you used to generate the rules.
4.   In a sentence or two, explain what meaning these rules might have for a store like Star Market. What could it do with this information?
5.   Using the plot() function in the arulesViz package, generate a scatter plot of any three rules involving your grocery item.   Include a screenshot of  your plot, along with the code you used to generate the plot.  Describe your results in a sentence or two.
6.   Again using the plot() function in the arulesViz package, generate a plot for any three of your  rules.   This time,  add two  more arguments to the function:   method="graph", engine="htmlwidget"   What do you see now?  Include a screenshot of your plot, along with the code you used to generate the plot. Describe your results in a sentence or two
–  what is  diferent about this plot, compared to the  one that you generated in the previous step?
Task 2: Classiﬁcation Tree 
1.    Bring the dataset CreditCard from the AER package into your R environment.
2.   Use the head() function to get a sneak preview of your dataset, and spend a few minutes exploring the  data.   In  about 3-4  sentences,   how  can you  summarize this dataset? What does it seem to be about?
3.   The  response  variable  in  our  model  for this  section will be ‘card.’   If ‘card’ is  not currently代 写AD699: Data Mining for Business Analytics Individual Assignment #4 Fall 2024Matlab
代做程序编程语言 a factor variable, convert it into a factor.
a.   What is the balance among the levels for card?   In the full dataset, how many ‘no’ and how many ‘yes’ outcomes are there?
4.   Using your seed value (from Assignment 2), partition your data into training (60%) and validation (40%) sets. Show the step(s) that you used to do this.
5.   Build a tree model with this dataset, using card as your outcome variable.
6.   Use rpart.plot to display a classiﬁcation tree that depicts your model.  (If the tree model is hard to see or read, that’s okay...but if you wish to change it, you can try changing some settings, such as cex, fallen.leaves, and varlen).
a.   Then, adjust the way your model looks.  Don’t change anything about the model itself, but use a new combination of values for ‘type’ and/or ‘extra’ in rpart.plot to change the appearance of the tree.
b.   Try yet another alternative way of viewing your model.  Show your results.
c.   Now, write  a couple  of sentences about what you saw with each of the three graphical versions of your model. Which one do you like best, and why?
7.   Describe the split that’s created at your tree’s root node (what variable did it split on, and what rule did it use?). Why is the root node  signiﬁcant?
8.   Did all the input variables from the dataset appear in your model diagram?  If not, why not?
9.   Describe any one rule that your tree generates regarding whether an applicant will be  approved for a credit card.  To describe a rule, just trace any path along your tree from the root node to a terminal node.
10.  Now, build another tree model.  This time, set a complexity parameter of 0, and use  minsplit =2,  to make the tree as large as possible.   Show what your overﬁttree looks like, using rpart.plot.  Don’t worry about interpreting this tree – just show it.
11. Using ﬁve-fold cross-validation, determine the optimal complexity parameter (cp) for a tree model built with your training data.  Demonstrate this by showing your cptable and stating which cp value you chose.
12. Generate a new tree model, with the cp value that you found previously.
13. Use rpart.plot to show your new tree model (the pruned tree).  Show this with your preferred “type” and “extra” settings in rpart.plot.
14a. Create confusion matrices in R to assess the performance of your huge tree against your training and validation sets. How did it perform?
b. Now, create confusion matrices to assess your optimally-sized tree model (the one that you built after cross-validation).  How was this optimally-sized model’s performance against the training and validation sets?  What happened to the diference between the two accuracy values as you went from the huge tree to the optimal one? 
c. Why would it be reasonable to expect that the diference between training set accuracy and validation set accuracy would decrease when using a pruned tree?







         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
