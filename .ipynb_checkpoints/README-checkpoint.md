# img2engage


### Focus 1: Addressing Data Imbalance

Based on our current labeling information, we have the following distribution:

![\|400](https://i.imgur.com/xV7rJh7.png)

1. Individual student
2. Board / materials
3. Whole class
4. Other

It's evident from the distribution that our dataset is imbalanced. To address this:

- **Weighted Loss Function**: We can assign different weights to classes, making the model more sensitive to underrepresented classes.
- **SMOTE (Synthetic Minority Over-sampling Technique)**: This technique can generate synthetic samples for minority classes, improving the balance.
- **Oversampling**: By randomly duplicating samples from the minority classes, we can increase their representation in the dataset.

### Focus 2: Strategic Training & Feature Engineering

While we have access to some tabular data like skeleton coordinates for training, I understand that in a real production environment, we might not always have the luxury of labeling this data. Consequently, I'm prioritizing the following approaches:

- **Image Augmentation**: Enhancing data diversity through methods like grayscale conversion, rescaling, colorization, etc.
- **Incorporating Depth Images**: Adding depth images as prior information can provide additional context, potentially enhancing the model's accuracy.

