# Skin Blemishes

A program that removes unwanted spots with Generative Image Inpainting. This code is adapted from an open source framework for generative image inpainting, with the support of [Contextual Attention](https://arxiv.org/abs/1801.07892) (CVPR 2018) and [Gated Convolution](https://arxiv.org/abs/1806.03589) (ICCV 2019 Oral).

[CVPR 2018 Paper](https://arxiv.org/abs/1801.07892) | [ICCV 2019 Oral Paper](https://arxiv.org/abs/1806.03589) | [Project](http://jiahuiyu.com/deepfill) | [Demo](http://jiahuiyu.com/deepfill) | [YouTube v1](https://youtu.be/xz1ZvcdhgQ0) | [YouTube v2](https://youtu.be/uZkEi9Y2dj4) | [BibTex](#citing)


## Requirements

- Install Python3 (tested on Python 3.5.6)
- Install Tensorflow (version 1.3.0, 1.4.0, 1.5.0, 1.6.0, 1.7.0)
- Install tensorflow toolkit [neuralgym](https://github.com/JiahuiYu/neuralgym) (run `pip install git+https://github.com/JiahuiYu/neuralgym`)
- Download all files from [CelebA-HQ](https://drive.google.com/drive/folders/1uvcDgMer-4hgWlm6_G9xjvEQGP8neW15?usp=sharing)) and put it under the `model_logs/` folder. This is a pretrained model, so once the requirements are met, you can proceed to testing the images directly, using `skin_blemishes()` from `test.py`.

  <img src="https://raw.githubusercontent.com/JiahuiYu/generative_inpainting/v2.0.0/examples/places2/case1_raw.png" width="33%"/> <img src="https://raw.githubusercontent.com/JiahuiYu/generative_inpainting/v2.0.0/examples/places2/case1_input.png" width="33%"/> <img src="https://raw.githubusercontent.com/JiahuiYu/generative_inpainting/v2.0.0/examples/places2/case1_output.png" width="33%"/>
<img src="https://raw.githubusercontent.com/JiahuiYu/generative_inpainting/v2.0.0/examples/places2/case4_raw.png" width="33%"/> <img src="https://raw.githubusercontent.com/JiahuiYu/generative_inpainting/v2.0.0/examples/places2/case4_input.png" width="33%"/> <img src="https://raw.githubusercontent.com/JiahuiYu/generative_inpainting/v2.0.0/examples/places2/case4_output.png" width="33%"/>

Free-form image inpainting results by our system built on gated convolution. Each triad shows original image, free-form input and our result from left to right.


## TensorBoard

Visualization on [TensorBoard](https://www.tensorflow.org/programmers_guide/summaries_and_tensorboard) for training and validation is supported. Run `tensorboard --logdir model_logs --port 6006` to view training progress.

## License

CC 4.0 Attribution-NonCommercial International

The software is for educational and academic research purposes only.

## Citing
```
@article{yu2018generative,
  title={Generative Image Inpainting with Contextual Attention},
  author={Yu, Jiahui and Lin, Zhe and Yang, Jimei and Shen, Xiaohui and Lu, Xin and Huang, Thomas S},
  journal={arXiv preprint arXiv:1801.07892},
  year={2018}
}

@article{yu2018free,
  title={Free-Form Image Inpainting with Gated Convolution},
  author={Yu, Jiahui and Lin, Zhe and Yang, Jimei and Shen, Xiaohui and Lu, Xin and Huang, Thomas S},
  journal={arXiv preprint arXiv:1806.03589},
  year={2018}
}
```
