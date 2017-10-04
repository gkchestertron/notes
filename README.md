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
Alternatively you could copy the notes script to someplace in your path:
```
$ cp notes /usr/local/bin/
```
or symlink it:
```
ln -s $(pwd)/notes /usr/local/bin/notes
```

## Mac and Linux Users
This should just work. Seriously, if you don't have git and vim, I can't help you.

## Windows Users
As usual, you're on your own.

## Usage
The usage is simple:
```
# append to notes from stdout
$ note

# create a new subheading at the end of your notes file and reads from stdout, 
# appending to notes file when you CTRL-C
$ note some heading title

# open the notes file and puts cursor on first occurrance of the search you gave it
$ notes some search text

# open notes at the end of the file
$ notes

# push your notes to the your git repo
# will create a generic commit and push it to your fork
$ notes push

# pull your notes from your fork for easy sharing across any computers you use
$ notes pull

# serve notes with grip and open in browser
$ notes serve
```

## Note on Using Private Repos
If you want your notes in a private repo (probably not a bad idea), you can't fork. You'll have to make a manual copy of the repo. Be my guest.
