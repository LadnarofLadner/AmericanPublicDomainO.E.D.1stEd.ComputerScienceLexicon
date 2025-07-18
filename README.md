# AmericanPublicDomainO.E.D.1stEd.ComputerScienceLexicon


GOAL : Production of an Open-Source, Public Domain, 1st Edition Oxford English Dictionary, "page-ified" (paginated?), "lex-ified" (lexicon-ized?), for computer science, APIs, speech generation, speech recognition, A.I. and etc.

(DISCLAIMER: I clicked GNU 3.0 GPL, and almost chose MIT license for this project, but after reading a bit more about the differences, I am leaning towards a re-launch of this project under "The Unlicense". In short, Copyleft principles should abound for this project, as the English language clearly belongs to all of us. I apologize for my initial neglect of--and reflexive and impetuous disregard for-- the legal particulars.)

Authored by, Randall Meyer, Evolution Biologist (and Memeticist) "Extraordinaire"; Hilo, Hawaii; July 15, 2025 (start date):

OK, just last week, or in the previous week, or two (or five?), I asked Google-A.I. if there was a legitimate place to get a scanned copy of the Oxford English Dictionary. Not that I am squeamish about illegitimate places to acquire scanned texts (as that seems to be the primary mode for the communication of intelligent ideas, these days! Illegitimately!!), but, I figured if I was to make it into a lexicon, similar to the CMU dictionary I already knew of, I would need something that was relatively permissive, especially if I wanted it to be open-source, to be shared, in the best of Linux, UNIX (Eunuchs!), FSF, and FOSS ethical traditions.

