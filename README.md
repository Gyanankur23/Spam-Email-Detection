# Spam Email Detector (Streamlit App)  
This project implements a Spam Email Detector using TF-IDF vectorization and a Linear Support Vector Classifier (LinearSVC).  
The app is built with Streamlit to provide an interactive interface where users can input email text and check if it is spam or not.  

## Features  
- Interactive Streamlit UI  
- Sidebar controls for model parameters: Test size for train/test split and Regularization parameter C for SVM  
- Displays model accuracy on sample dataset  
- Allows user to input custom email text and classify as Spam or Not Spam  

## Requirements  
Install dependencies with:  
`pip install -r requirements.txt`  

requirements.txt should contain:  
`streamlit`  
`scikit-learn`  
`pandas`  
`numpy`  

## Usage  
Run the app with:  
`streamlit run app.py`  
Then open the provided local URL (usually http://localhost:8501) in your browser.  

## Example Dataset  
The app uses a small sample dataset of emails:  
| Email Message | Label |  
|-------------------------------|-------|  
| Win a free iPhone now | Spam |  
| Meeting at 11 am tomorrow | Not Spam |  
| Congratulations you won lottery | Spam |  
| Project discussion with team | Not Spam |  
| Claim your prize immediately | Spam |  

## Notes  
- The model uses TF-IDF with unigrams and bigrams.  
- Labels: 1 = Spam, 0 = Not Spam.  
- You can extend the dataset by uploading or modifying the code.  

## License  
Released under the MIT License.  
