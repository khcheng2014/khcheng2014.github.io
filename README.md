# Academic Pages
**Academic Pages is a GitHub Pages template for personal and professional portfolio-oriented websites.**

![Academic Pages template example](images/homepage.png "Academic Pages template example")

基本信息
======
成宽洪，男，博士，西安理工大学计算机科学与工程学院讲师。美国光学学会会员，中国光学学会终身会员，“图像处理与视觉计算”陕西高校青年创新团队核心成员。2020年获西安电子科技大学电子科学与技术专业博士学位，2018-2019在新加坡南洋理工大学计算机科学与工程学院访问。现主要从事光电成像及图像处理、光电目标检测跟踪、光电图像质量提升等方面的科研工作。主持和参与相关国家自然科学基金项目6项，863计划、国防创新项目、国防预研项目、教育部科学技术研究重点项目、航空科学基金、重点实验室基金等项目多项；获陕西高校科技成果二等奖1项，发表学术论文30余篇，授权发明专利14项，国际专利2项。


## 科研项目

|               项目名称               |    项目来源     | 角色 |
|:--------------------------------:|:-----------:|----|
|      面向反射干扰场景的多源监督图像复原技术研究  |  国家自然科学基金   | 主持 |
|    	目标探测与拒止系统软件设计               |     横向      | 主持 |
|            	光电成像侦察装备升级            |     横向      | 主持 |
|     机器视觉智能测量系统-视觉智能测量软件研发    |     横向      | 主持 |
|        光电成像设备调参操作实验设计           |     横向      | 主持 |
|    面向公共安全的多模态场景感知与异常行为预警系统及应用    | 陕西省创新能力引导专项 | 参与 |
|     双模态图像噪声隐式建模的低照度视频增强理论应用      |  国家自然科学基金   | 参与 |
|   基于XXX的红外弱小目标检测与识别算法研究      | 航空科学基金  | 参与 |

	

[//]: # (![img_1.png]&#40;img_1.png&#41;)
## 教育经历

2020-至今  西安理工大学 讲师

2018-2019 新加坡南洋理工大学 计算机科学与工程学院 联合培养

2013-2020 西安电子科技大学 物理与光电工程学院 电子科学与技术 硕博连读

2008-2012 西安电子科技大学 技术物理学院 光信息科学与技术 本科

研究方向
======
## 1. 病态图像复原

采用图像处理和计算机视觉方法解决反射干扰、大气湍流干扰、图像HDR、图像修复、传感器非均匀性等高度病态的图像退化问题

<img alt="img.png" src="./images/img.png" title="湍流畸变校正" width="720"/>

<img alt="img_5.png" src="./images/img_5.png" title="反射干扰消除" width="720"/>

## 2. 目标检测跟踪

针对红外、可见光视频场景下的弱小目标进行检测和跟踪研究

<img alt="img_2.png" src="./images/img_2.png" width="720"/>

## 3. 光电成像与图像处理系统工程应用

将算法理论工程化，并针对不同场景开发相关软硬件系统，以解决实际应用需求

<img alt="img_4.png" src="./images/img_4.png" width="720"/>

<img alt="img_6.png" src="./images/img_6.png" width="720"/>


# Getting Started

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Click the "Use this template" button in the top right.
1. On the "New repository" page, enter your repository name as "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and add your content.
1. Upload any files (like PDFs, .zip files, etc.) to the `files/` directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## Running locally

When you are initially working on your website, it is very useful to be able to preview the changes locally before pushing them to GitHub. To work locally you will need to:

1. Clone the repository and made updates as detailed above.
1. Make sure you have ruby-dev, bundler, and nodejs installed
    
    On most Linux distribution and [Windows Subsystem Linux](https://learn.microsoft.com/en-us/windows/wsl/about) the command is:
    ```bash
    sudo apt install ruby-dev ruby-bundler nodejs
    ```
    If you see error `Unable to locate package ruby-bundler`, `Unable to locate package nodejs `, run the following:
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```
    then try run `sudo apt install ruby-dev ruby-bundler nodejs` again.

    On MacOS the commands are:
    ```bash
    brew install ruby
    brew install node
    gem install bundler
    ```
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.

    If you see file permission error like `Fetching bundler-2.6.3.gem ERROR:  While executing gem (Gem::FilePermissionError) You don't have write permissions for the /var/lib/gems/3.2.0 directory.` or `Bundler::PermissionError: There was an error while trying to write to /usr/local/bin.`
    Install Gems Locally (Recommended):
    ```bash
    bundle config set --local path 'vendor/bundle'
    ```
    then try run `bundle install` again. If succeeded, you should see a folder called `vendor` and open `.gitignore` then add `vendor` inside it.

1. Run `jekyll serve -l -H localhost` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.
    You may also try `bundle exec jekyll serve -l -H localhost` to ensure jekyll to use specific dependencies on your own local machine.

If you are running on Linux it may be necessary to install some additional dependencies prior to being able to run locally: `sudo apt install build-essential gcc make`

## Using Docker

Working from a different OS, or just want to avoid installing dependencies? You can use the provided `Dockerfile` to build a container that will run the site for you if you have [Docker](https://www.docker.com/) installed.

You can build and execute the container by running the following command in the repository:

```bash
docker compose up
```

You should now be able to access the website from `localhost:4000`.

# Maintenance

Bug reports and feature requests to the template should be [submitted via GitHub](https://github.com/academicpages/academicpages.github.io/issues/new/choose). For questions concerning how to style the template, please feel free to start a [new discussion on GitHub](https://github.com/academicpages/academicpages.github.io/discussions).

This repository was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License (see LICENSE.md). It is currently being maintained by [Robert Zupko](https://github.com/rjzupkoii) and additional maintainers would be welcomed.

## Bugfixes and enhancements

If you have bugfixes and enhancements that you would like to submit as a pull request, you will need to [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) this repository as opposed to using it as a template. This will also allow you to [synchronize your copy](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) of template to your fork as well.

Unfortunately, one logistical issue with a template theme like Academic Pages that makes it a little tricky to get bug fixes and updates to the core theme. If you use this template and customize it, you will probably get merge conflicts if you attempt to synchronize. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch.

---
<div align="center">
    
![pages-build-deployment](https://github.com/academicpages/academicpages.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)
[![GitHub contributors](https://img.shields.io/github/contributors/academicpages/academicpages.github.io.svg)](https://github.com/academicpages/academicpages.github.io/graphs/contributors)
[![GitHub release](https://img.shields.io/github/v/release/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io/releases/latest)
[![GitHub license](https://img.shields.io/github/license/academicpages/academicpages.github.io?color=blue)](https://github.com/academicpages/academicpages.github.io/blob/master/LICENSE)

[![GitHub stars](https://img.shields.io/github/stars/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io)
[![GitHub forks](https://img.shields.io/github/forks/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io/fork)
</div>
