*=> An in-depth introduction to Open Source with some specific examples taken from the approach used by the Quasar Framework, as we intend to use this tutorial as training and reference for all forthcoming (and existing) contributors.*

### Repository 
https://github.com/nothingismagick/quasar-articles/blob/master/tutorials/openSourceTutorial.md

### What Will Be Discussed?
> You will learn about Open Source and best-practices to make sure that your contributions are compliant.

**Introduction**
- You will learn about the difference between copyright, licensing and attribution
- You will discover the meaning of "Free/Libre and Open Source Software"
- You will find out what is meant by "GPL compatibility"
- You will learn about license discovery and licensing agreements
- You will learn how to use code and other assets that are open-source

**Your Identity and Rights**
- You will learn about "Non-Disclosure Agreements" (NDA)
- You will learn about "Contributor License Agreements" (CLA)
- You will learn how to become a "verified" contributor
- You will learn why "developer certificates of origin" are used
- You will learn what "signed-off-by" means
- You will learn about "release" forms
- You will learn about "provenance"
- You will learn about "changing licenses"

**License Types**
- Licenses for code
- Licenses for text / documentation
- Licenses for artwork / design / video
- Licenses for fonts

### Requirements
- You must read English proficiently
- A basic understanding of `git`  
- Knowledge of file types relevant to your field of activity 

### Difficulty
- Basic to medium

# Tutorial Contents
> This tutorial is a primer for those who are interested in contributing to open-source projects. It may also be useful for active contributors who were always curious about advanced topics. And finally, because licensing can be very contentious, this is also a text for those who want to engage in a discussion about open-source. Although we are using specific examples from the "Quasar Framework", the issues herein are relevant across the spectrum of open-source software development.
> 
> Our hope is that you will gain deeper insight into all of the great things (and potential pitfalls) surrounding licenses in the world of open-source software. The Introduction is a great place to start, as it defines some of the terms this tutorial will constantly return to. It will also teach you about some simple methods for making sure that your contributions are compliant with the licensing scheme taken by the project you are working with. Then, it begins a discussion about you, the contributor, and the rights and responsibilities that you have. Finally, it will go into depth about various domains of licensing, including code, copy, design and fonts.

