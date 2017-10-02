# Notes
Notes is a simple note-taking software for the command line.

## Dependencies

- [grip](https://github.com/joeyespo/grip) - if you want to be able to view your notes as an html page
- vim (if you want to use a lesser editor then fork and make your own)

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

## Usage
The usage is simple:
```
# open the notes.md file in vim
$ note

# create a new subheading at the end of your notes file and reads from stdout, 
# appending to notes file when you CTRL-C
$ note some heading title

# open the notes file and puts cursor on first occurrance of the search you gave it
$ notes some search text

# run grip on notes and opens in browser
$ notes

# push your notes to the your git repo
# will create a generic commit and push it to your fork
$ notes push

# pull your notes from your fork for easy sharing across any computers you use
$ notes pull
```

## Note On Private Repos
If you want your notes in a private repo (probably not a bad idea), you can't fork. You'll have to make a copy of the repo.
