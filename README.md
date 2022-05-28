# Intro
The code here is pretty much everything I use to create my datasets (from FBRef) or visuals. Most my scatter plots are made in Tableau, though, using the dataset created from the FBRef dataset download.

Feel free to download any of this code and use it yourself, it's on the MIT license. No need to give attribution to me, but any credit or even a tag (@BeGriffis on twitter) is much appreciated! And I'd love to see the work you do with this code, of course!

# Installing Jupyter Notebook
All of this code is written in Python but using Jupyter Notebook. Jupyter Notebook is free and safe, and easy, to install. If you don't have it on your computer yet, there are several ways to get it; I'll give two examples below.

### Project Jupyter
One method is by downloading direct from Project Jupyter: https://jupyter.org/install

Follow the short instructions there to download. You can download and start coding in seconds.

### Anaconda
Another way to get Jupyter Notebook is to install it via Anaconda, which acts as an environment to host much of your coding needs: https://www.anaconda.com/products/distribution

This method is what I use, however there are a couple extra steps to begin working in Jupyter Notebook. But, it is still easy to follow and Anaconda gives good instructions.

# Running These Code Files: No Major Coding Experience Needed!

Once you have Jupyter Notebook, you can begin running these code files.

Download the files from this repository and open them with Jupyter Notebook. The instructions should hopefully be straight forward for all files.

The 1st code file to run is the "Download Top 5 Leagues csv from FBRef .com", as the 2 datasets it creates act as the raw data for the majority of the other files. To run that code, all you need to do is click "Run" in the top bar in Jupyter Notebook. It's that simple!

After you have run that file, you can then start making your own scouting cards and passing style charts.

### Scouting Cards & Passing Style Programs

To create your own reports, you'll need to click in the second block of code (each block has a grey background) and Run that. Then, scroll back to the first block and edit the information. I added notes (after the # in each line) explaining (hopefully easiily) what to do.

Once you've entered your player's info, click Run (or press ctrl+enter on your keyboard) and voilà, there's your image!

### Distribution Charts

To create a distribution chart of a specific metric, you'll follow a similar process to the scouting cards and pass style programs.

Simply scroll to the "enter desired info here" section (it's all one block of code this time)) and enter the required information. Then run the code and Presto, a distribution chart hot off the press.

### Ternary Charts

This program will involve a few tweaks to the code if you want to change what variables are included. However, I have put notes in the code at the places you would need to change anything. The variable names are the same as the column names in the csv file from the FBRef download, so you can open that to find the specific variable names. The variable names are also hardly changed from FBRef.com, so you can look there as well. Per 90 stats just have 'Per90' at the end.

First, change the DPI (defaults at 300) if you want to. I use 300 dpi for getting everything how I want it, and then once at 2000 dpi that I save to post on Twitter. Then make sure to click on the 'Kernal' menu at the top, and then 'Restart & Clear Output' before closing Jupyter Notebook, because otherwise you'll store a huge image file!

Next, change the desired info under the "set your variables here" section. Finally, if you want to change any of the metrics that comprise one of the stats in the corners, scroll a little further and adjust that where it says "change anything here".

Please contact me if you want to change anything but are lost or get stuck!

## Running the Match Log Download program

Downloading the match logs for a certain league takes a little more effort, but no extra coding effort! First, run the first block of code. Then, scroll to the section for the league you want to download. Each league has a couple blocks of code as well as instructions. Make sure to read the instructions. You will probably be blocked by FBRef for several hours if you try to download each season's logs at once.

The only thing you need to change is what season to run the code for. To do this, you'll comment and uncomment each season. The program defaults to having the 17-18 season run first (the other season are in blue, italics, and have a '#' on the far left at the start of their line).

So, run that block first, then when it finishes, wait about 30 seconds to avoid being blocked by FBRef. Patience. Then, comment out the 17-18 season by either typing a '#' at the start of the line like the other seasons, or by clicking anywhere on it's line and pressing ctrl+/ on your keyboard.

Then uncomment the next season by either deleting the '#' in its line or clicking in its line and pressing ctrl+/ on your keyboard (crtl+/ both comments and uncomments!).

Finally, once you have run all seasons, run the block of code below it. Than, you'll need to open up the final csv file in Excel or Google Sheets and follow the directions just below that second block.

Basically, enter 1 in the first cell of the Match Number column, and then that formula ( =IF(R2=R3,IF(S3>S2,1,Y2+1),1) ) in the cell below the 1. Then drag that formula all the way down.

Repeat those steps for all the leagues you want matchlogs for and then you can run the League Ridge Line Plots or the Moving Average Charts programs

### League Ridge Lines

This program generates stacked distributions for all teams in the league you want to visualize. Just like the other programs, enter the required info in the area thats says "enter the desired info here". Then run the program and there's your chart!\

### Moving Averages Charts

Same dance as the others! After you have the match log for the league the club you want to visualize plays in, just enter the required information where it says, and run the program.

This program could need some basic coding if you visualize a team that has not played in all 5 of the recent top-flight seasons. If so, scroll to the very bottom of the code and you'll see under the "if image_ == 'y' " line a string of 4 numbers after 'add.axes'.

I have tried to give some direction on what to change and how, but you may need to play around with those 4 numbers to position your club's image perfectly. The first 2 numbers control the x/y position of the image, while the second 2 numbers control the image's height/width. Please reach out to me if you have questions, of course.

# 

Overall, I hope that you won't need too much coding experience to run these programs. You'll of course need coding experience if you want to customize them (colors, titles, etc.), but if you're wanting to fully customize them I'll assume you know how code some decent amount of Python anyway! If not, feel free to reach out to me and I can help you get your 'brand' or 'style' instead of mine.

Finally, never hesitate to contact me, ever. I hope people can use this not only as a guide for thier code, or as a way to quickly download some scouting reports on their favorite players, but also to help anyone who wants to learn Python. If you have any questions at all, or especially if there are problems with the code (or just want to chat about why I did X or Y), shoot me a DM on Twitter! @BeGriffis.

Good luck everyone and thanks for using this!
