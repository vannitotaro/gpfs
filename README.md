# Google Plus Follower Stats (gpfs) #

Copyright 2012 Giovanni Totaro (http://www.ingtotaro.it)

License: MIT (http://www.opensource.org/licenses/MIT)
 
Google+: https://plus.google.com/u/0/113250814961864918365/about

Twitter: https://twitter.com/vannitotaro

Official gpfs source code repository: https://github.com/vannitotaro/gpfs


## INTRO ##
**Who Are Your Most Influential G+ Followers?**
Probably you don't know the answer.
Maybe you are not following back someone with 100.000 or more followers... BAD!

This is a tiny dirty script that gives you a clickable list of people
who have you in their circles, ordered by how many people have them
in their circles in descending order...
i.e. you get **your followers sorted from most to least followed one**.
Nice, isn't it?

## DISCLAIMER ##
I am not affiliated with Google and Google does not endorse this software.

## NOTES ##
- This script does not make use of official Google APIs, so it can stop working
  if Google makes changes to the Google+ implementation.
- This script has been tested only under Ubuntu 12.04 32-bit.
- You need to install `curl` before running the script:
  `sudo apt-get install curl`

## USAGE ##
1. Open your web browser (tested under Chrome and Firefox)
2. Sign in to your Google Plus account
3. Visit the URL:
   https://plus.google.com/u/0/_/socialgraph/lookup/followers/?m=1000000
4. Save the response as a file named `response.txt`
5. Move `response.txt` into the directory where you put the script file `gpfs`
6. Run `./gpfs` (without parameters) in a terminal and wait its end
   (~2 minutes per 100 followers during my tests: yes, a lot of time...)
7. Your default web browser should now automatically open `gpfs.html`,
   a file just created into the same directory of the script
