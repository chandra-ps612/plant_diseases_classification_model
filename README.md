# plant_diseases_classification_model

For this particular project, I used ```TensorFlow==2.6.4```,  ```EfficientNetB0``` pre-trained model for 
```Transfer_learning``` freezing the ```base_model```.
Regarding ```Fine-tune_model```, I used a separate code block to explain the process. 
The model predicts label_name by providing image_path from ```test_set```.


What is ```EfficientNet```?

It was introduced by ```GoogleAI``` in 2019. It is a CNN architecture and scaling method
that uniformly scales all dimensions of CNN such as depth, width, and resolution using 
a compound co-efficient.

It provides a way to scale up CNNs in a more structured manner while also balancing
all dimensions of the network at once, leading to a significant improvement in both
accuracy and efficiency.

```EfficientNet``` has 8 models from ```b0``` to ```b7```. Each model has 4 components
given below-

1. Stem layer
2. Final Layer
3. Sub-blocks (Each block has sub-blocks.)
4. Modules (Each sub-blocks has modules.)

Layer details:


`Input Layer` ->  `Rescaling` -> `Normalization` -> `Zero Padding` -> `Conv2D` -> `Batch Normalization` -> `Activation`


Models' details:

|   Base Model    | Resolution (Input shapes)|
| --------------- | ------------------------ |
| `EfficientNetB0`|          224             |
| `EfficientNetB1`|          240             |
| `EfficientNetB2`|          260             |
| `EfficientNetB3`|          300             |
| `EfficientNetB4`|          380             |
| `EfficientNetB5`|          456             |
| `EfficientNetB6`|          528             |
| `EfficientNetB7`|          600             |



# Reference:
1. Dataset link:  https://lnkd.in/eVyxTqrX
