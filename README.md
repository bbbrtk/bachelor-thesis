## bachelor-thesis
### Video processing using style stransfer with convolutional neural networks

Each part of the project can be found on GitHub:
1. Style Transfer Algorithm and Neural Network

[https://github.com/kamieen03/style-transfer-net](https://github.com/kamieen03/style-transfer-net)

https://github.com/kamieen03/style-transfer-server

2. Mobile Application

https://github.com/bonczol/style-app

3. Server

https://github.com/bbbrtk/aiortc

4. Docker Container

https://github.com/bonczol/style-docker

### Abstract

In this thesis, we are interested in the use of convolution neural networks in video processing.
We analyzed the neural style transfer concept and base our project on the work of Li et al. 
Our goal is to enable fast real-time video processing using artistic style transfer by speeding
up the existing convolutional neural network and ensure easy access by mobile application and
lightweight server. We investigate different approaches and finally use network pruning and
TensorRT library in order to improve the speed of the algorithm. Focusing on availability, we
design the stream server in WebRTC standard and cross-platform mobile application written
in Flutter. The first chapters describe the technologies and implementation of these three
components. Then, we outline the experiments with various parameters on different architectures.
Our main contribution to the development of initial network architecture is network and
model pruning. Network pruning was proved to be very efficient for classification task. Since
transforming picture to picture can be more demanding and is often ill-defined, it was not clear,
whether the same compression algorithms would work just as well. We demonstrate even simple
pruning methods can be used with little to none degradation of output’s quality. The results,
after the final adjustments, shows that our network can achieve similar results to the initial one,
but with greater speed and higher image resolution. We reach the point where the application can
smoothly stream transformed video, so we are pleased with results. The possible delays depend
on the network connection between a mobile device and the server and might be multiplied by
poor GPUs architecture. There is still a field for further quality improvements and speeding,
since we focus only on some architectural aspects of network and did not optimize core server
functions.

### Results

The final result of the project is a mobile application which allows users to pick any photo and
then apply it as a filter in real-time video. Figure presents screenshots taken from style
transfer screen of an application. They show how filters with different textures and colors affects
photos. In order to make our application work we had to also create a back-end environment
which is mainly a server with style transfer neural network.

