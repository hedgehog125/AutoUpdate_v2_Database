## Launching a new version

To launch a new version first open database/Versions.txt

add the new version to the list.

E.g...

Add ",2.2" to the end.

Then make sure your database is set to your clone.

E.g:

https://raw.githubusercontent.com/hedgehog125/Auto-Update-Database/master/

Next, add in to the dictionary "Files.txt" your new version in quotes.

E.g:

{"1.0":[]}


# Next you need to add the files...


If you want a file specify True e.g:

{"1.0":[[True,]]}

Or if you want a directory:

{"1.0":[[False,]]}

If you chose file:
-   The next argument is the filename. {"1.0":[[True,"A file.txt"]]}
-   Then the next is file contents/url  {"1.0":[[True,"A file.txt","Some text..."]]} or 
-   {"1.0":[[True,"A file.txt",", "https://avatars0.githubusercontent.com/u/16543008?v=3&s=460"]]}

-   And the final argument is if you specified url (True) or contents (False).

-   {"1.0":[[True,"A file.txt",", "https://avatars0.githubusercontent.com/u/16543008?v=3&s=460",True]]}

-   In most cases you will want to use the above. 

-   But with very small files you might want to use:

-   {"1.0":[[True,"A file.txt",", "Some text...",False]]}



If you chose dir:
-   The last argument is directory name. {"1.0":[[False,"A dir"]]}







So here are the templates:

File with text:
-   {"1.0":[[True,"A file.txt",", "Some text...",False]]}

File from url:
-   {"1.0":[[True,"A file.txt", "https://avatars0.githubusercontent.com/u/16543008?v=3&s=460 ",True]]}

I put a space in the url so the link doesn't include the quotes.

You should remove it.

Dir:
-   {"1.0":[[False,"A dir"]]}


Hope this helps! :D
