Reviewers' comments:

## Reviewer #1: 

The paper presents some details on Geopyter, a hub for the distribution of contents in computational and spatial analytic instruction. It shows the design of the system and explains the types of innovative workflows that it enables for lecturers. I believe the effort is very promising and having the paper to both explain and advertise the initiative is worthy of publication by JGSY. However, I believe there are some points that can improve the contribution of the paper, as follows.

1. On page 4, line 21, please write in full the acronym MOOC. **Although MOOC had been defined earlier, I've changed to just 'online course'.**

2. On page 5, the authors try to explain what they call Atoms, Sessions and Modules. The differentiation between these is however not very clear at this point. I suggest maybe adding a box to better explain what each of these elements is and how they differ. **A small table has been created to outline the relationship between these elements.**

3. On page 6, line 45, the paper explains how to select only parts of an Atom. The example with 'a.super' doesn't really deliver a good explanation, since it is not really clear what this class is. A more extensive example may be more helpful. **I have rewritten this section substantially so that it is, I hope, more clear to the reader and added a figure to try to illustrate what we mean *before* we get to the more complicated representation further on.**

4. Actually, to have a full Jupyter notebook as an example, with print-screens may be a good idea to achieve the objective of addressing the "the cohort of teachers at all levels" (p.11). On page 7, the authors present an example of how to include an Atom in a Session. However, for a teacher at a beginner level, it may not be clear where/how that code is supposed to be inserted. Hence, I believe having a full notebook as example would really be more helpful to achieve the beginner level of teachers. In my opinion, this is the greatest weakness of the paper: not showing a full example that can be used by beginners to build upon it and from there start creating their own Sessions with a mixing approach as proposed by the authors. I strongly suggest the addition of a full example to the paper. **A working repository has been created with useable content illustrating two of the potential applications for Geopyter. However, our feeling is that including full Python/Jupyter code here would be confusing.**

5. The url used for the include examples takes the reader to a BlueHost advertising page. The authors should change it. 

   <div style="color:red;font-weight:bolder;border:dotted 1px red;padding:5pt;" />Serge: this one is for you!</div>

6. The authors mention that as the user base grows, so will the contributor base and from there a cumulative circular causation would start operating to increase the platform. I remain, however, in doubt of how Geopyter will be able to organise all this varying mix of contents and keep all of it following standard patterns of coding, documentation, etc. It would be interesting to know how this is planned. **I have added a subsection regarding this issue: it's an important point and we have some experience navigating these issues thanks to one author's work with PySAL. Clearly, developing teaching resources is more challenging than developing executable code; however, we believe that by placing groups of related Atoms under the 'control' of a small number of dedicated contributors a degree of coherence of style and presentation will be developed such that students on an introductory or specialist module would not encounter wide variation.**

In sum, I believe the initiative, and hence the paper, is very interesting. However, I am not confident the paper can, as it currently stands, be of much help to beginning lecturers as it proposes. Some work on it is required in order to achieve this.

## Reviewer #2: 

This manuscript introduces a novel and innovative instructional system that integrates code with instructional material in mix-and-matchable Jupyter Notebooks. The manuscript is well written, but does have a few sections that mix technical concepts with domain concepts, for example. This is a useful contribution to the literature and with some minor changes is publishable. I added more detailed comments below.

How does Open Education Resources (OER) factor into this work? This is a growing movement in the education space and intersects with OSS and MOOCs as well. The authors should consider discussing this as related work. **We thank the reviewer for drawing our attention to this literature—it is not something we'd previously come across even though we have been regularly publishing our teaching material and source code!**

<div style="padding:5pt;border:dotted 1px red;color:red;font-weight:bolder">This is really useful. Looks like it actually does away with much of the MOOC stuff—well, I can work it in effectively. Probably a couple of paragraphs.</div>

- https://doi.org/10.1080/08923641003696588
- https://doi.org/10.1080/02680510802625443
- https://eric.ed.gov/?id=ED535639
- https://www.learntechlib.org/p/147891/
- https://doi.org/10.1080/02680510903482132
- https://doi.org/10.1080/13562517.2013.774354
- https://www.researchgate.net/profile/Jan_Hylen/publication/235984502_Open_educational_resources_Opportunities_and_challenges/links/54d321a80cf250179181779b.pdf
- https://doi.org/10.3402/rlt.v20i0.14395
- https://doi.org/10.1111/bjet.12438
- https://digitalcommons.georgiasouthern.edu/gera/2018/2018/33/
- https://doi.org/10.1080/01587919.2017.1369350

Introduction
P1l14 - I would recommend removing the 'online' qualifier and reference simply teaching of these technologies. **Done**

Pl15 - This is a jarring pivot that readers may not fully follow. Readers without a background in data science may not know that there is an 'open' ethos nor what an 'open' ethos entails. So a brief 1-sentence introduction for these topics may be useful. **First paragraph rewritten to remove reference to 'open' as this made it simpler while removing the jarring effect.**

I would recommend that the introduction introduce and cite Jupyter Notebooks. **We have added a single sentence to this effect though it is necessarily a bit 'sketchy' on the nature of Jupyter.**

