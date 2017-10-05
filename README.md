# MBTI-Predicting-RNN
In this project, a RNN is used to predict the Myers–Briggs Type Indicator (MBTI) of a person, based on their posts on social media.
The dataset for this problem can be found at https://www.kaggle.com/datasnaek/mbti-type

# Description

---
## About MBTI 

*From the dataset website*

>The Myers Briggs Type Indicator (or MBTI for short) is a personality type system that divides everyone into 16 distinct personality types across 4 axis:

>Introversion (I) – Extroversion (E)
Intuition (N) – Sensing (S)
Thinking (T) – Feeling (F)
Judging (J) – Perceiving (P)
(More can be learned about what these mean here)

>So for example, someone who prefers introversion, intuition, thinking and perceiving would be labelled an INTP in the MBTI system, and there are lots of personality based components that would model or describe this person’s preferences or behaviour based on the label.

>It is one of, if not the, the most popular personality test in the world. It is used in businesses, online, for fun, for research and lots more. A simple google search reveals all of the different ways the test has been used over time. It’s safe to say that this test is still very relevant in the world in terms of its use.

>From scientific or psychological perspective it is based on the work done on cognitive functions by Carl Jung i.e. Jungian Typology. This was a model of 8 distinct functions, thought processes or ways of thinking that were suggested to be present in the mind. Later this work was transformed into several different personality systems to make it more accessible, the most popular of which is of course the MBTI.

>Recently, its use/validity has come into question because of unreliability in experiments surrounding it, among other reasons. But it is still clung to as being a very useful tool in a lot of areas, and the purpose of this dataset is to help see if any patterns can be detected in specific types and their style of writing, which overall explores the validity of the test in analysing, predicting or categorising behaviour.

---
## About Dataset

The dataset contains 8675 samples, where each sample consists of the person's MBTI and their last 50 posts. The posts are seperated by '|||'.

---
## Solution

In this problem, a RNN containg 256 units is used. The last unit is connected to a fully connected layer (ReLU activated) which is connected to another fully connected layer (softmax activated) consisting of 16 units in order to classify a post into 16 different MBTI types.

 
