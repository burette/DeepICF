# DeepICF
TensorFlow Implementation of Deep Item-based Collaborative Filtering Model for Top-N Recommendation

This is the official implementation for the paper as follows, which is based on the implementation of [NAIS](https://github.com/AaronHeee/Neural-Attentive-Item-Similarity-Model):
- **DeepICF: Deep Item-based Collaborative Filtering Model for Top-N Recommendation.**
Feng xue, Kai Liu, Xiang Wang, Jiandong Xu & Xiangnan He.

Two deep collaborative filtering models: **DeepICF** & **DeepICF+a**. To target the models for implicit feedback and ranking task, we optimize them using log loss with negative sampling.

**Please cite our paper if you use our codes. THX!**

## Environment Settings
- Python 2.7
- TensorFlow >= r1.0
- Numpy >= 1.12

## Examples to run the codes
Run **DeepICF**:

Output of **DeepICF**:

Run **DeepICF+a**:

Output of **DeepICF+a**:

## Dataset
We provide two processed datasets: MovieLens 1 Million (ml-1m) and Pinterest (pinterest-20).

**train.rating:**
- Train file.
- Each Line is a training instance: userID\t itemID\t rating\t timestamp (if have)

**test.rating:**
- Test file (positive instances).
- Each Line is a testing instance: userID\t itemID\t rating\t timestamp (if have)

**test.negative:**
- Test file (negative instances).
- Each line corresponds to the line of test.rating, containing 99 negative samples.
- Each line is in the format: (userID,itemID)\t negativeItemID1\t negativeItemID2 ...

Update Date: May 14th, 2018
