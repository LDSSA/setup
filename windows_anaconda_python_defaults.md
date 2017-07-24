## Configure Anaconda3's Python distribution as Windows10 defaults

## Target audience
This tutorial is for you if, like me:
- You are using Windows 10 with Python to develop Data Science contents.
- You want to use Anaconda3 as default, <b> currently </b> regarded as one of the best Data Science Python Distributions (and non Python :) ).

## Description of the Problem
When some users install Anaconda3 in their windows environment, the install recommends not to add Anaconda3 to %PATH% (Windows environment variable). Users often will follow the given suggestion.
After installation, some Pythpn power users like to use their "old" but also "fast" workflows and tools, like "Sublime Text 3" and have access to Command Prompt Python.
Since it wasn't added anything to %PATH% these tools will not recognize Anconda3 Python as their default Python interpreter.
The simple solution, which can be obvious for any experienced user, may be a bit complicated and time consuming to find out for the beginner.

## Solution
i) Verify if there is already a python.exe in %PATH% from other Python distributions you already have installed, that can obfuscate Anaconda3's.
- So press "Windows key + S" to open windows search;
- Type cmd for locating DOS like windows shell;
- Right-click with mouse and choose "Run as Administrator";
- type in cmd GUI: "echo %PATH%" which will output all the Windows Environment Variable %PATH% folders;
- type after: "where python" it will display any folder that gives direct access to Python;

ii) If any folder was found the options are to either:
- uninstall the competing distribution;
OR
- rename the Python.exe to Python3.exe or Python2.exe;

iii) Now configure Anaconda3's Python in windows as default:
- open windows explorer
- right-click the "This PC" folder (not the shortcut) and select Properties
- go to "Advanced System Settings"
- now select "Environment Variables"
- Select Path Variable in either User Environment (only affects current user) or Windows (will change for all users)
- Click Edit button, then new, and browse to Anaconda3's installation folder then add it into %PATH%
- Click ok.

iv) In sublime text you have to uninstall any Package that compiles Python with the name "Python" build, which is the name that is used by default system.

## RESULTS
![clone](http://imgur.com/0pCkIiq)

<b>Done Enjoy!</b>
