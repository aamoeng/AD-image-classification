# Results

<img width="341" height="200" alt="image (2)" src="https://github.com/user-attachments/assets/73fa0d82-7106-4225-a9f6-68e8b9e12c37" />

The classification report highlights excellent precision, recall, and F1-scores, indicating the model's ability to accurately identify nearly all positive samples while minimising false positives. High precision and accuracy is essential for medical diagnosis where the consequences of misdiagnosis are significant.

<img width="388" height="250" alt="image (1)" src="https://github.com/user-attachments/assets/57de1ce8-84e9-4a10-9249-8253ee14cf5b" />

The confusion matrix shows the correct and incorrect predictions for each class, thus seeing which disease stages are being confused with others. The highest level of confusion occurred at 1.2% and 2.7% between the Non-Demented and the Very Mild Demented classes.

<img width="300" height="250" alt="Bar graph" src="https://github.com/user-attachments/assets/7254f874-b6ae-4b53-a993-af17d3450385" />

The prediction probability bar graph displays the probability distributions of the predictions for each sample, showing the model’s confidence about each class. The bar graph demonstrates the model’s high confidence in classifying Very Mild Demented and Non Demented stages. Conversely, lower confidence in classifying the other stages may stem from data imbalance, highlighting areas where additional training data could enhance accuracy.


<img width="300" height="200" alt="image (4)" src="https://github.com/user-attachments/assets/b2210162-7665-4bdd-96ec-1cf87fd4cad9" />
<img width="300" height="200" alt="image (3)" src="https://github.com/user-attachments/assets/af523813-d8c7-447b-a776-fc66c74a7b25" />


The figures above show that the model's accuracy consistently increases across both training and validation phases, indicating improved performance in classifying MRI images over ten epochs. Additionally, the model’s loss history and indicates a decrease in errors, confirming that the model's predictions became progressively more accurate
