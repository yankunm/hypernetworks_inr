# hypernetworks_inr

Experiment 1: CIFAR-10

Problem: "Does INR capture semantic information?"

* Train SIREN-based hypernetwork model on CIFAR-10 dataset 
* Use SIREN-based hypernetwork outputs as inputs to a classifier for CIFAR-10 image classification
* Compare different feature representations on the performance of image classification (I, z, $\theta$)
$$
H: I \rightarrow z \rightarrow \theta
$$
* Describe insights gained from experiment


Experiment 2: Celeb-A

Problem: "Which INR architecture is the best?"

* Train SIREN-based hypernetwork model again on Celeb-A dataset
* Train FFN-based hypernetwork model on Celeb-A dataset
* Train ReLU coordinate network moedl on Celeb-A dataset
* For the three models, compare reconstruction quality, training stability, and computational efficiency
* For each model, evaluate model using PSNR, SSIM, LPIPS (common image generation and reconstruction metrics)
* Describe insights gained from experiment

Experiment 3: Super-Resolution Testing

Problem: "Which INR architecture generalizes the best?"

* Downsample Celeb-A to lower dimension (32 x 32)
* Train SIREN-based hypernetwork model again on downsampled Celeb-A 
* Train FFN-based hypernetwork model again on downsampled Celeb-A 
* Train ReLU coordinate network moedl again on downsampled Celeb-A 
* For each model, evaluate model using PSNR, SSIM, LPIPS (common image generation and reconstruction metrics) by generating higher resolutions (256 x 256)
* Describe insights gained from experiment. Analyze specifically how INR generalize to higher resolutions and how changing architectures influenced performance.