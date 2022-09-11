- [Content](#content)
    - ["Theory": The BIDS data management principles](#theory-the-bids-data-management-principles)
    - [BIDS conversion by hand](#bids-conversion-by-hand)
    - [Automated BIDS conversion](#automated-bids-conversion)
    - [Using BIDS apps (like fmriprep)](#using-bids-apps-like-fmriprep)
- [Notes](#notes)
- [Not covered](#not-covered)
- [Pre-requisites](#pre-requisites)
    - [Software to install](#software-to-install)

<br>

The
[brain imaging data structure (BIDS)](https://bids-specification.readthedocs.io/en/latest/)
is fast becoming the main standard to organize raw neuroimaging data.

Having your data in BIDS offers many downstream advantages to users: use of
standardized pipelines, facilitate data sharing and reuse…

But getting your data to be BIDS compliant and using can also be source of much
frustration. Especially when it is the first time you are dealing with
neuroimaging data.

This workshop aims to lessen the frustration level you will experience when
curating and using your data.

## Content

This workshop is divided in 4 parts.

### "Theory": The BIDS data management principles

Remembering and following a rule is always easier when you understand why the
rule was put in place: so we will spend a bit of time explaining the reason why
BIDS is structured the way it is.

### BIDS conversion by hand

Using automated BIDS converters is recommended, but using them too early can
turn BIDS into a black box. So doing the conversion of one small dataset by hand
helps better understand "what data/information goes where".

### Automated BIDS conversion

Converting large numbers files quickly becomes impractical and error prone when
by hand. So learning to use a bids converters should be the next logical step.

### Using BIDS apps (like fmriprep)

To wrap up we will spend a bit of time on how to use BIDS applications on the
dataset we have created.

## Notes

This workshop is mostly geared for the MRI part of BIDS but many principles of
BIDS apply to all imaging modalities.

We will finish the workshop with a "ask me anything about BIDS" session where
you can come with more specific questions as they relate to your use case.

## Not covered

The follow issues are be covered in this workshop:

- Where to store data
- Ethical issues around data sharing (notably GDPR)
- Data version control (for example with Datalad)

## Pre-requisites

- Coding experience: none
- Prior experience with neuroimaging data: none
- Data: feel free to bring your own dataset to work on but if you do not have
  data, some data is provided.
- Data type
  - fMRI and resting state
  - Anat
  - DTI
  - Physio / eyetracking

### Software to install

Here is a list of softwares, you will need to install to follow the workshop.

If you have troubles when installing any of these, please contact me before the
workshop and come to the "open-office" that will happen before the workshop
starts.

- Install [Visual studio code](https://code.visualstudio.com/) as your code
  editor

- Python: if you have never used Python before, install it with
  [miniconda](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links).

- Install
  [Dcm2niix](https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage#Download)

- Install the [BIDScoin converter](https://bidscoin.readthedocs.io/en/stable/)

- Install [Docker Desktop](https://www.docker.com/):

  - download the [MRIQC](https://mriqc.readthedocs.io/en/latest/) docker image

  ```bash
  docker pull nipreps/mriqc:latest
  ```

  - download the [fmriprep](https://fmriprep.org/en/stable/) docker image:

  ```bash
  docker pull nipreps/fmriprep:latest
  ```

<footer>
    <hr>
    <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
        <img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png"/>
    </a>
    <br />
    This work is licensed under a
    <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
    Creative Commons Attribution 4.0 International License
    </a>.
</footer>
