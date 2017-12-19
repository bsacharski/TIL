## Git for multiplatform projects

### Keeping EOL for text files intact
You should decide on one EOL variant for text files. We've noticed that scripts, that were written
on linux, got their line endings replaced from LF to CRLF in Windows - cygwin didn't really like that.
You could force it by adding file `.gitattributes` file to repo:
```
* text=auto eol=lf
```

That should do the trick 😊 
