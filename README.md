# SmartSAJ package

This README will guide you through the setup process. If some of these steps don't work for you, please let me know so we can improve this package or the instructions.

## Prerequisites

- Windows 10
- Python 3.8+
- Python packages: bs4, jellyfish, standard library
- Visual Studio 2019+ (with asp.net and web developing)

### Downloading SmartSAJ

- You can download the project from http://www.mediafire.com/file/71ysb6k09nwgs4y/MarkoProjekat.zip/file
- (It isn't on the GitHub at the moment because of its size, soon it will be fixed)
- Download the main folder ("MarkoProjekat") in directory "D:/"
- Unzip the folder
- Note: it is important whether you download it in the mentioned place

## Downloading Python packages

- You don't need to download (but it is better if you do) packages such as bs4 and jellyfish. You can find them at: "D:/MarkoProjekat/SmartSAJ/venv/Scripts/Lib/site-packages"

## Setting up SmartSAJ

- Open file Funkcionalnosti.cs and edit the string python_path. It is in the 16. line of code. You should put path to your computers python (the one where you downloaded and installed packages). This will be fixed soon. 

## Using SmartSAJ

- Open MarkoProjekat.sln in Visual Studio and run the project
- First open page should be login screen. Username: admin Password: admin (traditionally).
- After you login, your screen should show you a text box and a button "Izracunaj". In the text box you should put the link of ste site you want to test. Then, you should hit the "Izracunaj" button. If you filled the text box with a wrong link or you didn't do the setup well, then a quick message will pop out.
- If you did everything right, then you need to wait a few minutes (the bigger the site the more time you will wait, please be patient). For testing purpose you can put a small Wikipedia site or for example "https://gsm-nis.edu.rs/".
- When the testing ends, a bar will show under with information about the site.
- If you test multiple sites, they will all show in separate bars

- On the right bottom corner you can find other features. When you clcik on "Bezbedni sajtovi" or "Opasni sajtovi" you will find a table with top 10 safest/most dangerous sites that were tested by you, or were tested before you downloaded the project.

- If you go to the "Update" part, you will see two text boxes (left and right). This feature enables the program to "learn" new keywords and update the values of keywords that were already there. The left text box is for the sites that you judge are safe and the right text box is for the sites you judge are dangerous. You can put multiple sites at a time, with newline between them. This process is very fast and it should take no more than a second or few (if you don't put too many links). After the updating and learning is finished, a message will pop out to say so.

**Bugs that should be fixed soon.**

 - All the paths in the program are not relative, they are constant. The problem was with using few different languages (Python, C++, C#) and each of them having their directory.

## Upcoming features

- Faster testing (adding data bases instead of .txt files)
- More detailed esting (you can see the beta version in oceni_exp.py)
- Testing for languages other than English
