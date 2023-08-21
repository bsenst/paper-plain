## Paper Plain: Making Medical Research Papers Approachable to Healthcare Consumers with Natural Language Processing


By Tal August, Lucy Lu Wang, Jonathan Bragg, Marti A. Hearst, Andrew Head, and Kyle Lo

Abstract: When seeking information not covered in patient-friendly documents, like medical pamphlets, healthcare consumers may turn to the research literature. Reading medical papers, however, can be a challenging experience. To improve access to medical papers, we introduce a novel interactive interface--Paper Plain--with four features powered by natural language processing: definitions of unfamiliar terms, in-situ plain language section summaries, a collection of key questions that guide readers to answering passages, and plain language summaries of the answering passages. We evaluate Paper Plain, finding that participants who use Paper Plainhave an easier time reading and understanding research papers without a loss in paper comprehension compared to those who use a typical PDF reader. Altogether, the study results suggest that guiding readers to relevant passages and providing plain language summaries, or "gists," alongside the original paper content can make reading medical papers easier and give readers more confidence to approach these papers.

## Demos

We provide links to two papers we used in our study with all Paper Plain features applied:

* [Therapeutic peptides for the treatment of systemic lupus erythematosus: a place in therapy](https://s2-reader.tala-s2-simplify.apps.allenai.org/?file=/paper/Lupus_Peptides.pdf&p=1111)
* [Percutaneous endoscopic lumbar discectomy compared with other surgeries for lumbar discherniation](https://s2-reader.tala-s2-simplify.apps.allenai.org/?file=/paper/LDH_surgery.pdf&p=1111)

## Backend
`backend/` includes scripts and notebooks for running models for powering Paper Plain's features

## UI
TBD: `ui/` includes implementation of the interface with Paper Plain's features

## Setup
https://akrabat.com/creating-virtual-environments-with-pyenv/

Install pyenv.

```bash
sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev \
  libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev \
  xz-utils tk-dev libffi-dev liblzma-dev python-openssl git
curl https://pyenv.run | bash
```

```bash
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)
```

Install Python 3.6.

```
pyenv install 3.6
```

Create a virtual environment using Python 3.6.

```bash
pyenv virtualenv 3.6 env36
```

Activate the virtual environment.

```bash
pyenv activate env36
```

Install the requirements.

```bash
pip install -r requirements.txt
```

## Citation

If you use our work, please cite our preprint

```
@misc{august-2022-paper-plain,
    title={Paper Plain: Making Medical Research Papers Approachable to Healthcare Consumers with Natural Language Processing},
    author={Tal August, Lucy Lu Wang, Jonathan Bragg, Marti A. Hearst, Andrew Head, and Kyle Lo},
    year={2022},
    eprint={},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}
```
