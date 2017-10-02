# Notes
Notes is a simple note-taking software for the command line.

## Dependencies

- [grip](https://github.com/joeyespo/grip) - if you want to be able to view your notes as an html page

## Installation
To install clone this repo into your home folder (or wherever you want - just replace ~ with your path if you do).
```
cd ~
git clone https://github.com/gkchestertron/notes.git
```
Then source the script in your ~/.bashrc or ~/.bash\_profile
```
source ~/notes/notes
```

## Usage
The usage is simple:
```
# opens the notes.md file in vim
$ note

# creates a new subheading at the end of your notes file and reads from stdout, 
# appending to notes file when you CTRL-C
$ note some heading title

# opens the notes file and puts cursor on first occurrance of the search you gave it
$ notes some search text

# runs grip on notes and opens in browser
$ notes
