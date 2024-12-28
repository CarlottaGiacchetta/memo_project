## Deep Learning 2024 - Project Assignment

### 1. Introduction

Deep neural networks have enabled impressive results in many computer vision applications, such as image classification, object detection and tracking, and anomaly detection. However, they suffer from severe performance degradation when being tested on images that are visually different from the ones encountered during training due to the domain shift.

To address this problem, recent research has focused on devising domain adaptation techniques for building deep models that can adapt from an annotated source dataset to a target one. However, such methods require access to either downstream training data, which is difficult to collect, especially in real-world applications where privacy concerns may hinder data acquisition, or multiple samples from the training or testing split. Another line of work is Test-Time Adaptation (TTA), which involves improving the robustness of a pre-trained neural network to a test dataset, possibly by improving the network’s predictions on one test sample at a time.

In this assignment, your goal is to construct, fine-tune, and evaluate a TTA method for the task of image classification. You will be given two methods to draw inspiration from: Marginal Entropy Minimization with One test point (MEMO) [1] and Test-Time Prompt Tuning (TPT) [2]. To evaluate your approach for TTA, you will be provided with a benchmark consisting of ImageNet variants [3, 4] with natural distribution shifts (e.g., images collected from different sources or hard to classify) that you will use as an evaluation set. The performance will be evaluated based on top-1 accuracy on the test datasets.

To complete the assignment, you are free to use any technique or algorithm in the literature, such as attention mechanisms or convolutional neural networks. You are also free to propose a novel method that is different from the approaches of MEMO [1] and TPT [2] as long as it is well-reasoned and sound. In such a case, we encourage you to discuss your idea with us first. This will allow us to provide feedback and ensure that your proposal aligns with the project’s objectives.

### References

1. Zhang, M., Levine, S., Finn, C.: MEMO: Test time robustness via adaptation and augmentation. NeurIPS (2022).
2. Shu, M., Nie, W., Huang, D.-A., et al.: Test-time prompt tuning for zero-shot generalization in vision-language models. NeurIPS (2022).
3. Hendrycks, D., Zhao, K., et al.: Natural adversarial examples. CVPR (2021).
4. Recht, B., Roelofs, R., et al.: Do ImageNet classifiers generalize to ImageNet? ICML (2019).
5. Radford, A., Kim, J.W., et al.: Learning transferable visual models from natural language supervision. ICML (2021).
6. Zhou, K., Yang, J., et al.: Learning to prompt for vision-language models. IJCV (2022).
7. Zhou, K., Yang, J., et al.: Conditional prompt learning for vision-language models. CVPR (2022).

