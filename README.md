# NiftyNet

<img src="https://cmiclab.cs.ucl.ac.uk/CMIC/NiftyNet/raw/master/niftynet-logo.png" width="263" height="155">

[![build status](https://cmiclab.cs.ucl.ac.uk/CMIC/NiftyNet/badges/dev/build.svg)](https://cmiclab.cs.ucl.ac.uk/CMIC/NiftyNet/commits/dev)
[![coverage report](https://cmiclab.cs.ucl.ac.uk/CMIC/NiftyNet/badges/dev/coverage.svg)](https://cmiclab.cs.ucl.ac.uk/CMIC/NiftyNet/commits/dev)

NiftyNet is a [TensorFlow][tf]-based open-source convolutional neural networks (CNN) platform for research in medical image analysis and image-guided therapy.
NiftyNet's modular structure is designed for sharing networks and pre-trained models.
Using this modular structure you can:

* Get started with established pre-trained networks using built-in tools
* Adapt existing networks to your imaging data
* Quickly build new solutions to your own image analysis problems

NiftyNet is a consortium of research groups (WEISS -- [Wellcome EPSRC Centre for Interventional and Surgical Sciences][weiss], CMIC -- [Centre for Medical Image Computing][cmic], HIG -- High-dimensional Imaging Group), where WEISS acts as the consortium lead.


### Features

NiftyNet currently supports medical image segmentation and generative adversarial networks.
**NiftyNet is not intended for clinical use**.
Other features of NiftyNet include:

* Easy-to-customise interfaces of network components
* Sharing networks and pretrained models
* Support for 2-D, 2.5-D, 3-D, 4-D inputs*
* Efficient discriminative training with multiple-GPU support
* Implementation of recent networks (HighRes3DNet, 3D U-net, V-net, DeepMedic)
* Comprehensive evaluation metrics for medical image segmentation

 <sup>*2.5-D: volumetric images processed as a stack of 2D slices;
4-D: co-registered multi-modal 3D volumes</sup>


### Installation

1. Please install the appropriate [TensorFlow][tf] package*:
   * [`pip install tensorflow-gpu==1.1`][tf-pypi-gpu] for TensorFlow with GPU support
   * [`pip install tensorflow==1.1`][tf-pypi] for CPU-only TensorFlow
1. [`pip install niftynet`](https://pypi.org/project/NiftyNet/)

 <sup>*All other NiftyNet dependencies are installed automatically as part of the pip installation process.</sup>

[tf-pypi-gpu]: https://pypi.org/project/tensorflow-gpu/
[tf-pypi]: https://pypi.org/project/tensorflow/


### Getting started

Please follow the links for [demos](./demos) and [network (re-)implementations](./niftynet/network).

The API documentation is available on [Read the Docs][rtd-niftynet].

[rtd-niftynet]: http://niftynet.rtfd.io/


### Contributing

Feature requests and bug reports are collected on [Issues](https://cmiclab.cs.ucl.ac.uk/CMIC/NiftyNet/issues).

Contributors are encouraged to take a look at [CONTRIBUTING.md](./CONTRIBUTING.md).

### Citing NiftyNet

If you use NiftyNet in your work, please cite [Li et. al. 2017][ipmi2017]:

<blockquote>
<div>Li W., Wang G., Fidon L., Ourselin S., Cardoso M.J., Vercauteren T. (2017)
<a class="reference external" href="http://doi.org/10.1007/978-3-319-59050-9_28">On the Compactness, Efficiency, and Representation of 3D Convolutional Networks: Brain Parcellation as a Pretext Task.</a>
In: Niethammer M. et al. (eds) Information Processing in Medical Imaging. IPMI 2017.
Lecture Notes in Computer Science, vol 10265. Springer, Cham. DOI: <a class="reference external" href="http://doi.org/10.1007/978-3-319-59050-9_28">10.1007/978-3-319-59050-9_28</a></div></blockquote>

BibTeX entry:

```ini
@InProceedings{niftynet17,
  author = {Li, Wenqi and Wang, Guotai and Fidon, Lucas and Ourselin, Sebastien and Cardoso, M. Jorge and Vercauteren, Tom},
  title = {On the Compactness, Efficiency, and Representation of 3D Convolutional Networks: Brain Parcellation as a Pretext Task},
  booktitle = {International Conference on Information Processing in Medical Imaging (IPMI)},
  year = {2017}
}
```

[ipmi2017]: http://doi.org/10.1007/978-3-319-59050-9_28


### Licensing and Copyright

Copyright 2017 University College London and the NiftyNet Contributors.
NiftyNet is released under the Apache License, Version 2.0. Please see the LICENSE file for details.

### Acknowledgements

This project is grateful for the support from the [Wellcome Trust][wt], the [Engineering and Physical Sciences Research Council (EPSRC)][epsrc], the [National Institute for Health Research (NIHR)][nihr], the [Department of Health (DoH)][doh], [University College London (UCL)][ucl], the [Science and Engineering South Consortium (SES)][ses], the [STFC Rutherford-Appleton Laboratory][ral], and [NVIDIA][nvidia].

[cmic]: http://cmic.cs.ucl.ac.uk
[ucl]: http://www.ucl.ac.uk
[tf]: https://www.tensorflow.org/
[weiss]: http://www.ucl.ac.uk/weiss
[wt]: https://wellcome.ac.uk/
[epsrc]: https://www.epsrc.ac.uk/
[nihr]: https://www.nihr.ac.uk/
[doh]: https://www.gov.uk/government/organisations/department-of-health
[ses]: https://www.ses.ac.uk/
[ral]: http://www.stfc.ac.uk/about-us/where-we-work/rutherford-appleton-laboratory/
[nvidia]: http://www.nvidia.com

