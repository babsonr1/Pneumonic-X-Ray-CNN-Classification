# Pneumonic-X-Ray-CNN-Classification
Using both AlexNet and VGG16 to predict pneumonia in x-ray scans.

# Comparison
### AlexNet
- Significantly less computationally expensive
- Better recall via high positive predictions
    - Causes much worse precision
- Slightly low false negative rate - by virtue of predicting negative much less often

### VGG16
- Less loss implying a much better prediction rate
- 10% higher accuracy rate
- 11% higher precision
- Marginally less recall at the expense of much higher precision
- Many more true negatives

AlexNet was a much faster model that did not learn as much and preferred to simply predict positive more often, which resulted in a relatively high accuracy, as there are many positives in the dataset, but would generally not be the recommended approach.

VGG16 took much longer but learned many more trends in the images. VGG16 could actually predict negative instances at a much higher rate, which raised the accuracy, but slightly lowered the recall. This was favorable as the precision increased dramatically, as the predicitions were made based on more analysis, rather than always choosing positive.
