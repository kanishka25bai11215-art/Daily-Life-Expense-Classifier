#  Daily Life Optimizer: Personal Finance Classifier

##  Overview
- Managing daily expenses manually can be time-consuming and error-prone. Many existing applications fail to correctly classify expenses, especially when dealing with local vendors or personalized spending habits.
- This project aims to solve this problem using **Machine Learning (NLP)** by automatically classifying user expenses into meaningful categories.

##  Objective

To build an intelligent system that:

* Takes expense descriptions as input
* Automatically classifies them into categories
* Reduces manual effort in expense tracking

##  Machine Learning Approach
* **Problem Type:** Text Classification (NLP)
* **Model Used:** Multinomial Naive Bayes
* **Feature Extraction:** TF-IDF Vectorization

##  Categories
The model classifies expenses into the following categories:

* 🍔 Food
* 🚗 Travel
* 💡 Bills
* 🛍️ Shopping
* 🏥 Health
* 🎬 Entertainment

##  Dataset

* Custom dataset with **500+ entries**
* Designed with **real-world Indian context**
* Includes vendors like:

  * Zomato, Swiggy
  * Uber, Ola
  * Amazon, Flipkart

### Sample Data

| Text             | Category |
| ---------------- | -------- |
| zomato 250       | Food     |
| uber ride 300    | Travel   |
| electricity bill | Bills    |

---

## ⚙️ Tech Stack

* Python
* Pandas
* Scikit-learn
* Google Colab

##  How to Run

### Step 1: Clone Repository

```bash
git clone <your-repo-link>
cd Daily-Life-Optimizer
```

### Step 2: Install Dependencies

```bash
pip install pandas scikit-learn
```

### Step 3: Run in Google Colab / Python

* Upload `expenses_500_plus.csv`
* Run the notebook or script

##  Model Workflow

1. Load dataset
2. Preprocess text data
3. Convert text → numerical features using TF-IDF
4. Train Naive Bayes model
5. Predict category

##  Example Predictions

```python
model.predict([
    "zomato dinner",
    "ola ride",
    "amazon shopping",
    "doctor visit"
])
```

### Output:

```
['Food', 'Travel', 'Shopping', 'Health']
```

---

## 📈 Results

* Achieved good accuracy on test data
* Model successfully identifies patterns in expense text
* Works well for common real-world inputs

##  Limitations

* Dataset is synthetic (not real user data)
* Limited understanding of complex sentences
* Accuracy depends on dataset quality

##  Future Improvements

* Add more real-world data
* Improve model using advanced NLP (like Logistic Regression / BERT)
* Add user feedback learning system
* Build a web/mobile interface

##  What I Learned

* Text preprocessing techniques
* TF-IDF vectorization
* Naive Bayes classification
* End-to-end ML workflow
* Importance of real-world datasets

##  Author

-  Name - Kanishka Rajput
-  Reg No. - 25BAI11215
---

##  Conclusion

This project demonstrates how machine learning can simplify everyday tasks like expense tracking. It highlights the power of NLP in solving practical problems and provides a foundation for building more advanced financial tools.

---
