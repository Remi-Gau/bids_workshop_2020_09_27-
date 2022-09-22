# BIDS workshop

=======
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

# Abstract

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

This workshop will be divided in 4 parts.

1. Theory: The BIDS data management principles

Remembering and following a rule is always easier when you understand why the
rule was put in place: so we will spend a bit of time explaining the reason why
BIDS is structured the way it is.

2. BIDS conversion by hand

Using automated BIDS converters is recommended, but using them too early can
turn BIDS into a black box. So doing the conversion of one small dataset by hand
helps better understand "what data/information goes where".

1. automated BIDS conversion

Converting large numbers files quickly becomes impractical and error prone when
by hand. So learning to use a bids converters should be the next logical step.

4. using BIDS apps (like fmriprep)

To wrap up we will spend a bit of time on how to use BIDS applications on the
dataset we have created.

We will finish the workshop with a "ask me anything about BIDS" session where
you can come with more specific questions as they relate to your use case.

## Prerequisite

- Coding experience: none
- Prior experience with neuroimaging data: none
- Data: feel free to bring your own dataset to work on but if you do not have
  data, some will be provided.
- Data type
  - fMRI and resting state
  - Anat
  - DTI
  - Physio / eyetracking

### Software to install

- Install [Visual studio code](https://code.visualstudio.com/) as your code
  editor

- Python

If you have never used Python before, install it with
[miniconda](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links).

When installing if you are prompted, select `Register Miniconda as my default python`.

In Windows if you want to start conda and easily run python from your Powershell: follow this procedure

https://stackoverflow.com/a/67996662

- Install
  [Dcm2niix](https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage#Download)

- install the [BIDScoin converter](https://bidscoin.readthedocs.io/en/stable/)

- [Docker](https://www.docker.com/)

For Windows:

- Install **Docker Desktop**
- Launch Docker desktop and run the first part of the tutorial ("clone a repository") to make sure everything was correctly installed.

  - download the [MRIQC](https://mriqc.readthedocs.io/en/latest/) docker image

Open a terminal (or a powershell for Windows) and type the command

```bash
docker pull nipreps/mriqc:latest
```

  - download the [fmriprep](https://fmriprep.org/en/stable/) docker image:

```bash
docker pull nipreps/fmriprep:latest
```

## Note

This workshop will be mostly geared for the MRI part of BIDS but many principles
of BIDS apply to all imaging modalities.

## Not covered

The follow issues will not be covered in this workshop but could be discussed at
the end if some are interested.

- Where to store data
- Ethical issues around data sharing (notably GDPR)
- Data version control (for example with Datalad)

<footer>
    <hr>
    <br />
    <button style="margin-bottom: 10px"><a href="#TOC">back to the top</a></button>
    <br />
    <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
        <img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png"/>
    </a>
    <br />
    This work is licensed under a
    <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
    Creative Commons Attribution 4.0 International License
    </a>.
</footer>