Origins and Inspirations
P2l12 - This first paragraph mixes curriculum with software. It would be helpful to disentangle these two elements while also describing their interrelationships. **Tweaked to try to make this distinction more clear.**
P2l48 - space missing after Rey 2019 citation, the citation is the incorrect style. **Done.**
P2l50 - wrong citation style  **Corrected**
P3l16 - e.g., should be before the citation **Corrected**
P3l29 - the authors may consider broadening the quote to say something like: 'computational social/environmental/geospatial scientist' to make it more inclusive to a broader readership.  **Done.**
P3l34 - speed can also be an issue in these cases. **Indeed!**
P5l4 - An introduction of Git and Github would be helpful for readers that don't have a lot of experience with them. **We've tweaked this slightly to try to make their nature a bit more clear but think that a more detailed introduction to Git/GitHub is not appropriate in this article.**

Figure 1. This is a nice solution. The ability to test notebooks using the Markdown header hierarchy is very elegant. **Thank you!**

Use Cases
P8l22 - Define HE **Done.**

The descriptions in the use cases are clear. However, it would be nice to see a more specific use case with actual materials in addition to these broader discussion use cases. **This is was a request also made by Reviewer #1: it is difficult to know how we can provide a full demonstration of the tool *within* the article itself and we had always planned to provide a core set of 'Atoms' as part of the publication of the article, so we have opted to focus on the core concept(s) in the article and to leave a fuller demonstration for the 'Supplementary Online Materials'. However, we *also* recognise the challenges of getting one's head around the idea in the first place and have attempted to deal with this both by tidying up our explication and by offering more illustrations of how the process takes a document's implicit structure and uses that to extract relevant sections from another notebook.**

The rest of the manuscript summarizes the key points and extensions. I was happy to see the potential connection to other projects such as the Body of Knowledge.

## Reviewer #3: 

<div style="padding:5pt;border:dotted 1px red;color:red;font-weight:bolder">This critique is really the hardest to answer as it's clear that the reviewer doesn't really 'get' what we're doing. I kind of take this as a challenge to reformulate our article and make the applications more clear up front with the technical content coming a bit later...</div>

Fascinating to see how the development of this resource came about, and how its design aims to fill in a niche discovered within the teaching of spatial analytics. I was intrigued by the idea that this could connect the streams from the FOSS and MOOC movements, as the abstract pointed towards, but found myself not completely understanding how this fit in that trajectory after all in the sections describing the process. I believe a better historical grounding with actual telling of timelines and developments in those powerful movements would have situated this GeoPyTeR story more strongly. **We hope that the substantial edits and incorporation of OER literature has helped to position GeoPyTer more clearly in the reviewer's mind. We would suggest that a timeline is not strictly relevant here as GeoPyTer is not a MOOC and does not depend on any specific FOSS technologies other than iPython/Jupyter (where we've slightly adjusted our initial presentation of the material) to make this more clear.**

That said, this design narrative seems a bit smoothed over. It omits reflection on some of the challenges, and glosses over what might be a good opportunity to reveal what might be remaining or conquered flaws, false starts, wheel-reinventing, or other elements that surely hold some insights for audience of this journal. **We have tried to expand on some of the unresolved challenges and in particular that of ensuring overall coherence in the examples (including data!) provided. Space constraints precluded a more thorough examination of the 'false starts', but we hope that revisions to the initial submission have helped in this regard.**

Not being a developer, I had a hard time following some of the heavy jargon in many spots that might only need some signposts to reach a broader community of interest. It is important to identify the "instructors" audience more clearly: I am assuming that this is for university faculty teaching to undergraduates / graduates at mostly US / European institutions, but if that assumption is wrong, that underscores the need for the author to make that explicit. **We have specified a bit more clearly that the default assumption here is of technically sophisticated HE staff, but we also wish to be highlight that this is not the *only* group that could make use of such material. Hopefully, our edits and additions (especially the illustrative material) have mitigated at least a little bit some of the more forbidding jargon.**

The introduction should start with the problem and purpose. Two other brief mentions seem missed opportunities: the reference to "best practices" and reference to the Body of Knowledge, which seem could catapult uptake of such a resource. **We have included an earlier reference to the BoK where we think that this helps to set expectations about the managed nature of contributions.**

Finally, it surprised me that the use case scenarios were only "potential use" and not actual end-user cases. This led me to wonder who is using the resource in what actual context? How many? where? for which content? for which students? Does it rise to the usage potential with MOOCs and reach a massive audience? would some of the pitfalls of MOOCs befall this resource as well or not? How might some of the chalelnges of the open movement be resolved or remain? This also reveals how the article is devoid of time and timelines, which would orient the reader. **This does not replace or augment MOOCs, nor do we expect it to have the same kind of impact as it sits alongside such tools within domains where specific technical training is called for. We have used it in fits and starts already, and have made a set of Atoms and Sessions available via the Supplementary Online Material, but our own challenges of not having enough time to either finish development and write up the tool for publication have hampered wider adoption. We are hoping to secure funding to allow further development but felt that we needed to 'get the word out'.**