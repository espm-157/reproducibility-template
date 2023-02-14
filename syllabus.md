




# reproducibility tutorial :onion: 

Reproducible workflows are like onions :onion: :cry: :smiling_face_with_tear: :joy:. 

Reproduciblity comes in layers!

- Scripts
- Packages
- Containers


- Reproducibility is about robust, user friendly, and widely practiced standards.
- This tutorial is about robust, easy, widely-practiced, well automated standards. 
- Novelty and creativity are the enemy here. If it feels desperate it probably is. Bridges, not art. to be "trivial" is the highest possible praise.

## GitHub: Sharing Code



## Scripts

- Write code, share code.
- [Project-oriented workflows](https://www.tidyverse.org/blog/2017/12/workflow-vs-script/):
  - no `setwd()` / no `rm(list=ls())`
  - Clean starts, good organization, common practices. `usethis`.  (Rstudio users: `usethis::use_blank_slate()`)

- Reproducibility founders most often on externality


###  code & software dependencies.  
  - Be organized. (KISS, functions, `R/`)  
  - Be explicit. (`library()`. `DESCRIPTION`). 
  - be pedantic (`renv`)
  
### data dependencies & paths
  - keep your data with code and use relative paths.
  
  
Advanced cases: distributing complex code and large/complex data sets

  - If you're writing hundreds of lines of code / managing dozens of files, you have a _software_ project. 

There's a lot of advice about how to manage/organize large 'workflows', mostly in the realm of desperate hacks/shortcuts (i.e. bad software).
If you want this to go well, be reproducible, robust, etc, it needs to be written following software best practices: unit tests, documentation, modular design, the whole nine yards. It's not hard, what to do is very explicitly laid out, examples are plentiful, as are automated tooling to help, but it is still time consuming. You can follow as much or as little of the best practices for software development as you like, not everything needs to be professional developer quality, but if you can't be bothered to follow these practices, have lower expectations about the reproducibility, robustness, portability, re-usability, etc. Often a project is best distributed by dividing into smaller components.  Perhaps you make some of these robust. reusable elements, and just let other elements be messy. Just don't believe in the free lunch hype.


- If you have large custom data files that don't fit on GitHub / etc, you have a _data product_.
Again, the best practices of the field are relevant here. FAIR repositories, identifier based access, appropriate citations. Scale-based solutions download-free / cloud-native workflows.

(you can also have a software product or a data product that involves only small quantities.  However, such projects are more forgiving)


## GitHub Actions

Seeing if work is reproducible. 

## R Package Basics

Leveling up: From Project to Package

## Codespaces: portable compute environments

## Containers

- The Dockerfile, system dependencies, limitations.

## Archiving

- Zenodo DOIs. Alternatives

## Portability & Scale

- Identifiers. content-based identifiers.
- Data repositories
- 

