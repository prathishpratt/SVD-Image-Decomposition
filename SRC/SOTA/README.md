## State of the Art method for Image Compression

This code is directly forked from the [high-fidelity-generative-compression](https://github.com/Justin-Tan/high-fidelity-generative-compression) repo and we have used their Colab notebook  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Justin-Tan/high-fidelity-generative-compression/blob/master/assets/HiFIC_torch_colab_demo.ipynb) to run the SOTA code. 

If you face any errors running this code, please refer to their [repo](https://github.com/Justin-Tan/high-fidelity-generative-compression). 

#### Note: <br>
If you face this error ``` ImportError: cannot import name 'compare_ssim' from 'skimage.measure' (/usr/local/lib/python3.10/dist-packages/skimage/measure/__init__.py)```, install the following version of scikit image (```!pip install scikit-image==0.15.0```) and restart your kernel, if suggested.
<br>
<br>


#### Citation
This is a re-implementation of the [original](https://arxiv.org/pdf/2006.09965.pdf) paper.


@article{mentzer2020high, <br>
  title={High-Fidelity Generative Image Compression}, <br>
  author={Mentzer, Fabian and Toderici, George and Tschannen, Michael and Agustsson, Eirikur}, <br>
  journal={arXiv preprint arXiv:2006.09965}, <br>
  year={2020} <br>
}

