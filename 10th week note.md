# 第十周笔记



## Today Reading 

Mon, Nov 4, 2019

[Habitat: A Platform for Embodied AI Research](http://arxiv.org/abs/1904.01201)

### Abstract 

We present Habitat, a platform for research in embodied artificial intelligence (AI). Habitat enables training embodied agents (virtual robots) in highly efficient photorealistic 3D simulation. Specifically, Habitat consists of: 

+ (i) Habitat-Sim: 

  a flexible, high-performance 3D simulator with configurable agents, sensors, and generic 3D dataset handling. Habitat-Sim is fast – when rendering a scene from Matterport3D, it achieves several thousand frames per second (fps) running single-threaded, and can reach over 10,000 fps multi-process on a single GPU.

+  (ii) Habitat-API: 

  a modular high-level library for end-to- end development ofembodied AI algorithms – defining tasks (e.g. navigation, instruction following, question answering), configuring, training, and benchmarking embodied agents.

These large-scale engineering contributions enable us to answer scientific questions requiring experiments that were till now impracticable or ‘merely’ impractical. Specifically, in the context of point-goal navigation: (1) we revisit the comparison between learning and SLAM approaches from two recent works [19, 16] and find evidence for the opposite conclusion – that learning outperforms SLAM ifscaled to an order of magnitude more experience than previous investigations, and (2) we conduct the first cross-dataset generalization experiments {train, test} × {Matterport3D, Gibson} for multiple sensors {blind, RGB, RGBD, D} and find that only agents with depth (D) sensors generalize across datasets. We hope that our open-source platform and these findings will advance research in embodied AI.

---



## Today Reading 

Tus, Nov 5, 2019

[Few-Shot Image Recognition with Knowledge Transfer]()

### Abstract

Human can well recognize images of novel categories just after browsing few examples of these categories. One possible reason is that they have some external discriminative visual information about these categories from their prior knowledge. Inspired from this, we propose a novel Knowledge Transfer Network architecture (KTN) for few- shot image recognition. The proposed KTN model jointly incorporates visual feature learning, knowledge inferring and classifier learning into one unified framework for their optimal compatibility. First, the visual classifiers for novel categories are learned based on the convolutional neu- ral network with the cosine similarity optimization. To fully explore the prior knowledge, a semantic-visual mapping network is then developed to conduct knowledge inference, which enables to infer the classifiers for novel categories from base categories. Finally, we design an adaptive fusion scheme to infer the desired classifiers by effectively integrat- ing the above knowledge and visual information. Extensive experiments are conducted on two widely-used Mini- ImageNet and ImageNet Few-Shot benchmarks to evaluate the effectiveness of the proposed method. The results compared with the state-of-the-art approaches show the encouraging performance of the proposed method, especially on 1-shot and 2-shot tasks.

---



## Today Reading 

Wed, Nov 6, 2019

[Generation of 3D Brain MRI Using Auto-Encoding Generative Adversarial Networks](https://link.springer.com/chapter/10.1007%2F978-3-030-32248-9_14)

### Abstract

As deep learning is showing unprecedented success in medical image analysis tasks, the lack of sufficient medical data is emerging as a critical problem. While recent attempts to solve the limited data problem using Generative Adversarial Networks (GAN) have been successful in generating realistic images with diversity, most of them are based on image-to-image translation and thus require extensive datasets from different domains. Here, we propose a novel model that can successfully generate 3D brain MRI data from random vectors by learning the data distribution. Our 3D GAN model solves both image blurriness and mode collapse problems by leveraging *𝛼*α-GAN that combines the advantages of Variational Auto-Encoder (VAE) and GAN with an additional code discriminator network. We also use the Wasserstein GAN with Gradient Penalty (WGAN-GP) loss to lower the training instability. To demonstrate the effectiveness of our model, we generate new images of normal brain MRI and show that our model outperforms baseline models in both quantitative and qualitative measurements. We also train the model to synthesize brain disorder MRI data to demonstrate the wide applicability of our model. Our results suggest that the proposed model can successfully generate various types and modalities of 3D whole brain volumes from a small set of training data.

---



## Today Reading 

Wed, Fri 8, 2019

[Federated machine learning: Concept and applications](http://arxiv.org/abs/1902.04885)

### Abstract

Today's AI still faces two major challenges. One is that in most industries, data exists in the form of isolated islands. The other is the strengthening of data privacy and security. We propose a possible solution to these challenges: secure federated learning. Beyond the federated learning framework first proposed by Google in 2016, we introduce a comprehensive secure federated learning framework, which includes horizontal federated learning, vertical federated learning and federated transfer learning. We provide definitions, architectures and applications for the federated learning framework, and provide a comprehensive survey of existing works on this subject. In addition, we propose building data networks among organizations based on federated mechanisms as an effective solution to allow knowledge to be shared without compromising user privacy.



## Today Reading 

Sun Nov 10, 2019

[Weakly-Supervised Semantic Segmentation Network with Deep Seeded Region Growing](http://openaccess.thecvf.com/content_cvpr_2018/papers/Huang_Weakly-Supervised_Semantic_Segmentation_CVPR_2018_paper.pdf)

### abstract

This paper studies the problem of learning image semantic segmentation networks only using image-level labels as supervision, which is important since it can significantly reduce human annotation efforts. Recent state-of-the-art methods on this problem first infer the sparse and discriminative regions for each object class using a deep classification network, then train semantic a segmentation network using the discriminative regions as supervision. Inspired by the traditional image segmentation methods of seeded region growing, we propose to train a semantic segmentation network starting from the discriminative regions and progressively increase the pixel-level supervision using by seeded region growing. The seeded region growing module is integrated in a deep segmentation network and can benefit from deep features. Different from conventional deep networks which have fixed/static labels, the proposed weakly-supervised network generates new labels using the contextual information within an image. The proposed method significantly outperforms the weakly-supervised semantic segmentation methods using static labels, and obtains the state-of-the-art performance, which are 63.2% mIoU score on the PASCAL VOC 2012 test set and 26.0% mIoU score on the COCO dataset.