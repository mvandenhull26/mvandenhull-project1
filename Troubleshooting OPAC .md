# OPAC Book Cataloging Fails When Creating New Catalog Entry

Upon entering a new book into my cataloging website, instead of the book being entered, an error of "Not Found - The requested URL was not found on this server" presented itself. 

![image description](./images/1.png)

From here, I navigated to my website folder using "cd-mvandenhull-project1"

![image description](./images/2.png)

Then I used "ls" to find what I had in the system. 

![image description](./images/3.png)

Next, I went into "ls /var/www/html"

![image description](./images/4.png)

And then ran "cd /var/www/html"

![image description](./images/5.png)

I ran "ls" agian to see what my options were once again.

![image description](./images/6.png)

Then what the issue I discovered that I accidentally named a file as "instert" instead of "insert". Silly me and my silly goofy typos causing issues.

![image description](./images/7.png)

I realized I needed to move the folder, so I ran "mv cataloging/instert.php cataloging/insert.php" so my typo folder would be redirected into the correct folder. 

![image description](./images/8.png)

It didn't work right, and I realized I needed "sudo" in front of my command line, so I then ran "sudo mv cataloging/instert.php cataloging/insert.php"

![image description](./images/9.png)

After all of this, my cataloging part of the website started to work! I then entered several books, and was very happy. 
