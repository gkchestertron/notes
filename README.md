# Notes
Notes is a simple note-taking software for the command line.

## Dependencies

- [grip](https://github.com/joeyespo/grip) - if you want to be able to view your notes as an html page
- vim (if you want to use a lesser editor then fork and make your own)
- git

## Installation
First, fork this repo, and clone to your home folder:
```
cd ~
git clone https://github.com/<your_username>/notes.git
```
Then source the script in your ~/.bashrc or ~/.bash\_profile
```
source ~/notes/notes
```

## Mac and Linux Users
This should just work. Seriously, if you don't have git and vim, I can't help you.

## Windows Users
As usual, you're on your own.

## Usage
The usage is simple:
```
# create a note
$ notes create some_name

# destroy a note
$ notes destroy some_name

# append to default notes from stdout (press CTRL-C to finish - and make sure to make a new line, or it won't write)
$ note

# appending to a specific note file from stdout
$ note some_name

# open a specific note file in vim
$ notes some_name

# open the the notefiles folder in vim so you can select a notefile to work in
$ notes

# serve default note file with grip and open in browser
$ notes serve

# serve specific note file with grip and open in browser
$ notes serve some_name

# push your notes to the your git repo
# will create a generic commit and push it to your fork
$ notes push

# pull your notes from your fork for easy sharing across any computers you use
$ notes pull
```

## Keeping up to date
While there are push and pull methods available, notes will automatically try to push and pull every time you open/close them

## Note on Using Private Repos
If you want your notes in a private repo (probably not a bad idea), you can't fork. You'll have to make a manual copy of the repo. Be my guest.
