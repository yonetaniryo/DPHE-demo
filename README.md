# DPHE-demo
This is a simpler version of doubly-permuted homomorphic encryption (DPHE) proposed in our ICCV paper:

Ryo Yonetani, Vishnu Naresh Boddeti, Kris M. Kitani, Yoichi Sato: “Privacy-Preserving Visual Learning Using Doubly Permuted Homomorphic Encryption”, International Conference on Computer Vision, 2017 [(arxiv preprint)](https://arxiv.org/abs/1704.02203)

### Installation tips
phe is a python library for Paillier encryption: https://github.com/n1analytics/python-paillier and can be installed via ```pip install phe```.
If you are using Python 2.7 and get an error about printing function on the above pip verson, just try to use my forked version: https://github.com/yonetaniryo/python-paillier.

### Note
I made this notebook just for showing how the proposed DPHE works on simple cases.
The functions in the notebook cannot be applied directly to sparse vectors with different numbers of non-zeros.
Also, if you want to take real valued vectors (i.e., not integers) as input, please make sure to transform them to valid integers before encryption.
More specifically, please refer to https://github.com/yonetaniryo/python-paillier/blob/master/phe/paillier.py.
