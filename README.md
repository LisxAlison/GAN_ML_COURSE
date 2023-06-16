# GAN_ML_COURSE

- GAN "生成对抗网络"（Generative Adversarial Networks）
> GAN 是由 Ian Goodfellow 和他的同事在 2014 年引入的一种机器学习技术。GAN 由两个部分组成：一个是生成器（generator），另一个是判别器（discriminator）。这两部分都是神经网络。

> 生成器（Generator）
生成器的目标是创造出看起来像从真实数据集中抽取出来的新的、假的数据点。在艺术鉴定比赛的比喻中，这就像伪造者尝试复制真实艺术品的行为。为此，生成器以随机噪声作为输入，然后将这个噪声通过一系列的神经网络层进行转换，以生成新的数据。

> 判别器（Discriminator）
判别器的目标是区分出一个数据点是来自于真实数据集还是由生成器制造出来的。回到我们的比喻，判别器就像艺术鉴定师，努力去区分真实艺术品和伪造品。判别器接收一个数据点作为输入（无论是真实的还是生成的），然后输出一个在 0（代表假）到 1（代表真）之间的分数。

> 如何训练GAN
> - 训练 GAN 涉及到反复训练生成器和判别器。判别器在真实数据和生成器生成的数据上进行训练，努力提高其区分真假数据的能力。而生成器则在判别器的指导下进行训练，尝试提高其生成数据的真实性。这是一个动态过程，生成器和判别器都在不断的进化和改进。

> 以下是训练过程的一些步骤：
> - 首先，我们对判别器进行训练。我们用一些真实数据和生成器生成的一些假数据来训练它。判别器的目标是正确地标记真实数据为真，假数据为假。
> - 其次，我们训练生成器。我们用生成器生成一些假数据，然后用判别器来评估这些数据。然后我们将判别器的反馈反向传递给生成器，使其能够改进其生成的数据。生成器的目标是使判别器误判其生成的数据为真。
> - 我们反复进行上述两个步骤，直到判别器无法区分真实数据和假数据，或者达到预定的训练次数。

GANs 的潜力是巨大的，但是他们也是很难训练的，可能会遇到各种问题，比如模式崩溃、训练不稳定等。而且GANs 需要大量的数据和计算资源。
