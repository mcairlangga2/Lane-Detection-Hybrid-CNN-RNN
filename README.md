# Lane-Detection-Hybrid-CNN-RNN
This project is part of my undergraduate thesis. I build my own dataset for Indonesian road in three weather conditions: sunny, rainy, night and also three road conditions: straight, turn right, and turn left. The model that I used is based on Zou et. al. [1] which is the combination of UNet/SegNet and LSTM. The lane detection was done in the manner of semantic segmentation. I evaluate the performance of the model using F1-score and compare it with the algorithm that used by my senior in previous undergraduate thesis. 

## Architecture of the model:
![Lane Detection Architecture](https://user-images.githubusercontent.com/95354928/194760765-197392f5-0300-4322-8e4b-7c51a99c6474.png)

## Code and Resources Used:
Thanks to original source code. For the complete dataset for training and original code, you may find it in [this link](https://github.com/qinnzou/Robust-Lane-Detection)
Below is resources for my own implementation
- Python == 3.7.11
- PyTorch == 1.10.2
- Packages: numpy, PIL, sklearn, tqdm, OpenCV

Below is the notebook i used to train the model and process the input video
- Model training : 
  - [UNet-ConvLSTM](https://github.com/mcairlangga2/Lane-Detection-Hybrid-CNN-RNN/blob/main/UNet-ConvLSTM%20train.ipynb)
  - [SegNet-ConvLSTM](https://github.com/mcairlangga2/Lane-Detection-Hybrid-CNN-RNN/blob/main/SegNet-ConvLstm%20train.ipynb)
- Video Processing :
  - OpenCV Video Processing(https://github.com/mcairlangga2/Lane-Detection-Hybrid-CNN-RNN/blob/main/VideoProcessingLaneDetection.ipynb)

## References
[1] Zou, Q., Jiang, H., Dai, Q., Yue, Y., Chen, L., & Wang, Q. (2019). Robust lane detection from continuous driving scenes using deep neural networks. IEEE transactions on vehicular technology, 69(1), 41-54.

[2] Widianto, S. C. (2020). Deteksi Lajur Mobil Otonom Pada Kondisi Gambar Terdistorsi dan Kurang Pencahayaan Menggunakan Pengolahan Citra [Undergraduate Thesis]. Institut Teknologi Sepuluh Nopember.
