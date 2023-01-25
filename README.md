# GPU Programming (N8 CIR Fork)

This is an adapted version of the [Carpentries Incubator GPU Programming workshop](https://github.com/carpentries-incubator/lesson-gpu-programming). 
The course has been adapted for an [N8 CIR Training workshop](https://n8cir.org.uk/events/) with minor adjustments.

## Remit

This adapted fork is for workshops set to be delivered in February and April 2023. 
There will be limited maintainence of this fork after that time period and we recommend using the original Carpentries Incubator lesson for more up-to-date materials.

## Running this code on Bede

This repository and associated code will run on Bede by taking the following steps:

1. Install [miniconda](https://docs.conda.io/en/latest/miniconda.html) to access the `conda` package manager by following the [Bede documentation](https://bede-documentation.readthedocs.io/en/latest/software/applications/conda.html#installing-miniconda)
2. Install mamba in your base environment
  ```bash
  $ conda activate base
  (base) $ conda install -c conda-forge mamba
  ```
3. Create the `gpu-py` environment using the provided environment.yml
  ```bash
  (base) $ cd lesson-gpu-programming
  (base) $ mamba env create -f environment.yml
  (base) $ conda activate gpu-py
  ```
4. Load the cuda module
  ```bash
  (gpu-py) $ module add cuda
  ```
5. You can then run the code snippets in this tutorial via JupyterLab (will require additional configuration) or the IPython terminal (this is **not** recommended for production code)


## Contributing

We welcome all contributions to improve the lesson! Maintainers will do their best to help you if you have any
questions, concerns, or experience any difficulties along the way.

We'd like to ask you to familiarize yourself with our [Contribution Guide](CONTRIBUTING.md) and have a look at
the [more detailed guidelines][lesson-example] on proper formatting, ways to render the lesson locally, and even
how to write new episodes.

Please see the current list of [issues][FIXME] for ideas for contributing to this
repository. For making your contribution, we use the GitHub flow, which is
nicely explained in the chapter [Contributing to a Project](http://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project) in Pro Git
by Scott Chacon.
Look for the tag ![good_first_issue](https://img.shields.io/badge/-good%20first%20issue-gold.svg). This indicates that the maintainers will welcome a pull request fixing this issue.  


## Maintainer(s)

Current maintainers of this lesson are 

* Alessio Sclocco [@isazi](https://github.com/isazi)


## Authors

A list of contributors to the lesson can be found in [AUTHORS](AUTHORS)

## Citation

To cite this lesson, please consult with [CITATION](CITATION)

[lesson-example]: https://carpentries.github.io/lesson-example
