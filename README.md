# Sentiment-Analysis
# Student Remark Sentiment Classifier (BERT)

This project features a fine-tuned **BERT-base-uncased** model designed to classify student feedback into **Positive**, **Negative**, and **Neutral** categories. 

A key highlight of this project is its ability to understand **Standard English** alongside **Nigerian Pidgin**, making it highly effective for regional academic feedback systems.

---

## Live Demo
Click the badge below to open the notebook and test your own sentences (e.g., *"The oga teacher sabi well well"*).

[Open In Colab](https://colab.research.google.com/github/ufedoabdul4-coder/Sentiment-Analysis/edit/main/cleaned_notebook.ipynb)

---

## Project Features
* **Bi-lingual Support:** Custom templates for English and Nigerian Pidgin (e.g., "sabi teach," "no gree," "naso it suppose be").
* **Advanced Neutral Handling:** Solved common sentiment bias by training the model on 300+ factual and "middle-ground" neutral statements.
* **Modern NLP Stack:** Built using `Hugging Face Transformers`, `PyTorch`, and `Evaluate`.
* **Clean Deployment:** Includes a metadata-stripping script to ensure the notebook displays perfectly on GitHub without widget errors.

## Performance & Evaluationprint(predict_sentiment("im quite dissapointed in the teachers teaching method"))
### Sample Predictions
| Text | Predicted Sentiment |
| :--- | :--- |
| "I think Mr. Fidelis is useful." | **Positive** |
| "She dey rush the class too much." | **Negative** |
| "The new teacher is just there." | **Neutral** |
| "I don't like the way the class is going." | **Negative** |

---

## How to Test Your Own Sentences
Run the Setup: Open the Colab link and run the first block of code. This installs the necessary libraries and loads the BERT model.

Predict Sentiment: Scroll to the bottom of the notebook (or create a new cell) and use the following command:

Python
print(predict_sentiment("INPUT STATEMENT HERE"))
Get Results: The model will immediately output Positive, Negative, or Neutral based on your input.