## Preface
> Some software has source code that only the person, team, or organization who created it—and maintains exclusive control over it—can modify. People call this kind of software "proprietary" or "closed source" software.
> ...
> Open source software is different. Its authors [make its source code available](https://opensource.com/business/13/5/open-source-your-code) to others who would like to view that code, copy it, learn from it, alter it, or share it. [LibreOffice](https://www.libreoffice.org/) and the [GNU Image Manipulation Program](http://www.gimp.org/) are examples of open source software.

https://opensource.com/resources/what-open-source

Every act of creativity can be attributed to someone or to a group of people working together. In fact, it is actually quite silly to think that anything exists in a vacuum. We are all connected, and ideas are things that often take on a life of its own. However, in these modern times many people have started protecting their ideas from being stolen by giving it away - by publishing their work so  that other people are empowered and invited to contribute to the project - or even take it in an entirely different direction.

Not unlike the way that guilds of centuries past protected their trade-secrets, the excuse of a "proprietary" protection of ideas and an enshrinement of "closed source" in legislation and free-trade agreements can directly be traced to many of the problems that turbo-capitalism has unleashed on our planet. But guess what - there is something you can do. You can participate in the open-source movement.

## Introduction
### Copyright, Licensing and Attribution

It is generally accepted in modern democratic society that a notice of copyright is required as a preface for all licenses, because someone has to be responsible for declaring how the thing being licensed can be used. In a strange (but somehow logical) twist, if you wish to share your work as Public Domain, Copyleft or CC0, you have to first declare that you are the owner of your work (and that everyone who contributed to it agrees with you on that matter). 

Once a copyright is declared, the copyright holder may inform readers and users of the code / text / art under which circumstances it is appropriate to use it. No matter what licensing approach the original author / copyright holder takes, it is always appropriate to retain copies of these licenses in the repository  hosting your work should it use open-source licensed works of third parties. It is never ok to remove or edit license files or license references in the headers or metadata of source files - because that is literally stealing and a form of plagiarism. 

As long as "consumers" of your built artefacts (website, app, etc.) are informed to where they can see the licenses of the third-party projects that you have used to build your project, you can avoid shipping them.

If you do decide to use anything done by a third-party within your work, except for public domain works (which I personally believe you should also cite), you are required (both legally and morally) to cite the source. This is called **attribution**, and a general rule of thumb is that you should include references to all of the code you are using. We will get more into this later on in the tutorial, because there are different requirements depending upon the domain of the resource being attributed.

### "Free/Libre and Open Source Software"
> The term "open source" refers to something people can modify and share because its design is publicly accessible.
> 
> https://opensource.com/resources/what-open-source

There is a perpetual discussion by FLOSS hardliners about the degree of **freedom** inherent in "open" source - and even what **free** means. However, it is probably a good idea to go back in time to 1998 and [read this article](https://opensource.com/article/18/2/coining-term-open-source-software) by the woman who came up with the name "open source": Christine Peterson. Although Richard Stallman and Linus Torvalds are two of the most successful, visible and vocal proponents on the matter; the point is that even though the term began as a "marketing device", it stuck and changed the lives of everyone on the planet - arguably for the better. 

Stallman and the "Free Software Foundation" (FSF), who have arguably been around the longest, will define freedom as an important part of open source, because your freedom to use the code and change it is also a responsibility that you bear in the name of the entire community. In fact, if it is not totally free, 

<center><strong>What is free? What is libre?</strong></center>

If one ignores for a moment the annoying fact that *free* also means "doesn't cost any money" (which is the main argument for adding the word libre), there is still an unresolved semantic issue, in fact, one that will likely never resolve: 
 
Depending upon your perspective, the Gnu Public License isn't ABSOLUTELY free, because it comes with the requirement that you must return changes that you make to the code back to the community - and being free would mean you get to decide how to work and what to do with the code you use. At the same time and on a different spectrum, there are those who consider the MIT license not to be entirely free. They do so because there are circumstances where the code can be permissibly changed and not returned to the community - in a sense "imprisoning" the code.

> There is no right or wrong answer here, because it is a matter of perspective - however every developer and every organisation needs to decide for themselves where they want to put the focus of their attention. At the Quasar Framework, we are not purists in the sense that we believe Code is in and of itself a spiritual being deserving of transferrable rights. If perhaps we were working on the Linux kernel that might be different - but we are more concerned with the human side of code and believe that the people who use our project should have the ultimate freedom of choice to do what they want. This is why we have taken the "permissive" approach and chosen the MIT license. 

There is often a great deal of discussion around "how free to make the code". I propose that you ask yourself four questions:
1. Do you prefer to work alone?
2. Are you worried about people stealing your idea?
3. Have you written all of the code yourself, including the libraries?
4. Have you signed any type of Non Disclosure Agreement regarding the work in question?

If you answered **no** to any of these questions, then using an open source license for your work is a great way to go. 

If you answered **yes** to all of these questions, then considering licensing your work as open-source is probably still one of the best ways to protect your work and make sure that it has an impact on the rest of the world. Just think of it this way: if all of the software around you today was not open source, would you still be able to work as you do? Don't you owe it to the community to share your work? 

### Permissive vs. Copyleft licensing
One of the common misconceptions about licensing your project with GPL is that it will prevent corporations from taking your idea and using it to make money - all without giving you any cut of the profits. This is patently untrue. If someone wants to steal your code and break the law, they will. If a corporation wants to use your GPL library, they can isolate it from the rest of their system and reveal nothing of their proprietary code. If this is your biggest concern, then stop, go back to the beginning of this tutorial and start from the beginning. 



The biggest issue is what happens when you include GPL-licensed code in your project, because GPL is very strict and can actually force you to reveal your code. Contrary to popular belief, 

GPL compatibility 


### License discovery and licensing requirements
Using open-source software in your projects is a great thing, but you need to stay diligent, especially when you are contributing work to another project. And this is doubly true if you are required to do reporting about license compliance (for example in the case of public agencies or within corporate legal firewalls). In any case, it can be a bit of a hassle to manually go through and track down all the license files.

There are a few projects that treat this issue of discovery, such as [nlf](https://www.npmjs.com/package/nlf) and [https://fossa.io/](https://fossa.io/ "https://fossa.io/") and specifically [their free **CLI** that does not require registration](https://github.com/fossas/fossa-cli). 
```
$ nlf --summary detail > nlf.txt
```
[Here is a report made from the Quasar repo using the **nlf** approach.]( https://raw.githubusercontent.com/nothingismagick/quasar-articles/master/tutorials/nlf_report_licenses_quasar.txt.md)

If you want to see a license report generated by the **fossa CLI** in your repository, after following their install instructions, you can just use this command:
```
$ fossa report licenses > fossa.txt
```
[Here is a report made from the Quasar repo using the **fossa cli** approach.]( https://raw.githubusercontent.com/nothingismagick/quasar-articles/master/tutorials/fossa_report_licenses_quasar.txt.md) As you can see, the great majority of modules use the MIT license, but several are not clear from the report alone: 15 of the projects were not autodetected by **fossa**. I followed each of the links, tracked down their licenses, and made a note not only of the license, but that I was the one who did it. 

Furthermore, I detected that only one of our libraries (stylint) is requires a GPL license, but the developers have a license conflict in the declaration in the  package.json (GPL-2) and the actual license file (GPL-3).  

 That is what you will need to do as well. Should a license file not be included in the project, and you cannot find one, it is wise to contact the author.

**A word of caution**: These automated systems are not foolproof (e.g. a module about license detection may detect multiple licenses, even though it is itself using another license). If you are bound by regulatory compliance, you need to go through them all by hand - and don't be afraid to reach out to the author if you need clarification. 


### Using open-source
If you use anything that is open-source, you must declare it and make the original licenses easily accessible. If you are using, for example, node modules in your project, then these licenses are available in the source code of the project when someone downloads the project files and "installs" the dependencies. You can usually find it as a file named `LICENSE` in the root folder or in the "license" field in the `package.json`

Generally this is enough, however if you make any changes to the original library, you may be required to notify and / or submit these changes back to the community. This depends on the license type, but we will cover licensing specifics in the final section.

> **Stack Overflow**: A common pitfall is to merely copy and paste things that you find on stackoverflow.com - but this is dangerous, because even though it is implied that the user is sharing this information, you do not know with 100% certainty that it is appropriate (or permitted) to use the code example 1 to 1. The common practice of citing the resource is better than nothing, but you should really consider rewriting the example to fit your code style, the needs of your project AND reference the source as "inspiration".

In the case of images, you should do one or more of the following:

1. Name the file accordingly
2. Put license information in a watermark in the file
3. Inject the information into the metadata of the file
4. Cite the image sources / licenses directly after the image if possible
5. Put this same information in a footnote / endnote / linked document
6. Place license information or licenses and release form-cover-sheets in the repository in the same folder as the image or some other delegated location

## Your Identity and Rights
- You will learn about "Non-Disclosure Agreements" (NDA)


### What is a Contributor License Agreement (CLA)


### Become a "verified" contributor
https://stackoverflow.com/questions/10161198/is-there-a-way-to-autosign-commits-in-git-with-a-gpg-key

### What is a "developer certificate of origin"
https://developercertificate.org/

### What does "signed-off-by" mean, and how to do it
https://stackoverflow.com/questions/1962094/what-is-the-sign-off-feature-in-git-for

### When do I need to get "release" forms
A release form is generally required when making photographs of people and private property - and using them for any non-private purpose. Although specifics vary from jurisdiction to jurisdiction, it is very important that you get people to sign a release form, and if it is clear WHERE the picture was taken, then you might need to get permission of the owner.

> One clever way to deal with a release form for humans (if they genuinely want to support you) is a so-called "reciprocal pay". Before the photo-shooting, prepare two receipts. On one receipt you pay them e.g. 5 EUR for being a model. On the other receipt, they pay you e.g. 5 EUR for a copy of the photograph. The rule (got the cash, keep the copy) applies, so each party has one original receipt and one copy receipt. You send them a digital copy of the final image as a link to the open-source repository where it was used, and note this on the copy of the receipt they gave you. Keep this in your own records, and everybody is happy.

If you do use photographs of people that you have made and submit them to open source projects, you need to be able to prove that the person  

###  How can I document "provenance"

### Can you change licenses?

## License Types


### Major licenses for code
- [Github's License Helper](https://choosealicense.com/)
- [The exhaustive list by the GNU Foundation](https://www.gnu.org/licenses/license-list.html)
### Important licenses for text / documentation
- Creative Commons
- Free Documentation License https://www.gnu.org/licenses/fdl.html
### Licensing artwork / design / video
- Copyright
- Release forms (Right to the person)
- Notification
1. Name the file accordingly
2. Put license information in a watermark in the file
3. Inject the information into the metadata of the file
4. Cite the image sources / licenses directly after the image if possible
5. Put this same information in a footnote / endnote / linked document
6. Place license information or licenses and release form-cover-sheets in the repository in the same folder as the image or some other delegated location

#### Considerations about your place of residence
#### Consideration of the contents of your work

### Font licenses
Of the hundreds of fonts listed at [Google Fonts](https://fonts.google.com/attribution), there are exactly two different licenses used: Either the Apache License v2, or the SIL Open Font License v1.1. The vast majority are OFL
#### SIL Open Font License (OFL)

- ![OFL](https://scripts.sil.org/cms/sites/nrsi/media/OFL_logo_rect_color.png) [OFL-FAQ web version (1.1-update5)](https://scripts.sil.org/cms/scripts/page.php?item_id=OFL-FAQ_web)

# Final Words
Just because you "open" your work to collaboration from others, this is not the end of the story. Just because you slap a Creative Commons license on a photoshop file does not mean it is open and free. The degree of openness of an asset or project is also determined by the operating system and the software needed to use and or modify the file. Please consider publishing not only the results of the process of your work, but also inform people about how you did it.

# Further Resources
In case you want to go more into depth about these topics, we have a few additional resources that we highly recommend:
- Stallman's distinction between [FLOSS and FOSS](https://www.gnu.org/philosophy/floss-and-foss.en.html)
- This chapter of the [ZeroMQ Guide](http://zguide.zeromq.org/page:all#toc141) goes into great detail about governance in open-source projects with the specific example of their community


#### Proof of Work Done (Authorship)
The original version of this article has been compiled and written by @nothingismagick https://github.com/nothingismagick

#### License
This work and all derivatives are [licensed under the FDL 1.3](https://github.com/nothingismagick/quasar-articles/blob/master/LICENSE).

> Written with [StackEdit](https://stackedit.io/).
