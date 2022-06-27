# High-resolution Face Swapping via Latent Semantics Disentanglement
>We present a novel high-resolution face swapping method using the inherent prior knowledge of a pre-trained GAN model. Although previous research can leverage generative priors to produce high-resolution results, their quality can suffer from the entangled semantics of  the latent space. We explicitly disentangle the latent semantics by utilizing the progressive nature of the generator, deriving structure attributes from the shallow layers and appearance attributes from the deeper ones. Identity and pose information within the structure attributes are further separated by introducing a landmark-driven structure transfer latent direction. The disentangled latent code produces rich generative features that incorporate feature blending to produce a plausible swapping result. We further extend our method to video face swapping by enforcing two spatio-temporal constraints on the latent space and the image space. Extensive experiments demonstrate that the proposed method outperforms state-of-the-art image/video face swapping methods in terms of hallucination quality and consistency.
## Description

We present the inference code on CelebA-HQ dataset, Anaconda is required.


**Build the environment**
`conda env create -f stylegan.yaml`

**Download the dataset and checkpoint**
1. We have inverted the CelebA-HQ dataset using pSp encoder. The whole dataset can be download from this [link](https://drive.google.com/file/d/1TRLvURZpx5xtEnxBXeaaZs1RbReWftBv/view?usp=sharing). *After dowoload the dataset, unzip it and move it to the upper folder*.
2. The checkpoint can be downloaded from this [link](https://drive.google.com/file/d/1LH4RlxaPnrHAiWEDm3LDp5Sz9H02bzXU/view?usp=sharing). *Download it and put it at the current folder*.

**Run the inference code**
`bash run.sh`



## Citation
>@inproceedings{xu2022high,
  title={High-resolution face swapping via latent semantics disentanglement},<br />author={Xu, Yangyang and Deng, Bailin and Wang, Junle and Jing, Yanqing and Pan, Jia and He, Shengfeng},<br />booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},<br />pages={7642--7651},<br />year={2022}
}
