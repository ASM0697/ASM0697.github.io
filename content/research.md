---
title: 'Research'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`
sections:
  - block: collection
    content:
      title: Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  
  - block: collection
    content:
      title: Under Review
      text: ''
      filters:
        folders:
          - pubunderreview
        exclude_featured: false
    design:
      view: citation

  - block: markdown
    content:
      title: Poster Presentation
      text: |
          * Participated in the design and presentation of a scientific poster titled **‘C.A.S.E. Study: Engineered Stem Cells Combating Cancer’**, focusing on the therapeutic potential of reprogramming patient-derived stem cells to targetcancer at the [City of Scientific Research and Technological Applications](https://srtacity.sci.eg/) (SRTA City) in July 2019.
      
      #filters:
       # folders:
        #  - ???
        #exclude_featured: false
    #design:
     # view: citation
  - block: markdown
    content:
      title: Peer Review
      text: |
        * Contributed to the peer-review process of [**Journal of Molecular Histology**](https://link.springer.com/journal/10735) as an invited reviewer in July 2026.

        * Contributed to the peer-review process of [**Open Veterinary Journal**](https://www.scimagojr.com/journalsearch.php?q=21100438194&tip=sid) as an invited reviewer in November 2025.
      
      #filters:
        #folders:
          #- peerreview
        #exclude_featured: false
    #design:
      #view: citation
  - block: markdown
    content:
      title: Internships
      text: |
          * I completed two research internships for one month at [SRTA City](https://srtacity.sci.eg/) in Egypt, where I gained hands-on experience with molecular and tissue culture techniques.
          
          * I completed a research internship for over three months at [Egypt Scholars Labs](https://egyptscholars.org/es-labs2/), where I learned the practical application of research skills, including producing and publishing scientific articles.
      
      #filters:
       # folders:
        #  - ???
        #exclude_featured: false
    #design:
     # view: citation
---
