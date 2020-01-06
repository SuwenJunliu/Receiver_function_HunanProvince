


# Receiver_function_HunanProvince
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

[![license](https://img.shields.io/github/license/SuwenJunliu/Receiver_function_HunanProvince)](https://github.com/SuwenJunliu/Receiver_function_HunanProvince/blob/master/LICENSE)

[![version](https://img.shields.io/badge/Version-0.0.1-blue)](https://github.com/SuwenJunliu/Receiver_function_HunanProvince)

[![status](https://img.shields.io/badge/Status-constructing-red)](https://github.com/SuwenJunliu/Receiver_function_HunanProvince)

An example of Receiver function inversion of Hunan province


# Table of Contents

- [Receiver_function_HunanProvince](#receiverfunctionhunanprovince)
- [Table of Contents](#table-of-contents)
- [Background](#background)
  - [Purpose](#purpose)
  - [Warning](#warning)
- [Install](#install)
  - [Dependence](#dependence)
  - [Setup](#setup)
- [Manual](#manual)
  - [Package Structure](#package-structure)
    - [data](#data)
  - [Receiver Function Inversion Workflow](#receiver-function-inversion-workflow)
    - [Prepare the event file](#prepare-the-event-file)
      - [QuickStart](#quickstart)
      - [Procedure](#procedure)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [Contributors](#contributors)
- [License](#license)

# Background


## Purpose

This is my first project about Geophysics (Receiver function) which is managed in Github. During the research, I found that receiver function is much popular in the inversion of nature seismic, but there is not a complete process of receiver function inversion. So I decided to create a example of receiver function inversion. I hope that every small process during the inversion could be shown in this project, and it may help for young scientists who work on receiver function.

## Warning
This project is base on the data of Hunan Province, China. According to the restrictions of data, only limited data is provided. Besides, this package contain serveral preseved code of specific research group, and I will provide some substitute code on Github. All the inversion tools are public, you can find these code or packages below.

# Install

## Dependence
This package consists of several software, make sure that you have install these software before:

- [CPS330](http://www.eas.slu.edu/eqc/eqccps.html)
- [NA](http://rses.anu.edu.au/~malcolm/na/)
- [RF_INV](https://github.com/akuhara/RF_INV)

I strongly recommend [Obspy](https://github.com/obspy/obspy) for data preprocessing. The scripts written by python are read much easier than those written by sh/bash. If you install Obspy by anaconda, please make sure that the enviorment setting is correct.

In order to run some Linux script, this serveral programs was demand

- [taup_time](http://www.seis.sc.edu/taup/)
- [hk1.3](http://www.eas.slu.edu/People/LZhu/downloads/hk1.3.tar )
- []

## Setup

```
git clone https://github.com/SuwenJunliu/Receiver_function_HunanProvince.git
```

# Manual

Accoring to the purpose of this project, I will introduce the package structure, including what every folder is, and how to use them. Next, the whole inversion workflow will be present. You could follow the instruction of "QuickStart" and realize them easily. For more details, you could find the "readme" of corresponding folder.

## Package Structure

### data
The folder "./data" consists the data of Hunan Province in SAC format.


## Receiver Function Inversion Workflow

### Prepare the event file

#### QuickStart
```
cd /prepareEventFile/
python 
```
Then, you will find the event index in this folder.

```
python 
```
After that, the data of nature seismic event was created.

#### Procedure
The first thing for RF inversion is preparing SAC file of nature seismic event.
Usually, I use Obspy to download the event index.
The code could be found in 
```
./prepareEventFile/
```
Note that if your study area is in China, and the data was gather recently, the event may not be included by ISC. In this situation, you can download the event index from [CENC](http://news.ceic.ac.cn/index.html?time=1578326915).


Once you prepare the event index, you could cut the event data form original record. Usually, the original record last one hour or much longer. In this project, I use python script to cut the event.
The code could be found in 
```
./prepareEventFile/
```




# Maintainers

[@Junliu](https://github.com/SuwenJunliu/).

# Contributing

Feel free to dive in! [Open an issue](https://github.com/SuwenJunliu/Receiver_function_HunanProvince/issues/new) or submit PRs.



# Contributors




# License

[GPL3.0](LICENSE) © Junliu Suwen
