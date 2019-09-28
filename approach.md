# how it works

this program has three parts.  
one for generating passwords and logins,  
one for storing them  
and one for restoring them.

you can read more details about each.

## password and login generator

one for generating random passwords and logins.  
since some sites have you to use passwords in a special type  
(like containing numbers but no spaces), this program will be  
able to make passwords in any format you have it.

## password and login storer

after login and password generated, we need to store them.  
this has to be in an encrypted way to make piracy less effective.

this will store (site address + login + password + your notes)  
for each site in a seperate file so appending will be easy.

also a strong user password is needed for secure encryption.  
something long, unguessable and easy to remember.  
for more info and help for generating such keys see this repo:  
[python password gemerator](https://github.com/ekm507/python-password-generator "ekm507/python-password-generator")

## data restorer

to restore password for a site we need user's master password  
and also we need to locate the file in which password to  
this site is stored.

since we don't want to decrypt everything to find a password,  
we are going to save hash codes for site names in a file which  
tells us which file should be decrypted.

also for more security, we do some process on site address  
before hashing. (hell I can't recall what was that process called)
