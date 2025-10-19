# OPAC Book Cataloging Fails When Creating New Catalog Entry

This page described how to resolve an issue that come up when the insert.php filr in the simple OPAC application is not found. When this issue occurs, attempting to add a new book on the page "cataloging/index.html" will not result in a "Not Found" pafe being shown when the "Submit button is pressed. 

![image description](./images/.5.png)

The root of the issue is the file "cataloging/insert.php" is not present. You can verify that you are experiencing this issue by reading the URL bar. If it ends in "cataloging/insert.php" as depicted, and you are getting the "Not Found" error page shown above, this pagee can help you. If not, you are most likely to be encountering another issue.

The problem is resolved by ensuring that the file "cataloging/index.php has the appropriate name as well as contents. To start correcting this error, navigate to the folder containing your cataloging pages. 

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
