# BioHackrXiv Publication Template

Minimal example of a [BioHackrXiv](https://biohackrxiv.org/) publication that can be generated with the
[Preview Service](http://preview.biohackrxiv.org/).


## Step 1: Configuring the Markdown

The publication Markdown is found in the `paper/paper.md` file. At the top you can edit the
YAML code with metadata. It is important to get this part correct, because otherwise the PDF
generation will fail. The metadata looks like this:

```yaml
title: 'BioHackEuro SWAT2025 Barcelona Report for Project 6: Automatic Ontology Mapping with LLMS'
title_short: 'BioHackEU25 #6: Auto Ontology Mapping with AI'
tags:
  - ontology mapping
  - SSSOM
  - AI
authors:
   - name: Mark Doerr
    orcid: 0000-0003-3270-6895
    affiliation: 1
affiliations:
  - name: Dept of Biotechnology and Enzyme Catalysis,Inst. f. Biochemistry, University Greifswald, DE
    index: 1
date: 27 February 2025
cito-bibliography: paper.bib
event: BH22EU
biohackathon_name: "BioHackathon Europe 2025"
biohackathon_url:   "https://biohackathon-europe.org/"
biohackathon_location: "Barcelona, Spain, 2025"
group: ontology mapping group
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/biohackrxiv/publication-template
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Mark Doerr \emph{et al.}
```

### Which metadata to update?

#### To change

The following fields should be changed:

* title
* title_short
* tags
* authors (name and optionally their ORCID identifier)
* affiliations
* date
* group
* authors_short

Particularly important to update is the following field, which should point to
your clone of the template, instead of the template itself:

* git_url: https://github.com/biohackrxiv/publication-template

#### Only update for other BioHackathons

The following fields should only be changed if you are not writing for the BioHackathon Europe 2022:

* event: BH22EU
* biohackathon_name: "BioHackathon Europe 2022"
* biohackathon_url:   "https://biohackathon-europe.org/"
* biohackathon_location: "Paris, France, 2022"

## Step 2: Writing the article

A full Markdown example is given in [paper/paper.md](paper/paper.md). This includes instructions how to include
figures, tables, and annotate citations with the Citation Typing Ontology.

## Step 3: Previewing the paper as PDF

This repository can be converted into a preview PDF with BioHackrXiv [Preview Server](http://preview.biohackrxiv.org/).
The preview website asks for the link to your repository and will automatically find the `paper.md` and create an PDF.

