# GAN_ML_COURSE

- GAN "生成对抗网络"（Generative Adversarial Networks）
> GAN 是由 Ian Goodfellow 和他的同事在 2014 年引入的一种机器学习技术。GAN 由两个部分组成：一个是生成器（generator），另一个是判别器（discriminator）。这两部分都是神经网络。
生成器：它的目标是生成可以通过判别器检测的新数据。生成器接收随机噪声作为输入，然后通过这个噪声生成新的数据实例。
判别器：它的目标是区分来自生成器的假的数据实例和来自训练集的真实数据实例。判别器是一个二元分类器，输出一个在 0 到 1 之间的分数，这个分数表示输入实例来自真实数据（而不是生成器）的概率。

> 想象一下你正在看一场艺术伪造品鉴定比赛。在这场比赛中，有两位参赛者：一个是伪造者（生成器），一个是艺术鉴定师（判别器）。
> - 伪造者（生成器）：这个人的任务是创建看起来像真实艺术品的复制品。他们从零开始，逐渐学习怎样才能制作出看起来真实的艺术品。

> - 艺术鉴定师（判别器）：这个人的任务是鉴别出哪些作品是真正的艺术品，哪些是伪造者制作的。他们是艺术品的专家，知道如何识别真实艺术品的各种特征。

> 比赛开始后，伪造者开始制作他的复制品，而鉴定师则开始鉴定这些作品。初始阶段，伪造者的技术可能还不够成熟，所以鉴定师很容易就识别出了伪造品。
但是，伪造者不会就此放弃。每当鉴定师识别出伪造品，伪造者都会学习鉴定师的反馈，然后改进他们的技术。随着时间的推移，伪造者的技术越来越好，他们的复制品看起来越来越像真实的艺术品。
与此同时，鉴定师也在学习。他们会根据伪造者的新技术调整自己的鉴定标准，从而更好地识别伪造品。
这个比赛会一直持续，直到伪造者的复制品看起来几乎和真实的艺术品无法区分，或者比赛时间到。
这就是生成对抗网络（GANs）的工作原理。生成器（伪造者）试图生成看起来像真实数据（艺术品）的新数据，而判别器（鉴定师）则试图区分真实数据和生成的数据。他们两者之间的“对抗”推动了他们的进步，最终生成器能生成非常逼真的数据。

> 这种方法已经被广泛应用在许多领域，比如生成新的图像、视频或者音频，甚至是改进游戏的AI。但是，GANs 的训练也是有挑战的，比如需要很大的计算能力，训练过程可能会不稳定，等等。
