*=> A general introduction to Open Source with specific examples taken from the approach used by the Quasar Framework, as we intend to use this tutorial as training and reference for all forthcoming (and existing) contributors.*

#### Repository
https://github.com/nothingismagick/quasar-articles/blob/master/tutorials/openSourceTutorial.md

#### What Will Be Discussed?
> You will learn the basics about licenses in Open Source software and best practices to make sure that your contributions are compliant.

**Introduction**
- You will learn about the difference between copyright, licensing and attribution
- You will discover the meaning of "Free/Libre and Open Source Software"
- You will find out what is meant by "GPL compatibility"
- You will learn about license discovery
- You will learn how to use code and other assets that are open-source

**License Types**
- Licenses for code
- Licenses for text / documentation
- Licenses for artwork / design / video
- Licenses for fonts

**Your Identity and Rights**
- You will learn about Contributor License Agreements (CLA)
- You will learn how to become a "verified" contributor
- You will learn why "developer certificates of origin" are used
- You will learn what "signed-off-by" means
- You will learn 

#### Requirements
- You must speak English proficiently
- A basic understanding of `git`  
- Knowledge of file types relevant to your field of activity 

#### Difficulty
- Basic to medium

# Tutorial Contents
> This tutorial is a primer for those who are interested in contributing to open-source projects. It may also be useful for active contributors who were always curious about advanced topics. And finally, because licensing can be very contentious, this is also a text for those who want to engage in a discussion about open-source. Although we are using specific examples from the "Quasar Framework", the issues herein are relevant across the spectrum of open-source software development.
> 
> Our hope is that you will gain deeper insight into all of the great things (and potential pitfalls) surrounding licenses in the world of open-source software. The Introduction is a great place to start, as it defines some of the terms this tutorial will constantly return to. It will also teach you about some simple methods for making sure that your contributions are compliant with the licensing scheme taken by the project you are working with. Then it will go into depth about various domains of licensing, including code, copy, design and fonts. Finally, it wraps up with a discussion about your identity and your rights.

## Introduction
### Copyright, Licensing and Attribution
Every act of creativity can be attributed to someone or to a group of people working together. In fact, it is actually quite silly to think that anything exists in a vacuum. We are all connected, and ideas are things that often take lives of their own. However, in these modern times many people have started protecting their ideas from being stolen (or worse) by claiming copyright and publishing their work in a way that enables other people to contribute to the project - or even take it in an entirely different direction.

It is generally accepted that a notice of copyright is required as a preface for all licenses, because someone has to be responsible for declaring how the thing being licensed can be used. In a strange (but somehow logical) twist, if you wish to share your work as Public Domain, Copyleft or CC0, you have to first declare that you are the owner of your work (and that everyone who contributed to it agrees with you on that matter).

Once a copyright is declared, the copyright holder may inform readers and users of the code / text / art under which circumstances it is appropriate to use it. No matter what licensing approach the original author / copyright holder uses, it is always appropriate to retain copies of these licenses in the repository hosting your work. 

If you do decide to use anything done by a third-party within your work, except for public domain works, you are required (both legally and morally) to cite the source. This is called **attribution**, and a general rule of thumb is that you should include references to all of the code you are using. We will get more into this later on in the tutorial, because there are different requirements depending upon the domain of the resource being attributed.

### "Free/Libre and Open Source Software"
> The term "open source" refers to something people can modify and share because its design is publicly accessible.
> 
> https://opensource.com/resources/what-open-source

There is a perpetual discussion by the FLOSS hardliners about the degree of openness inherent in "open" source - and even what "freedom" means. However, it is probably a good idea to go back in time to 1998 and [read this article](https://opensource.com/article/18/2/coining-term-open-source-software) by the woman who came up with the name "open source": Christine Peterson. Although Richard Stallman and Linus Torvalds are two of the most successful, visible and vocal proponents on the matter; the point is that even though the term began as a "marketing device", it stuck and changed the lives of everyone on the planet - arguably for the better. 

Stallman and his "camp" will define freedom as an important part of open source, because your freedom to use the code and change it is also a responsibility that you bear in the name of the entire community. (In an interesting irony, the Gnu Public License isn't ABSOLUTELY free, because it comes with the requirement that you must return changes that you make to the code back to the community.)

In fact, there is often a great deal of discussion around "how free to make the code". I propose that you ask yourself three questions:
1. Do you prefer to work alone?
2. Are you worried about people stealing your idea?
3. 

If you answered yes to 

### MIT versus GPL


### License discovery and licensing requirements
Using open-source software in your projects is a great thing, but you need to stay diligent, especially when you are contributing work to another project. And this is doubly true if you are required to do reporting about license compliance (for example in the case of public agencies or within corporate legal firewalls). In any case, it can be a bit of a hassle to manually go through and track down all the license files.

A great project that solves this quite elegantly is [https://fossa.io/](https://fossa.io/ "https://fossa.io/") and specifically [their free **CLI** that does not require registration](https://github.com/fossas/fossa-cli). If you want to see a license report generated by their **CLI** in your repository, after following their install instructions, you can just use this command:
```
$ fossa report licenses > fossa.txt
```
[Here is a report made from the Quasar repo using this technique.]( https://raw.githubusercontent.com/nothingismagick/quasar-articles/master/fossa_report_licenses_quasar.txt.md) As you can see, the great majority of modules use the MIT license, but several are not clear from the report alone. As you can see, 15 of the projects were not autodetected by fossa. I followed each of the links, tracked down their licenses, and made a note not only of the license but that I was the one who did it.

# License Types


## Major licenses for code
- [Github's License Helper](https://choosealicense.com/)
- [The exhaustive list by the GNU Foundation](https://www.gnu.org/licenses/license-list.html)
## Important licenses for text / documentation
- Creative Commons
- Free Documentation License https://www.gnu.org/licenses/fdl.html
## Licensing artwork / design / video
- Copyright
- Release forms (Right to the person)
- 
### Considerations about your place of residence
### Consideration of the contents of your work
## Font licenses
Of the hundreds of fonts listed at [Google Fonts](https://fonts.google.com/attribution), there are exactly two different licenses used: Either the Apache License v2, or the SIL Open Font License v1.1. The vast majority are OFL
#### SIL Open Font License (OFL)

- ![OFL](https://scripts.sil.org/cms/sites/nrsi/media/OFL_logo_rect_color.png) [OFL-FAQ web version (1.1-update5)](https://scripts.sil.org/cms/scripts/page.php?item_id=OFL-FAQ_web)
#### 

# Your Identity and Rights
## What is a Contributor License Agreement (CLA)


## Become a "verified" contributor
https://stackoverflow.com/questions/10161198/is-there-a-way-to-autosign-commits-in-git-with-a-gpg-key

## What is a "developer certificate of origin"
https://developercertificate.org/

## What does "signed-off-by" mean, and how to do it
https://stackoverflow.com/questions/1962094/what-is-the-sign-off-feature-in-git-for

# Final Words
Just because you "open" your work to collaboration from others, this is not the end of the story. 

# Further Resources
In case you want to go more into depth about these topics, we have a few additional resources that we highly recommend:
- Stallman's distinction between [FLOSS and FOSS](https://www.gnu.org/philosophy/floss-and-foss.en.html)
- This chapter of the [ZeroMQ Guide](http://zguide.zeromq.org/page:all#toc141) goes into great detail about governance in open-source projects with the specific example of their community
https://stackoverflow.com/questions/1962094/what-is-the-sign-off-feature-in-git-for


#### Proof of Work Done
This article is entirely the work of @nothingismagick https://github.com/nothingismagick

> Written with [StackEdit](https://stackedit.io/).
