Group Members: Abigail Amiscosa, Joshua Ibrom, Julian Spindola  
Machine Learning

# Term Project- Week 2-3: Model Implementation & Initial Training

Our team has made significant progress in fine-tuning and hyperparameter tuning our models. Last week, we ran our BERT model against our baseline model (Convolutional Neural Network) and saw decent results. Since then, our focus has been on improving both models to see which one is best suited for our disaster tweets dataset.

**Experimentation and Results**

To improve the performance of our models, our team conducted the following experiments to analyze their results:

1. Experiment with CNNs’ **batch sizes** and **learning** **rates**
2. Experiment with CNN’s **architecture** (adding a convolutional layer)
3. Experiment with BERT’s **learning rate**

Let’s analyze each experiment one by one. First, we compared the accuracies and F1 scores of our CNNs across four different batch sizes and learning rate combinations. The results of this experiment can be viewed below:

| Configuration                       | Accuracy | F1 Score |
| :---------------------------------- | :------- | :------- |
| batch_size=16, learning_rate=0.001  | .8316    | .0681    |
| batch_size=16, learning_rate=0.0005 | .8259    | .0000    |
| batch_size=32, learning_rate=0.001  | .8259    | .0000    |
| batch_size=32, learning_rate=0.0005 | .8259    | .0000    |

Our first run of the CNN yielded an accuracy of 89.3%, meaning our new models are performing worse. The F1 scores also don’t seem to be calculated correctly, which may be a bug in our code. Our team plans to look into this and try to resolve this issue.  
Second, let’s examine our CNN with an added convolutional layer. This model performed better than the ones from our experiments, but is still shy of our original run (88.43% accuracy). I believe this underwhelming performance is due to our limited training time for each model. In each case, we only ran for a single epoch.  
Lastly, our team experimented with two different learning rates for our BERT model to identify the optimal one. The first learning rate we tested was 0.00002, yielding an accuracy of 92.5% after one epoch and an F1 score of 76.5%. Next, we tested a learning rate of 0.00003, yielding an accuracy of 91.29% and an F1 score of 71.95% after one epoch. These results were an improvement over our first run of BERT, reaching an accuracy of 92.4% after two epochs. If trained for more epochs, I’m sure this model would surpass our previous ones.  
**Next Steps**  
To complete our project strongly, our team will focus on training our models for more time and working on our deliverables (paper and presentation). While our model training is running, we will start building the pieces required for our paper and list core ideas for each section (related work, methodology, results, discussion, etc.). We will also look to incorporate a connection of our model to AI ethics for maximum transparency. We plan to build these ideas incrementally to hopefully deliver a well-written and executed paper. Our presentation will model our paper’s general structure and contain our project’s main takeaways and ideas.
