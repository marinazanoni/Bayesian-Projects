# 🚴 Riding Data Waves - A Bayesian Model for Bicycle Incident Analysis  

## 📌 Overview  
This project applies Bayesian modeling to classify bicycle accident injuries using real-world data.  
A multinomial logistic regression model is developed and analyzed with MCMC simulations.  
The results are compared with frequentist methods, and model performance is evaluated through diagnostic tests.  

## 📊 Dataset  
The dataset is sourced from Kaggle and contains 57 variables, primarily categorical.  
It includes factors related to cyclists, drivers, road conditions, and environmental variables.  
Key preprocessing steps included:  
- Removing unknown values in injury severity  
- Addressing class imbalance through resampling  
- Feature engineering for variable selection  

## 📈 Bayesian Model  
The project implements a **multinomial Bayesian logistic regression model**, where injury severity is predicted based on various factors.  
- **Model Estimation**: Uses MCMC methods (JAGS) to estimate parameters  
- **Inference**: Bayesian point estimation and hypothesis testing  
- **Model Selection**: Alternative models compared using DIC and marginal likelihood  

### 🛠️ **Model Versions**  
1. **First Model**: Full feature set with convergence diagnostics  
2. **Second Model**: Removed non-converging coefficients for better performance  
3. **Third Model**: Introduced interaction terms for improved prediction  

## 🔍 Key Findings  
- 🚦 **Environmental factors (weather, road conditions)** significantly impact injury severity  
- 👤 **Cyclist characteristics (age, sex)** influence accident severity, in line with literature  
- 🛣️ **More lanes → higher probability of severe accidents**  
- 📉 **Frequentist vs. Bayesian methods**: Bayesian estimates provided more stable interval estimations  

## 📌 Code Structure  
- `data/` → Processed dataset  
- `models/` → JAGS scripts for Bayesian modeling  
- `notebooks/` → Exploratory analysis, visualization, and diagnostics  
- `results/` → Model summaries, plots, and comparative analysis  

## 📚 References  
- Nowakowska (2017): Bayesian classifiers in road safety analysis  
- Yang et al. (2021): Bayesian risk analysis of bicycle accidents  
- Bayesian Model and Variable Evaluation (2009)  

## 👩‍💻 Author  
**Marina Zanoni**  
This project was developed as part of the *Statistical Modeling and Data Science II (SMDS-II)* course at Sapienza Univerisity.  
