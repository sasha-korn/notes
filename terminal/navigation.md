# Terminal

## Navigation

- `pwd`: shows the current path/location 
```
$ pwd
/Users/alexkorniichuk/Documents/notes/terminal
```
- `ls`: shows files and directories (folders) in the current path
```
$ ls
1021-613.jpg
95905cc73a1c0b9ae5de234ea20e27d1.png
A Folder
Certificado_OLEKSANDRA.pdf
English vocab
Gmail - Coach Ticket Confirmation.pdf
```
- `ls -la`: shows permissions and hidden files/directories (which starts with .)
```
total 0
drwxr-xr-x@ 4 alexkorniichuk  staff  128 Apr 17 22:46 .
drwx------@ 6 alexkorniichuk  staff  192 Apr 17 22:46 ..
drwxr-xr-x@ 9 alexkorniichuk  staff  288 Apr 17 21:16 .git
drwxr-xr-x@ 3 alexkorniichuk  staff   96 Apr 17 22:46 terminal
```
- `cd` : to enter/exit the directory
```
➜  notes git:(main) $ ls
terminal
➜  notes git:(main) $ cd terminal
➜  terminal git:(main) $
```
- `cd ..`: to go back for 1 level; cd ../../ goes for 2 lvl back etc
```
➜  terminal git:(main) $ pwd  
/Users/alexkorniichuk/Documents/notes/terminal
➜  terminal git:(main) $ cd ..    
➜  notes git:(main) $ pwd
/Users/alexkorniichuk/Documents/notes
```
- `mkdir $dirName` : creates new directory named $dirName
```
➜  notes git:(main) $ ls
terminal
➜  notes git:(main) $ mkdir maru
➜  notes git:(main) $ ls
maru     terminal
```
- `touch $fileName` : creates new file named $fileName
```
➜  maru git:(main) $ touch maru.txt
➜  maru git:(main) $ ls
maru.txt
```
- `cat $fileName` : shows content of the file 
-  `echo $text > $fileName` : creates/rewrites $text to the $fileName
```
➜  maru git:(main) $ cat maru.txt 
➜  maru git:(main) $ echo mew > maru.txt 
➜  maru git:(main) $ cat maru.txt       
mew
```
- `echo $text >> $fileName` : adds $text to the $fileMame
```
➜  maru git:(main) $ cat maru.txt 
mew
➜  maru git:(main) $ echo mew2 >> maru.txt 
➜  maru git:(main) $ echo bow >> maru.txt 
➜  maru git:(main) $ cat maru.txt 
mew
mew2
bow
```
- `cat $fileName | grep $searchSelection` : shows lines in $fileName containing $searchSelection
```
➜  maru git:(main) $ cat maru.txt 
mew
mew2
bow
➜  maru git:(main) $ cat maru.txt | grep mew
mew
mew2
```
- `man $commandName` : $commandName description (to exit press $q)
- `rm $fileName` : deletes (forever!) $fileName
- `rm -r $directoryName` : deletes (forever!) $directoryName and its contents
- `mv $fileNameOld $fileNameNew` : renames/moves
```
➜  terminal git:(main) $ ls
terminal.md
➜  terminal git:(main) $ mv terminal.md navigation.md
➜  terminal git:(main) $ ls
navigation.md
```
- `history` : shows commands history