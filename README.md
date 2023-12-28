# GTZAN---Music-Genres-Classification

 ![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/04964d0a-2e7f-4a96-92c3-61c55c7377e2)

## Tools used:
![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/62821b16-e30c-4606-a1aa-87fe6ad3aaf5)

## Classification
A notebook that presents music genre classifications:
- based on 30-second wav files
- converting a music file to a spectrogram that can be classified in the same way as an image
- using CNNs to select the appropriate music genre

![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/598c4c4a-9533-4a59-b14b-5fb3b882ec31)

## Data Augmentation 
Data Augmentation was performed which increased preformance of the model significantly.
On Audio:
- Time shifting
- Adding Gaussian Noise
- Cropping and Padding
- 
On spectrogram:
- Time / frequency masking
- CutMix
- MixUp
  
![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/1932a69d-7088-4048-bd9c-2246161f37bc)

![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/70b01b07-6f3f-4cb1-8451-09c5c653aa45)

## Data Processing Pipeline

![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/498d7a61-1c07-468d-adea-05386fadbd9b)

## Transfer learning
Final model was based on EfficientNet:
![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/84110ca6-742b-4968-9749-95458bb4a333)
![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/44adc891-1eef-4942-8870-3164e0c4a9f0)

The model had the most trouble distinguishing disco from pop, which makes sense because these music genres are the most general, easily confused with each other.


## Saliency Maps
The notebook additionally shows which part of the spectrogram the neural network focuses on during classification using Saliency Maps.

Example:
![image](https://github.com/kmotyka00/GTZAN---Music-Genres-Classification/assets/61949638/647f63ac-c106-498c-96b2-7b2a05ae3df1)

For jazz music, neural network was focusing on sequentially repeating lack of amplitude in lower frequencies.
