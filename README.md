# deepsaldet
Source code for our CVPR 2015 work on saliency detection by multi-context deep
learning. 

Created by [Rui Zhao](www.ee.cuhk.edu.hk/~rzhao), on May 30, 2015

## Summary
This source code is mainly written in Python and bash shell scripts, and it is for the following paper:
- Rui Zhao, Wanli Ouyang, Hongsheng Li, and Xiaogang Wang. Saliency Detection by
Multi-Context Deep Learning. In CVPR 2015. 

## Usage
- OS and pre-installation: this source code is tested on 64-bit Arch Linux OS,
    and it should be executable in other linux distributions. Pre-installations
    are mainly for [caffe](http://caffe.berkeleyvision.org/), and
    ./caffe-sal/Makefile.config is only for reference. 
- Download caffe models by running: cd models/ && sh get_models.sh && cd ..
- Run demo: sh get_deep_mutlicontext_saliency.sh

## Remark
- Caffe-sal is a customized version of original caffe toolkit. Comparing the
original version, revisions happen
in the following files:

	- ./caffe-sal/src/caffe/layers/mcwindowdatalayers.cpp
	- ./caffe-sal/src/caffe/layers/mcwindowdatalayers.cu
	- ./caffe-sal/src/caffe/proto/caffe.proto
	- ./caffe-sal/src/caffe/layer_factory.cpp

- Test folder can be set in ./get_deep_multicontext_saliency.sh
- This source code requires GPU to accelerate the testing process

##Citing our work
Please kindly cite our work in your publications if it helps your research:

	@inproceedings{zhao2015saliency,
	    title = {Saliency Detection by Multi-Context Deep Learning},
 	    author={Zhao, Rui and Ouyang, Wanli and Li, Hongsheng and Wang, Xiaogang},
	    booktitle = {IEEE Conference on Computer Vision and Pattern
		Recognition (CVPR)},
	    year = {2015}
	}

##License

	Copyright (c) 2015, Rui Zhao
	All rights reserved. 

	Redistribution and use in source and binary forms, with or without 
	modification, are permitted provided that the following conditions are 
	met:
    		* Redistributions of source code must retain the above copyright 
      		  notice, this list of conditions and the following disclaimer.
    		* Redistributions in binary form must reproduce the above copyright 
      		  notice, this list of conditions and the following disclaimer in 
      		  the documentation and/or other materials provided with the distribution
   
	THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" 
	AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE 
	IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE 
	ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE 	
	LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR 
	CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF 
	SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS 
	INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
	CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) 
	ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE 
	POSSIBILITY OF SUCH DAMAGE.
