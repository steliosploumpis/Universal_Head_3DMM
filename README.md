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
Detailed overview of our regression modeling pipeline. 1) The left part illustrates the matrix formulation from the original LYHM head model; 2) the central part demonstrates how we utilize the MeIn3D database to produce highly-detailed head shapes; 3) the final part on the right depicts the registration framework along with the per-vertex template weights and the statistical modeling.

<p align="center"><img width="50%" src="figures/triangles.png" /></p>
A graphical representation of the non-rigid registration of all mean meshes along with our head template St and the calculation of the local covariance matrix Ki,j based on the locations of the ith and jth points.


<br/>

## Head Reconstruction Results from single images

<p align="center"><img width="70%" src="figures/qual_1.png" /></p>

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

## Public release models
The head models have been freely available for research and education purposes. To obtain access to the models, you need to complete and sign the user agreement form. This agreement should be completed by a full-time academic staff member (not a student) or a craniofacial clinician. The form should be signed, and emailed to Stylianos Ploumpis (s.ploumpis@imperial.ac.uk). We will verify your request and contact you on how to download the model package. Note that the agreement requires that:

1. The models are used for non-commercial research and education purposes only.
2. You agree not copy, sell, trade, or exploit the model for any commercial purposes.
3. In any published research using the models, you cite the following paper:

Combining 3D Morphable Models: A Large scale Face-and-Head Model, Stylianos Ploumpis, Haoyang Wang, Nick Pears, William AP Smith, Stefanos Zafeiriou, Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition, 2019


<a href="http://www.youtube.com/watch?feature=player_embedded&v=fNlMGWm7bbk&t=4700s
" target="_blank"><img src="figures/qual_1.png"
alt="Oral presentation" width="240" height="180" border="10" /></a>
