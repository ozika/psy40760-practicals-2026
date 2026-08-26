# PSY40760 — Advanced Data Analysis and Statistics in R (2026/27)

Weekly practical materials for PSY40760, MSc Behavioural Neuroscience, UCD. Each week has its own R Markdown notebook you'll work through in RStudio during the practical session.

This repo does **not** contain the take-home exam — that's released separately, on its own repo, at the start of the exam window.

## Getting started (do this once, before Week 2)

1. **Install R and RStudio.** See the "General Setup" section on Brightspace for step-by-step instructions.
2. **Install Git and set up SSH keys**, if you haven't already — also covered in the Brightspace General Setup section.
3. **Clone this repository:**
   ```
   git clone git@github.com:ozika/psy40760-practicals-2026.git
   ```
4. **Open the project** by double-clicking `psy40760-practicals-2026.Rproj` — always open the `.Rproj` file first, not an individual `.Rmd`, so your working directory is set correctly.
5. **Restore the package environment:**
   ```r
   renv::restore()
   ```
   This installs the exact package versions the course uses, into an isolated project library, without touching anything else on your machine.

## Getting each week's update

New weeks are added to this repo as the trimester progresses. Before each practical:

```
git pull
```

from inside the project folder. If `renv.lock` has changed (i.e. new packages were added for that week), run `renv::restore()` again afterwards.

## Structure

```
psy40760-practicals-2026/
├── psy40760-practicals-2026.Rproj   <- open this first
├── renv.lock                          <- exact package versions for the course
└── weeks/
    ├── week02-r-basics/
    │   ├── week02_practical.Rmd       <- work through this in the practical
    │   └── data/
    └── ...                             <- added week by week
```

Each week folder contains the student notebook and any data files it needs. Solutions notebooks (`*_SOLUTIONS.Rmd`) are for instructor/TA use.

## Problems?

Bring it to the practical session — Cameron is there to help. If it's a "my R won't even open the project" problem, check the General Setup section on Brightspace first.
