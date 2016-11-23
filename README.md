#pdf2audio
A tool to convert PDF files to audio files.

##Prerequisites:
- Vim
- Unix machine (less)
- eSpeak

##Instructions
- Make a text out of your PDF.
```
$ less file.pdf > file.txt
```

- Enter Vim, and spread some macro-magic!
```
$ vi file.pdf
```
- Macro:
```
qavipJ$2jq
```
- Having stored the macro successfully in a, run
```
10000@a
```
to audiofy the file!
- Use espeak voices to read out the book to you.
```
cat file.txt | espeak -v ta -w out.wav
```

##TODO:
- Add chapterwise chunking
- Get an ESpeak Voice File that sounds less Dalek-like
