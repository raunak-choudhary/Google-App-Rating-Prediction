# Google App Rating Prediction

This project aims to build a machine learning model that predicts the **rating of Google Play Store apps** using structured metadata such as category, reviews, installs, size, price, and more. The analysis is driven by data cleaning, exploratory data visualization, and linear regression modeling.

## 🧠 Problem Statement

With the growing number of apps in the Play Store, Google is exploring ways to promote high-quality apps by predicting their performance. App ratings are a strong indicator of quality. The goal is to identify patterns and predict which apps are likely to receive high ratings based on their attributes.

## 📊 Dataset

- **Source**: Google Play Store scraped dataset (`googleplaystore.csv`)
- **Features**:
  - App, Category, Rating, Reviews, Size, Installs, Type, Price
  - Content Rating, Genres, Last Updated, Current Version, Android Version

## 🛠️ Key Steps Performed

- **Data Cleaning**:
  - Handled missing values
  - Converted inconsistent data types (e.g., "1,000,000+" to int)
  - Removed outliers in `Price`, `Reviews`, and `Installs`
- **Data Transformation**:
  - Applied log transformation to reduce skew in `Reviews` and `Installs`
  - Used dummy encoding for categorical variables: Category, Genres, and Content Rating
- **Exploratory Analysis**:
  - Created scatter plots and boxplots to explore relationships between features and rating
  - Identified top-rated categories (e.g., Events) and observed trends in paid apps
- **Modeling**:
  - Applied **Linear Regression**
  - R² Score on Train Set: `0.074`
  - R² Score on Test Set: `0.063`

## 📉 Observations

- Paid apps generally receive better ratings than free apps
- Larger apps tend to have slightly better ratings
- More reviews correlate with higher app ratings
- Apps targeted for adults (`18+`) tend to be rated higher than those for everyone
- The `Events` category stands out as having the highest average ratings

## 📁 Final Dataset Shape

- After preprocessing: **8496 rows** × **96 columns**

## 👨‍💻 Author

- **Raunak Choudhary**  
  Email: [raunakchoudhary17@gmail.com](mailto:raunakchoudhary17@gmail.com)  
  LinkedIn: [linkedin.com/in/raunak-choudhary](https://www.linkedin.com/in/raunak-choudhary)