
# Diet Recommendation System

## Goal of the Project
Your daily food choices significantly impact your health, affecting how you feel today, tomorrow, and in the future. Good nutrition, combined with physical activity, helps you reach and maintain a healthy weight, reduces your risk of chronic diseases like heart disease and cancer, and promotes your overall health. A balanced diet provides your body with the necessary nutrients to function correctly. This project aims to assist users in making informed dietary choices through a personalized diet recommendation system, enhancing health outcomes and personal well-being.

## Introduction
Diet and daily food intake are pivotal for a healthy life, particularly for people suffering from various health conditions. The eHealth initiatives have shown that inappropriate and inadequate diet is a major reason for numerous health issues. The World Health Organization estimates that poor nutrition links to significant percentages of non-communicable disease deaths worldwide. This project develops a diet recommendation system that offers dietary assistance tailored to individuals' specific health needs and lifestyle choices, using a blend of content-based and collaborative filtering methodologies.

## Significance of the Project
This project addresses the critical challenge of dietary management in a personalized manner, leveraging data structures and algorithms to make informed suggestions that can help individuals improve their eating habits and overall health. It introduces a novel approach by integrating user health data with machine learning models to dynamically suggest diet options that are not only healthy but also customized to individual nutritional needs.

## Installation and Instructions to Use
### Installation
**For Windows and macOS:**
1. Ensure Python 3.x is installed on your system. You can download it from [python.org](https://www.python.org/downloads/).
2. Install required Python libraries using pip:
   ```bash
   pip install pandas numpy sklearn
   ```
3. Clone the repository:
   ```bash
   git clone https://github.com/jrobin11/cmpsc445.git
   cd cmpsc445
   ```

### Instructions to Use
1. Run the application:
   ```bash
   python diet_recommendation_system.py
   ```
2. Enter your details in the GUI fields provided (age, vegetarian/non-vegetarian, weight, and height).
3. Select the type of recommendation you need (Weight Loss, Weight Gain, Healthy Diet) and view the suggested food items.

## Structure of the Code
The project is structured as follows:
- **Data Loading and Preprocessing**: CSV files are read and data is formatted into usable structures.
- **User Interface**: Tkinter is used to create a simple and interactive GUI for user input.
- **Machine Learning Models**:
  - **K-Means Clustering**: Used to classify food items based on their nutritional content.
  - **Random Forest Classifier**: Predicts the most suitable food items based on user BMI and age.
- **Output**: Food suggestions are displayed based on the model predictions.

## Functionalities and Test Results
### Functionalities
- **User Profile Input**: Users can input their personal data including dietary preference.
- **Diet Recommendation**: Based on the input, the system suggests a list of food items for different meals.
- **GUI Interaction**: The system is fully interactive through a graphical user interface.

### Test Results
- **Unit Testing**: Individual functions are tested to ensure they return expected outputs.
- **Integration Testing**: The whole system is tested to ensure that the components work together correctly.
- **User Acceptance Testing**: Conducted with potential users to ensure the system meets their needs.

### Reading the dataset
![dataset](https://github.com/jrobin11/cmpsc445/assets/73866458/358ee81e-209d-4817-984c-368532a61dfa)

### Applying KMeans for clustering on Lunch_data, Breakfast_data, Dinner data
![kmeans](https://github.com/jrobin11/cmpsc445/assets/73866458/b5d843f9-8062-484f-9903-fd9dd807f79f)

### Applying Random Forest Classifier
![random](https://github.com/jrobin11/cmpsc445/assets/73866458/5d42814f-59f2-4c32-bf2e-3543c2df7154)

### Creating Interface
![interface](https://github.com/jrobin11/cmpsc445/assets/73866458/19e4ef63-55e0-4043-aa0c-424fb6d189a8)

### Taking inputs
![taking inputs](https://github.com/jrobin11/cmpsc445/assets/73866458/1e16476c-6fcc-4576-b2d0-3afe4fd0e1a2)


### Predicting food items for Weight Loss Diet Plan
![plan](https://github.com/jrobin11/cmpsc445/assets/73866458/31cf0a40-01be-4ce0-8a0b-494e4bf826c6)

### Predicting Food Items for Weight Gain Diet Plan
![weight gain](https://github.com/jrobin11/cmpsc445/assets/73866458/775af0a6-85d9-41c0-a5dc-05e2f16c0779)

### Predicting Food Items for Healthy food items
![healthy](https://github.com/jrobin11/cmpsc445/assets/73866458/9c22ba38-7ba6-455d-b5f5-342ab4ce7021)


# Results and Discussion

## Case Study Overview
To validate the effectiveness and precision of our Diet Recommendation System, we conducted a detailed case study using a specific user profile. The subject chosen for this study was a 22-year-old individual with a non-vegetarian dietary preference. Key physical attributes include a weight of 120 kg and a height of 177 cm. This profile was selected to test the system’s ability to handle cases where significant dietary management is necessary.

## Computational Analysis
### BMI Calculation
The initial step in the recommendation process involves calculating the user's Body Mass Index (BMI). For our subject, the BMI was calculated to be 38.3, categorizing them as "Severely Overweight" according to established health standards. This metric is crucial as it guides the subsequent dietary suggestions.

### Dietary Recommendations
Based on the calculated BMI, the system utilized a refined algorithm to generate a list of appropriate food items. The algorithm considers both the caloric content and the nutritional value of foods, aiming to create a balanced diet tailored to weight management needs. The recommendations were as follows:

- **Fruits and Vegetables:** Avocados, Bananas, Cauliflower, Grapes, Orange, Pears, Peas, Pumpkin, Tomato
- **Grains and Cereals:** Bagels made with wheat, Poha, Chappati
- **Dairy and Proteins:** American cheese, Milk, Protein Powder
- **Treats and Snacks:** Sugar Doughnuts, Strawberry Icecream, Marshmallows, Chocolate milk, Rice Pudding

## Technical Discussion
The selection algorithm prioritizes a mix of macronutrients (carbohydrates, proteins, and fats) and micronutrients (vitamins and minerals), crucial for addressing obesity-related health risks. Notable is the inclusion of high-fiber fruits and vegetables, protein sources for muscle maintenance and satiety, and whole grains for sustained energy release.

However, the algorithm also recommended high-calorie snacks, which while satisfying taste preferences, could potentially undermine the weight management goal. This outcome highlights a need for further refinement in the system’s recommendation logic to better balance health benefits against user satisfaction.

## Algorithmic Limitations and Future Directions
Currently, the system’s recommendations are primarily driven by calorie content and basic nutritional values, without deep consideration of other dietary factors like sodium levels, sugar content, or potential allergens. Future development will aim to integrate a more holistic nutritional analysis, potentially employing advanced machine learning models such as neural networks or ensemble methods that can learn from a broader set of dietary data and user feedback.

Additionally, incorporating user feedback loops into the system can help in dynamically adjusting the recommendations based on real-world efficacy and user satisfaction, enhancing personalization and accuracy.

## Conclusion
This case study underscores the potential of the Diet Recommendation System to deliver personalized dietary advice tailored to the specific health requirements of users. The insights gained from this analysis are instrumental in driving future improvements, ensuring the system not only meets but exceeds the dietary management needs of individuals, particularly those at risk due to obesity.
