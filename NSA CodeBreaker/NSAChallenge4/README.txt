B2:
Looked at the header and saw that there was a had a x-git-commit-hash. Did some google searches and found these articles about it. 
https://towardsdatascience.com/understanding-the-fundamentals-of-git-25b5b7ded3c4
https://wildlyinaccurate.com/a-hackers-guide-to-git/

From these I understood how to access the git directory for the website through the URL. 
Had to go through the git directories multiple times. The way I did this is first by making a git repository then inside that
I downloaded the git commit history through curl command and opened it using git commands in my terminal. Then used the git 
tree file name to download that and go deeper in by repeating the lookup in my git terminal and looking at git tree files and
getting the next one. I found the server python file and analyzed the code. Noticed that they added a weird string before the 
requested login page. After doing that I was able to reach the login page.

Flag: https://vktwkoeclxtsqtcj.ransommethis.net/ngovaralpzwqezxt/login