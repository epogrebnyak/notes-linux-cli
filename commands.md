[GNU Coreutils](https://ru.wikipedia.org/wiki/GNU_Coreutils)
============================================================

| Area                          | Familiar             | Not familiar                               |
| ----------------------------- | -------------------- | ------------------------------------------ |
| Output of entire files        | cat                  | tac nl od base32 base64                    |
| Formatting file contents      |                      | fmt pr fold                                |
| Output of parts of files      |                      | head tail split csplit                     |
| Summarizing files             |                      | wc sum cksum b2sum md5sum sha1sum sha2     |
| Operating on sorted files     |                      | sort shuf uniq comm ptx tsort              |
| Operating on fields           |                      | cut paste join                             |
| Operating on characters       |                      | tr expand unexpand                         |
| Directory listing             | ls dir               | vdir dircolors                             |
| Basic operations              | cp mv rm             | dd install  shred                          |
| Special file types            | mkdir rmdir unlink   | mkfifo mknod ln link readlink              |
| Changing file attributes      | chmod touch          | chgrp chown                                |
| Disk usage                    |                      | df du stat sync truncate                   |
| Printing text                 | echo                 | printf yes                                 |
| Conditions                    |                      | false true test expr                       |
| Redirection                   |                      | tee                                        |
| File name manipulation        |                      | dirname basename pathchk mktemp realpath   |
| Working context               | pwd                  | stty printenv tty                          |
| User information              | whoami               | id logname whoami groups users who         |
| System context                | date                 | arch nproc uname hostname hostid uptime    |
| SELinux context               |                      | chcon runcon                               |
| Modified command invocation   |                      | chroot env nice nohup stdbuf timeout       |
| Process control               |                      | kill                                       |
| Delaying                      | sleep                |                                            |
| Numeric operations            |                      | factor numfmt seq                          |




[Unix command-line interface programs and shell builtins](https://en.wikipedia.org/wiki/Util-linux)
===================================================================================================

| Area              | Commands       |                                                                                                                           
|-------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| File system       | **cat chmod** chown chgrp cksum cmp **cp** dd **du** df file fuser ln **ls mkdir mv** pax **pwd rm rmdir** split tee **touch** type umask |
| Processes         | at bg crontab fg kill nice ps time                                                                                                        |
| User environment  | env **exit** logname mesg talk tput uname who write                                                                                       |
| Text processing   | awk basename comm csplit cut diff dirname ed ex fold head iconv join m4 **more** nl paste printf sed sort strings tail tr uniq vi wc args |
| Shell builtins    | alias **cd echo** test unset wait                                                                                                         |
| Searching         | **find** grep                                                                                                                             |
| Documentation     | **man**                                                                                                                                   |
| Software development   | ar ctags lex **make** nm strip yacc                                                                                                  |
| Miscellaneous     | bc cal expr lp od sleep true and false                                                                                                    |
