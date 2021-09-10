# Visual-Question-Answering
This repository contains an AI system for the task of **[Visual Question Answering]**: given an image and a question related to the image in natural language, the systems answer the question in natural language from the image scene. The system can be configured to use one of 3 different underlying models:

1. **VQA**: This is the *baseline model* given in the paper [VQA: Visual Question Answering]. It encodes the image by a CNN and the question by an LSTM and then combines these for VQA task. It uses *pretrained vgg16* to get the image embedding (may be further normalised), and a 1 or 2-layered LSTM for the question embedding.
2. **SAN**: This is an *attention based model* described in the paper [Stacked Attention Networks for Image Question Answering]. It incorporates attention on the input image.
3. **MUTAN**: This is a variant of the VQA model where instead of a simple of pointwise-product, the image and question embedding are combined using a a special *Multimodal Tucker fusion* technique described in the paper [MUTAN: Multimodal Tucker Fusion for Visual Question Answering].
