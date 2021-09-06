# SDLC
SDLC Definition
Software Development Life Cycle a frame-work that process used of software industry to planning, design, develop, test and deploy.
##
# LAMP Stack: 
This stand for Linux, Apache, Mysql, PHP. Together they provide a proven set of software for delivering high-performance web applications. Each component contribute essential capabilities.
##
# Chmod and Chown commands in linux
Both are file permission.
#Chown is use to change the ownership of a file or folder.
. Give the members of the group permission to read the file, but not to write and execute it:
(chmod g=r filename)
. To Remove the execute permission for all users:
(chmod a-x filename)
. Recursively remove the write permission for other users:
(chmod -R o-w dirname)
. Remove the read, write, and execute permission for all users except the file’s owner:
(chmod og-rwx filename)
. The same thing can be also accomplished by using the following form:
(chmod og= filename)
. Give read, write and execute permission to the file’s owner, read permissions to the file’s group and no permissions to all other users:
(chmod u=rwx,g=r,o= filename)
. Add the file’s owner permissions to the permissions that the members of the file’s group have:
(chmod g+u filename)
. Add a sticky bit to a given directory:
(chmod o+t dirname)
##
#Each write, read, and execute permissions have the following number value:

    r (read) = 4
    w (write) = 2
    x (execute) = 1
    no permissions = 0
    
The permissions number of a specific user class is represented by the sum of the values of the permissions for that group.
To find out the file’s permissions in numeric mode simply calculate the totals for all users classes. For example, to give read, write and execute permission to the file’s owner, read and execute permissions to the file’s group and only read permissions to all other users you would do the following:

    Owner: rwx=4+2+1=7
    Group: r-x=4+0+1=5
    Others: r-x=4+0+0=4
