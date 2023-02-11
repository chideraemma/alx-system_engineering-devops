Shell permissions:

To have a clear understanding of what each script dose use this reference below 

The numbers here represent each letter and it is meant to be Added + Absolute Method read - r - 4, write - w - 2, execute - x - 1

rwx rwx rwx = 111 111 111
rw- rw- rw- = 110 110 110
rwx --- --- = 111 000 000

and so on...

rwx = 111 in binary = 7
rw- = 110 in binary = 6
r-x = 101 in binary = 5
r-- = 100 in binary = 4

0. "su" meanings "substitute user" it gives us privileges to become a superuser, it is often necessary to become the superuser to perform important system administration tasks, but we should not stay logged in as the superuser.

1.  To print the effective username of the current user, you can use "whoami" it shows you who you are at s parent directory.

2. "groups" It is used to prints all the groups the current user is part of.

3. "sudo chown" It is used to changes the owner of the file.

4. "touch" It is used to creates an empty file.

5. "chmod u+x" It is used to Write a script that adds execute permission to the owner of the file hello.

6. "chmod u+x,g+x,o+r" It is used to Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

7. "chmod ugo+x" It is used to Write a script that adds execution permission to the owner, the group owner and the other users, to the file  hello.

8. "chmod 007" It is used to Write a script that sets the permission to the file hello as follows:

    Owner: no permission at all
    Group: no permission at all
    Other users: all the permissions

9. "chmod 753" It is used to Write a script that sets the mode of the file hello:

10. "chmod --reference=olleh hello"  It is used to Write a script that sets the mode of the file hello the same as olleh’s mode.

11. "chmod -R +111 */" It is used to Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.

12. "mkdir -m 751 my_dir" It is used to Create a script that creates a directory called my_dir with permissions 751 in the working directory.

13. "chgrp school hello" It is used to Write a script that changes the group owner to school for the file hello.

14. "chown vincent:staff *" It is used to Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

15. "chown -h vincent:staff _hello" It is used to Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.

16. "
