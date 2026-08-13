# Customer Churn Prediction — Simple Demo

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Streamlit-blue)](https://churnmodellingannclassification-dsdaxl5d4p33unux5j2kcz.streamlit.app/)  https://churnmodellingannclassification-dsdaxl5d4p33unux5j2kcz.streamlit.app/

This project is a small, user-friendly demo that predicts whether a bank customer is likely to stop using the service ("churn"). It includes a ready-to-run web app you can open in your browser and use by entering a few customer details.

No coding skills are required to try the demo — just install the listed requirements and run the app.

## Try it (quick steps)
1. Install required Python packages:

```bash
pip install -r requirements.txt
```

2. Start the application locally:

```bash
streamlit run app.py
```

3. A browser window will open (or visit http://localhost:8501). Enter simple customer details like Geography, Gender, Age, Balance, Credit Score, and the app will show whether the customer is likely to churn.

4. Alternatively, try the hosted live demo (no install required):

https://churnmodellingannclassification-dsdaxl5d4p33unux5j2kcz.streamlit.app/

## What the app does (plain language)
- You fill a short form with basic customer information (age, location, gender, balance, etc.).
- Behind the scenes, a trained machine learning model looks at those values and returns a single result: "likely to churn" or "not likely to churn." 
- The app also uses small helper files to make sure inputs are interpreted correctly (for example, converting location names into the format the model expects).

## Files included (what they mean)
- `app.py` — The simple web app you run with Streamlit. It shows the form and displays the prediction.
- `model.keras` — The trained prediction model. This is the piece that makes the churn decision.
- `scaler.pkl` — A helper file that scales number inputs so they match how the model was trained.
- `label_encoder_gender.pkl` — A helper that converts the written gender into the numeric form the model expects.
- `onehot_encoder_geo.pkl` — A helper that converts the chosen geography into the format the model expects.
- `requirements.txt` — A short list of Python packages needed to run the app.
- `LICENSE` — The project license (GNU GPL v3).

## Who might use this
- Product managers or business stakeholders who want a quick demo of how customer data can indicate churn risk.
- Anyone curious about how a small, interactive prediction app works without getting into code.

## Notes and safety
- This demo uses a pre-trained model included in the repository; it is for demonstration only and may not be accurate for real-world decisions.
- Do not supply real personal data when trying the demo on public machines or shared environments.

## Questions or feedback
If something doesn't work, open an issue in this repository or contact the repository owner.