Some years ago, while fiddling with a "speakjet" speech chip, and then, later, with a Linux program called "festival" (see Alan Black's work, at Edinburgh and Carnegie-Mellon; see also, Fest-Vox, and Sphinx; and the unassociated espeak, and similar open-source, speech phoneme concatenators), I happened upon the CMU-dict, a digitized list of approx. 134,000 pronounceable, machine-pronounceable, dictionary entries, utilizing phonemes, IPA, and ARPABET binary codes (I will note, here, that all versions of CMU-dict up to version 0.6-0.7 are and were in the public domain, with versions after about 1998-2014? adopting a 2-clause BSD license).

So, I wasted a bit of time on the internet archive downloading some very over-sized files (15 files, pdfs, about 42 GB worth! The "text-fied" files listed next to these pdfs were barely Megabytes, or 10s of MB, if I recall correctly.) but I paid little attention to the licenses or copyrights, or even print or copyright dates. I simply assumed the internet archive had sorted that part out, but I reconsidered this, when I decided that this project should occur here, on Github, and that this project should include other people; I  will not assume those files (42 GB data set) are free to use in this project.

So, I then asked Google-A.I., again, if any O.E.D. was in the public domain. Google answered, yes, in the USA, the 1st edition printing is defintiely in the public domain, as of 2024. It is most certainly 2025, now, so I care not what month or date of 2024 it entered public domain. We seem to be in legal and legitimate territory, here.

And so, my next question to Google-A.I. was "Where can I get pdf copies of the 1st Ed. O.E.D., the one that is in the public domain?". Google responded with a fine link to a UPENN website, which, incidentally, just linked to the 15 particular files (10 volumes, I-X) on the internet archive. These volunmes were, luckily, more compact, coming in at about 4 GB. Here is the link, as well as two others that might prove useful to us, in this project ( (1) https://onlinebooks.library.upenn.edu/webbin/metabook?id=newenglishdictionary (2) https://onlinebooks.library.upenn.edu/search.html (3) https://onlinebooks.library.upenn.edu/webbin/book/search?author=&amode=words&title=Oxford+English+Dictionary&tmode=words&c=x ).

It is also worth noting here, that, if one needs metadata files associated with these pdfs, the internet archive offers about 17 different types, for each of the 15 links that the UPENN "Online Books" website points to. (The earlier, larger files I had downloaded, at 42 GB, I had actually taken 30 files, two of each, one labelled "pdf" and one labelled "pdf+txt"). But the archive.org items linked to by the UPENN library did not have an entry for "pdf+txt". Those 15 links tended to have about 17 different options for different kinds of metadata; namely, .pdf, .txt (html?/txt?), JSON, chOCR, hOCR, OCR, epub, daisy, abby-ZIP, J2-ZIP, JPEG-ZIP, JP2-ZIP, torrent, and others. It is my intention to provide a mirror of that pdf data, here, alongside 15 file folders containing the 15,000 pages that I have separated with the "poppler" utility "pdfseparate" (see Appendix I. for "poppler" license info). The file naming should be automatic and standard and self-explanatory. Each of the 15 file folders will contain between approx. 500 and 2,000 pages, depending upon size of the original file; the size of the original book. (See Appendix II, below: for my evolving notion of what this project can be. I see it might not be possible to host the pdf dictionary data here, and perhaps I must cobble together only the code which will act upon the dataset and, then, I may invite users and modifiers of my code to download the datasets, i.e. the pdf of the dictionary, on their own.)

UPENN's "Online Books" lists the entries for the files and the dates of the book's original printing, as follows: 

"
Volume I: A-B (ca. 1888). Some initial pages, including the front matter and part of the preface, are missing from this scan.
Google Books also has the first part of volume 1 (up to "Axiform") in the 1888 edition. It includes all front matter and the full preface, but might not be accessible outside the United States.
Volume II: C (1893).
Volume III, Part I: D (1897).
Volume III, Part II: E (1897).
Volume IV: F-G (1901).
Volume V: H-K (1901).
Volume VI, Part I: L (1908).
Volume VI, Part II: M-N (1908).
Volume VII: O-P (1909).
Volume VIII, Part I: Q-R (1914).
Volume VIII, Part II: S-Sh (ca. 1914).
Volume IX, Part I: Si-St (1919).
Volume IX, Part II: Su-Sz and T-Th (1919).
Volume X, Part I: Ti-U (1926).
Volume X, Part II: V-Z (1928).
"


The Internet Archive, hosting those files, names thefiles like this (I have added the year printed, following the filename, in parentheses, thusly : (18xx) ):

"
1_oed01arch_missing pages	 (1888)
2_oed02arch	(1893)
3_oxforddictionaryv3p1unse_a5h6	(1897)
4_oxforddictionary0003unse	(1897)
5_oed04arch	(1901)
6_newenglishdict05murrmiss	(1901)
7_oed6aarch	(1908)
8_oed6barch	(1908)
9_newenglishdic07murruoft	(1909)
10_oed8aarch	(1914)
11_newenglishdictio82murruoft	(1914)
12_oed9aarch	(1919)
13_oed9barch	(1919)
14_newenglishdictio101murruoft	(1926)
15_newenglishdictio102murruoft	(1928)
"


You'll also note, that onlinebooks, the UPENN page, mentions that : "This is a "meta-book", which stitches together separate files elsewhere on the Web as they appeared in a previously published book. It is subject to removal if someone produces an integrated edition. If that happens, The Online Books Page will point to the integrated version.".

Perhaps this repsotory can become the "edition" that will be that "integrated edition" that they refer to? Perhaps, an O.E.D., downloadable, open source, public domain, searcheable by first three letters (or more) and returiing the entire entry upon such query, would be a valuable resource? Perhaps it woulod be valubale to end-users, as an excellent and acedmically authoritative free dictionary, but also as a lexical tool for A.I. researchers, and speech sysnthesis researchers?

The "text" versions are mere megabytes or 10s or maybe 100s of Megabytes. I don't recall, off the top of my head. But once I have split the pdf pages and placed them in their own, separate, 15 directory folders, with predictable names, referenceing what page order each individual one-page pdf is, some sort of C or python or perhaps bash script can be applied to pick out all the bold text. This seems to me to be the easiest way to find the likely, possible, probable, lexical items on each page.

I envision a simple script that will append the number fo probable lexical items to the end of the filenamwe, and then "save as", this new file name. _0 would be zero bold items. _7 would be seven bold items, and thus, seven possible lexcical items.

Lexical items bridging several pages would have to be handled by a separate program, applied after the first one (beacuse my mind thinks small, and in little, incremental steps).

It is possible even, that I must first convert these single page .pfd files into something more "readable", as an image, in order to extract, or count, the bold sections.

These bold sections should then be cross-referenced to the "text-ified" pdf files, as available for download from the internet archive.

I don't know if this "cross-referencing" will include my earlier 48 GB of downloads, wherein the "pdf+txt" file was available. Perhaps it will only use the UPENN pointed-to 15 files, as their ".txt" files are much smaller and simpler, and track directly to our dataset, the one under study. i.e. the EXACT pdfs that I have split apart and paginated.

Also, the UPENN-pointed-to OED files on intenet archive have many metadata files. I will download them into my own personal data repsository, and possibly put them onto githubs servers. Its possible I can supply all the meatdata needed for this project on this gutgub repository MINUS the pdfs themselves. Internet archive can continue to hiost those.

Public computer... my time has run out today ... press save ... ttyl !!!!

Signed, Randall Meyer, 2:11 PM ; July 15, 2025. A day after my 45th birthday !




APPENDIX I:

"
SANDBOX: FIX THIS PARAGRAPH LATER : 

The Linux utilities pdfseparate and pdfunite are provided by the Poppler utilities package, which is free and open-source software. 

The Poppler utilities are primarily licensed under the GNU General Public License (GPL). Specifically, this includes GPL-2.0-only, GPL-3.0-or-later, LGPL-2.0-or-later, LGPL-2.1-or-later, MIT, and HPND-sell-variant licenses. 

This means you are generally free to use, distribute, and modify pdfseparate and pdfunite, as long as you adhere to the terms of the chosen GPL version.

Google-A.I. does not seem to think that this license would limit distirbution or modification fo the separated or combined files, after use of the pdfseparate and pdunite "poppler" utilities. I will assume that the files, once split apart into individual IO.E.D. 1st edition pages, are as frewe to sue an d utilize and modifiy as the original total fiels were. i will also assume that other imaging sioftware that we use to fruther process these files place no trestircitons on end use of our data. I wil do SOME due diligience, to make certain I am using copyleft softwware with permsissive rights, but I will not be taking on the role of lawyer here. Somwe of the softawre I / We need in this project must be written from scratch, or preferebly will eb written from scratch, so it is probabkly a moot point.
"



APPENDIX II :


"

I asked Google-A.I. the following :


What is the most amount of data that a github repository will tolerate for a user to put on their website to host?


AI Overview

To understand the data limits for a GitHub repository being used to host a website (like with GitHub Pages), it's important to consider several aspects:

1. Overall repository size limits
GitHub recommends keeping repositories small, ideally under 1 GB, and strongly recommends staying below 5 GB.
While exceeding 5 GB is technically possible, GitHub Support might contact you to address excessive use of their resources if your repository significantly impacts their infrastructure.
Free and Pro GitHub accounts have a 2 GB limit per repository, while GitHub Team has a 4 GB limit, and GitHub Enterprise Cloud has a 5 GB limit.

2. Individual file size limits
GitHub blocks individual files larger than 100 MB.
For files between 50 MB and 100 MB, you'll receive a warning, but you can still push the file (though removing the commit is advised for performance).
If you're uploading files through the browser, the limit is even lower, at 25 MB per file. 

3. GitHub pages specific limits
GitHub Pages source repositories have a recommended limit of 1 GB.
The published GitHub Pages site itself (the actual website content) should be no larger than 1 GB.
There's a soft bandwidth limit of 100 GB per month for GitHub Pages sites. If your site significantly exceeds this limit, GitHub might disable your account or throttle your file hosting.
GitHub Pages deployments have a timeout of 10 minutes.
There is a soft limit of 10 builds per hour for GitHub Pages sites, unless you're using a custom GitHub Actions workflow. 

4. Git Large File Storage (LFS)
If you need to include files larger than the standard limits in your repository, you can use Git LFS.
Git LFS stores references to large files in your repository, while the actual files are stored elsewhere.
With Git LFS, the maximum file size depends on your GitHub plan:
2 GB for Free and Pro accounts.
4 GB for GitHub Team.
5 GB for GitHub Enterprise Cloud.
Important: New files will be rejected silently if you exceed your LFS storage quota.
You get 1 GB of free LFS storage and 1 GB of free bandwidth per month. You can purchase more if needed.

5. Other considerations
Git is designed for version control of code, not for storing large binary files or serving as a backup solution.
Consider using GitHub Releases for distributing very large files, such as binaries or datasets. Individual files in a release can be up to 2 GB, and there's no limit on the total size or bandwidth for the release itself.
For external dependencies, use a package manager (like npm, Maven, etc.) instead of committing the dependencies directly to the repository to keep it smaller.
Optimize images and other assets using compression to reduce your repository size and improve website performance.

"
