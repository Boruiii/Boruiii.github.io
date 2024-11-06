---
permalink: /
title: "Welcome to berry academic websites!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

关于我的一切（中文版）
======
张博睿，男，1999年生于天津，2019年12月加入中国共产党。2021年，于西南大学计信院信息管理系获得管理学学士学位。2022年，以专业课第一名成绩，考入中国科学院大学。自入学以来，累计获得成思危优秀学生奖、李炳穆二等奖、国科大三好学生及成都分院气排球比赛第八名等荣誉。
学术研究方面，以通讯作者身份累计发表3篇CSSCI论文，以及《数据分析与知识发现》返修1篇，外审3篇与多篇在研。
科研项目方面，参与国家社科基金、文情中心一流学科建设、中国工程院战略研究与咨询重大项目等项目。文体生活方面，先后担任研会学术部副部长、文体部兼生活部部长。
社会实践方面，参与科学计量与科技评价天府论坛等6项会务工作，以及国科大2023“青年服务国家”社会实践、社会调查活动专项两项重大社会实践。
公共服务方面，运营学术自媒体，累计5k+粉丝，播放量达40万。

关于我的一切（英文版）
======
I was born and raised in Tianjin. I obtained BS of Information Management and Information System in [西南大学计算机与信息科学学院(School of Computer and Information Science,The Southwest University)](http://cis.swu.edu.cn/) in 2021,advised by [Prof. Li](http://jyxb.swu.edu.cn/s/jyxb/jjfjs/20220408/4746449.html). Then, I passed the graduate examination in 2022. Now, I'm a first year graduate student from [中国科学院文献情报中心(National Science Library)](http://www.las.cas.cn/). I’m very fortunate to be advised by [Prof. Wen](https://people.ucas.ac.cn/~0058187)and[Prof. Yang](https://people.ucas.edu.cn/~yn).In the future, maybe my research interest includes scientific dataset recommendation and sharing.

You can find my CV here: [XX's Curriculum Vitae](../assets/Curriculum_Vitae.pdf).

[Email](mailto:berry_borui@163.com) / [Github](https://github.com/QiuDi233) / [Wechat](../images/wechat.jpg) / [CSDN](https://blog.csdn.net/qd1813100174?spm=1000.2115.3001.5343)


A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
