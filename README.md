# Machine Learning for Changing Ecosystems  

## Introduction  
Under funding from the **National Science Foundation (NSF)**, our team participated in the **Machine Learning for Changing Ecosystems** workshop alongside:  
- **Dr. Jack Buckner** and **Dr. Zechariah Meunier** (Oregon State University)  
- **Nathan Fitzpatrick**, Ph.D. student (University of Hawaiʻi at Mānoa)  
- **Dr. Lisa McManus** (Hawaiʻi Institute of Marine Biology)  

Our research explores how machine learning can be used to analyze and predict ecological and agricultural changes over time.  

---

## Background  
Understanding the spatial distribution of agricultural lands is vital for many ecological and sustainability analyses. Identifying crop types and land use changes provides insights into nutrient inputs, land degradation, and resource management.  

Our guiding questions were:  
- How much does land use change over time?  
- Can we identify higher thematic resolution in agricultural lands (e.g., crop type) across more years of satellite data?  

For more information, view our workshop presentation:  
[**ML for Changing Ecosystems (Canva)**](https://www.canva.com/design/DAGu237Nguw/BvL6w_q-pXvWI2GQrMbDfw/view?utm_content=DAGu237Nguw&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h06f4339142)

---

## Methodology  
We used a combination of NASA Landsat 8, Hawaiʻi State GIS Land Use Cover, and Hawaiʻi Agriculture Baseline Study vector data to train and evaluate machine learning models that observe agricultural changes across Oʻahu.  

### Project Structure  
The project was divided into three main tasks:  

1. **Unsupervised Learning:**  
   - Used K-Means clustering to identify regions with major agricultural changes.  
   - Calculated key spectral indices including NDVI, NDBI, NDWI, and MNDWI to detect vegetation, urbanization, and water bodies.  

2. **Supervised Learning (Crop Type Classification):**  
   - Applied a Random Forest model to classify agricultural vs. non-agricultural lands using spectral band ratios.  
   - Implemented bootstrapping and Gini impurity to evaluate pixel-level classification and feature importance.  

3. **Model Evaluation:**  
   - Compared training and testing accuracies to assess overfitting.  
   - Evaluated performance using vegetation-sensitive bands (NIR, SWI).  

---

## Findings  
- Near-Infrared (NIR) was the strongest predictor of vegetation presence and health.  
- Short-Wave Infrared (SWI) reflected soil moisture and plant water stress.  
- The Random Forest model achieved:  
  - Training Accuracy: 98.6%  
  - Testing Accuracy: 89.32% (indicating some overfitting).  
- Agricultural land was more accurately predicted than non-agricultural land.  

For additional visualizations and outputs, explore the `/charts` folder in this repository.  

---

## Next Steps  
- Apply supervised learning methods to older datasets (pre-2015).  
- Use a two-stage model approach:  
  1. Random Forest Model 1: Identify agricultural land  
  2. Random Forest Model 2: Classify crop types within identified agricultural zones  
- Expand datasets to include both Rainy and Dry seasons.  
- Extend model coverage to neighboring islands beyond Oʻahu.  
- Evaluate K-Means clustering performance on unseen data.  
- Experiment with deep learning models (CNNs) to improve crop classification accuracy.  

---

## Future Applications  
- Statewide monitoring of agricultural expansion and land conversion.  
- Crop classification for resource management and sustainability planning.  
- Integration with ecological models to assess land use and biodiversity relationships.  

---

## Resources  
- NASA Landsat 8 Data  
- Hawaiʻi State GIS Land Use Cover  
- Hawaiʻi Agriculture Baseline Study  
- [ML for Changing Ecosystems Workshop Presentation](https://www.canva.com/design/DAGu237Nguw/BvL6w_q-pXvWI2GQrMbDfw/view?utm_content=DAGu237Nguw&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h06f4339142)

---

### Contributors  
- **Sakura Takahashi** – University of Hawaiʻi at Mānoa
- **Alana Wesly** – University of Hawaiʻi at Mānoa
- **Lucas Moroz** – University of Hawaiʻi at Mānoa
- **Madeline Berger** – University of Hawaiʻi at Mānoa
- **Nathan Fitzpatrick** – University of Hawaiʻi at Mānoa  
- **Dr. Jack Buckner** – Oregon State University  
- **Dr. Zechariah Meunier** – Oregon State University  
- **Dr. Lisa McManus** – Hawaiʻi Institute for Marine Biology  
