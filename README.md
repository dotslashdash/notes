# notes

This note taking system is designed to keep friction low. That means not
worrying about file types, formatting, tagging, check boxes, syntax rules, and
anything else that might distract or slow you down. The goal is to get it out
of your head and into a document.

## Advantages
- You can use `grep`, etc. to search through it later
- Consumes very little disk space
- Easy to backup & sync

I use it as a scattered brain dump in which anything can be found via grep in a
few seconds.

## Notes are organized by auto-dated monthly files

For example, on January 1st, 2023 if you run `notes My first note` it will
create a file `2023-01.txt` in your `NOTES_DIRECTORY`. `My first note` gets
appended to the file.

## Installation
Copy & paste the line below:
```
sudo curl \
  -L https://raw.githubusercontent.com/dotslashdash/notes/master/notes \
  -o /usr/local/bin/notes && sudo chmod +x /usr/local/bin/notes
```

## Usage examples

- `notes something you want to jot down`
  - Appends whatever arguments you add as text into the dated file
- `pbpaste | notes`
  - Pipes and appends anything in your clipboard
- `notes`
  - Opens the dated file in your configured `EDITOR`
