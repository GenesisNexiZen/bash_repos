# git_repos

what are bash commands?

$ ex                              #bash command to run the "ex" program.
: i                               #ex command to "insert" some text.
Hello!
.                                 #A line with just a dot tells ex to stop inserting text.
: w greeting.txt                  #ex command to "write" the text to a file.
"greeting.txt" [New] 1L, 7C written
: q                               #ex command to "quit" the program.
$ cat greeting.txt                #And now we're back in bash!
Hello!                            #The "cat" program shows the contents of the file.
$ 

#How do I give bash a command?

 read -p "Your name? " name       #This command is complete and can be started immediately.
Your name? Maarten Billemont
$ if [[ $name = $USER ]];         #thenThe "if" block started but wasn't finished.
>     echo "Hello, me."
> else
>     echo "Hello, $name."
> fi                              #Now the "if" block ends and bash knows enough to start the command.
Hello, Maarten Billemont.

