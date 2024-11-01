# notebook-generator


(Auto) generate notebooks from your source code. Useful for ACM-ICPC. 

## Installation

You need texlive and node installed in your device. so check how to install texlive and node in your OS. 

#### Download Texlive 
texlive for Linux or WSL:

```
apt install texlive texlive-latex-extra
```
texlive for Windows:

download installer (install-tl-Windows.exe) from https://www.tug.org/texlive/acquire-netinstall.html

#### Clone Repository

Clone this repository in your device
```
https://github.com/BUET-IUPC/notebook-generator.git
```

#### Download npm dependencies

Download npm dependencies
```
cd notebook-generator
npm i
```

## Use

    Usage: notebook-generator <source_dir> [options]

    Auto generate notebooks from your source code

    Options:
        -V, --version             output the version number
        -a --author <name>        author's name to be added in the notebook
        -o --output <filename>    output file for the notebook. (default: "./notebook.pdf")
        -s --size <size>          font size is allowed 8, 9, 10, 11, 12, 14, 17, 20 pt (default: "10")
        -c --columns <amount>     number of columns is allowed 2, 3. (default: "2")
        -p --paper <size>         paper size is allowed letterpaper, a4paper, a5paper. (default: "letterpaper")
        -h, --help                output usage information


example:
```
/<path to bin>/notebook-generator ./ --output /tmp/team_reference.pdf
```
Preffered command for IUPC with acceptable presentation is
```
/<path to bin>/notebook-generator ./ --author "Your Team Name" --size 11 --columns 3 --paper a4paper 
```
You can probably be safe with font size 10 too. However, you probably shouldn't go lower than that. 

## Example PDF

Here you can find an example https://github.com/pin3da/Programming-contest/blob/master/codes/notebook.pdf

## Files

The notebook generator will add your source code with syntax highlight, additionally
you can add .tex files which will be rendered as latex code.

## Notes:

- Try to use up to 3 "levels" in your source code.
- Use spaces insead of underscore (in the filenames) to print a prettier TOC.

----
Original Author: [Manuel Pineda](https://github.com/pin3da/) & [Diego Restrepo](https://github.com/Diegores14)

Modification: [Pritom Kundu](https://github.com/Anachor)

