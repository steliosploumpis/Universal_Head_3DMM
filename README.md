# [Combining 3D Morphable Models: A Large Scale Face-And-Head Model](http://openaccess.thecvf.com/content_CVPR_2019/html/Ploumpis_Combining_3D_Morphable_Models_A_Large_Scale_Face-And-Head_Model_CVPR_2019_paper.html)

 [Stylianos Ploumpis](https://www.imperial.ac.uk/people/s.ploumpis)<sup> 1,2</sup>, [Haoyang Wang](https://ibug.doc.ic.ac.uk/people/hwang)<sup> 1,2</sup>, [Nick Pears](https://www-users.cs.york.ac.uk/~nep/)<sup> 3</sup>, [William A. P. Smith](https://www.cs.york.ac.uk/cvpr/member/will/)<sup> 3</sup>, & [Stefanos Zafeiriou](https://wp.doc.ic.ac.uk/szafeiri/)<sup> 1,2</sup>
 <br/>
 <sup>1 </sup>Imperial College London, UK
 <br/>
 <sup>2 </sup>FaceSoft.io
 <br/>
 <sup>3 </sup>University of York, UK
#### [CVPR2019]

<br/>

<p align="center"><img width="100%" src="figures/first_page_fig.png" /></p>

<br/>

## Abstract

Three-dimensional Morphable Models (3DMMs) are powerful statistical tools for representing the 3D surfaces of an object class. In this context, we identify an interesting question that has previously not received research attention: is it possible to combine two or more 3DMMs that (a) are built using different templates that perhaps only partly overlap, (b) have different representation capabilities and (c) are built from different datasets that may not be publicly-available? In answering this question, we make two contributions. First, we propose two methods for solving this problem: i. use a regressor to complete missing parts of one model using the other, ii. use the Gaussian Process framework to blend covariance matrices from multiple models. Second, as an example application of our approach, we build a new head and face model that combines the variability and facial detail of the LSFM with the full head modelling of the LYHM. The resulting combined model achieves state-of-the-art performance and outperforms existing head models by a large margin. Finally, as an application experiment, we reconstruct full head representations from single, unconstrained images by utilizing our proposed large-scale model in conjunction with the Face-Warehouse blendshapes for handling expressions.

## Approach

<p align="center"><img width="100%" src="figures/overview.png" /></p>
#Detailed overview of the proposed approach. A 3D face reconstruction is rendered by a differentiable renderer (shown in purple). Cost #functions are mainly formulated by means of identity features on a pretrained face recognition network (shown in gray) and they are #optimized by flowing the error all the way back to the latent parameters (ps, pe, pt, c, i, shown in green) with gradient descent #optimization. End-to-end differentiable architecture enables us to use computationally cheap and reliable first order derivatives for #optimization thus making it possible to employ deep networks as a generator (i.e,. statistical model) or as a cost function.

<br/>

## More Results

<p align="center"><img width="100%" src="figures/qual_1.pdf" /></p>
<p align="center"><img width="100%" src="figures/special_cases.pdf" /></p>

<br/>

## Citation
If you find this work is useful for your research, please cite our [paper](http://openaccess.thecvf.com/content_CVPR_2019/html/Ploumpis_Combining_3D_Morphable_Models_A_Large_Scale_Face-And-Head_Model_CVPR_2019_paper.html):

```
@inproceedings{ploumpis2019combining,
  title={Combining 3D Morphable Models: A Large scale Face-and-Head Model},
  author={Ploumpis, Stylianos and Wang, Haoyang and Pears, Nick and Smith, William AP and Zafeiriou, Stefanos},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={10934--10943},
  year={2019}
}

```

<br/>

## Publicly Available Head Model
TBA
