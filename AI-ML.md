# 1. What is AI?
AI (Artificial Intelligence) is the ability of machines to perform tasks that normally require human intelligence like reasoning, learning, and decision-making.

# 2. What is Machine Learning?
ML is a subset of AI where systems learn patterns from data without being explicitly programmed.

# 3. What are the types of ML?
- Supervised Learning (labeled data)
- Unsupervised Learning (unlabeled data)
- Reinforcement Learning (reward-based learn

# 4. What are the types of unsupervised learning?
Clustering (k means), Dimension reduction

# 5. What is K mean clustering?
Random k no. of points are chosen (say 3). Now say there are 3 fruits. The algo might or might not know the no. of points. It might incorrect assume there are 4 points too. Either way, nearby points are assigned to each of these 3 points in a cluster by calculating Euclidean distance. Then mean is calculated and process is repeated until 3 fruits (say apple, banana & mango are identified).

# 6. What are the types of supervised learning?
Classification and regression

# 7. What is Cost function analysis?
For each data point, Error = Actual - Predicted
But for total error, Positive and negative errors can cancel each other out. Positive and negative errors can cancel each other out. So, we use different mathematical methods to calculate the cost.
A Cost Function is a mathematical function that measures the overall error of a machine learning model over a dataset. Cost function measures how well model parameters fit thr training data by quantifying prediction error.
There are several cost functions depending on the machine learning problem. E.g. Mean Squared Error

<img width="236" height="85" alt="image" src="https://github.com/user-attachments/assets/abef2c25-2029-42f7-86dc-46fcac23f860" />

# 8. What is the Statistical Approach?
It is a method of Pattern Recognition. Pattern recognition is the process of identifying and classifying objects based on their features. The statistical approach uses mathematical and statistical techniques to identify patterns and classify data based on their features and probability distributions. E.g to distinguish between two flowers, Class A generally has smaller petal dimensions. When a new flower is introduced, The computer examines the characteristics and determines that it is more likely to belong to Class B.

A pattern class is a category to which an object belongs. For example: C={A,B}. Here say A is rose & B sunflower.

# 9. What is soft computing?
Say, in order to recognise handwritten digits, handwriting might be unclear, fuzzy, noisy, Two different digits might look very similar etc. A traditional system that relies on strict rules may struggle with such imperfect information. Typically, traditional hard-computing algorithms heavily rely on concrete data and mathematical models to produce solutions to problems. We need a computational approach that can work with uncertainty, approximation and imprecision.

Soft Computing is a collection of computational techniques that deal with uncertainty, imprecision, approximation and incomplete information to solve complex problems.  Fuzzy logic is a computational paradigm that entertains the uncertainties in data by using levels of truth rather than rigid 0s and 1s in binary. Next, neural networks which are computational models influenced by human brain functions. Finally, evolutionary computation is a term to describe groups of algorithm that mimic natural processes such as evolution and natural selection.  Key points include tackling ambiguity, flexible learning, grasping intricate data, real-world applications, and ethical artificial intelligence

# 10. What is Perceptron?
perceptron is an algorithm for supervised learning of binary classifiers.
In simple terms, a perceptron is a mathematical model that imitates the basic working principle of a biological neuron. It receives inputs, processes them, and produces an output.
For example, imagine a machine that has to decide whether an email is:
- Spam (+1)
- Not spam (−1)

# 11. What is feature exctraction/ engineering?
Process of finding deterministic character of an object
