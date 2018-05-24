# Relieve-the-Asymmetric-Graidents-in-GAN
## Abstract
The Generative Adversarial Network(GAN) which can generate very realistic images is a popular model recently. But it also has a lot of problems, such as gradient asymmetry, mode collapse, etc. In this study, we treat the train of GAN as a saddle surface optimization problem, and regard the negative effects of GAN's loss function as an oblique saddle surface in restricted parameter space.

Along the ideas of optimization, we propose a new method to relieve the GAN's training problem. This method adopts the 2-norms of discriminator's gradients as gradient penalty to restrain the discriminator's gradients. Experiments prove that this method improves the quality of generated images and relieves the phenomenon of mode collapse. On the popular generative model databases such as CELEBA, CIFAR10, STL-10 etc, this method achieves state of the art Inception scores.

The contributions of this work are as follows. First, we give a new view to analyze the training of GAN, and get the reason why discriminator' gradients are larger than generator's gradients except vanishing gradients. Furthermore, we summarize the advantages of latest models from the view of this paper, and find that in the view of point they have the similar purpose although by different approaches. Additionally, a group of regularization methods is proposed to improve GAN' training along our idea, and get the state of the art generated images.

## Image
![A simple example, the left one is the surface of f(x,y)=log(1-sigmoid(xy)) and the right one is the f(x,y)=log(1-sigmoid(xy)) + log(sigmoid(x)). It is clear that the left image is a symmetrical saddle surface along diagonal lines, but the right image is not.](https://github.com/Hongyun1993/Relieve-the-Asymmetric-Graidents-in-GAN/blob/master/image/surface-eps-converted-to.pdf)

