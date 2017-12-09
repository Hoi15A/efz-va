# efz-va
Document and presentation files related to my Vertiefungsarbeit (required paper for Eidgenössisches Fähigkeitszeugnis).

## Structure
This project consists of two main parts, the [written paper](https://github.com/fuerbringer/efz-va/tree/master/documents) and the [presentation](https://github.com/fuerbringer/efz-va/tree/master/presentations/compiled). The presentation can be exported into any format as long as pandoc supports it.

## Building the presentation
Clone this repo recursively to build the presentation files: `git clone --recursive https://github.com/fuerbringer/efz-va.git`. Then enter the `presentations` directory and run `make`.

### Requirements
#### Environment
Building the presentation files requires a unix-like environment.

#### Packages
It's assumed that the following packages are present in the global scope:
- `pandoc` (full suite)
- `texlive`
- `GNU Make` or similar
