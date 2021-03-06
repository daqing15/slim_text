# Slim Text

Slim Text is a Slim Text editor which runs inside a web browser.

Official website: http://slimtext.org

![for Windows](http://slimtext.org/images/windows.png)
![for Linux](http://slimtext.org/images/linux.png)
![for Mac](http://slimtext.org/images/mac.png)



## For Windows 8 users

"This application is not supported on this computer. Installation has been disabled"

Run chrome in Windows 7 compatible mode can fix this issue:

1. right click on Chrome shortcut, select "Properties"
2. switch to the "Compatibility" tab
3. check "Run this program in compatibility mode for:"
4. select "Windows 7"
5. click "OK"

It is said that after installation you can disable compatibility mode and Slim Text will still work.



## Do you want to contribute?

If you want to contribute, here is list of tasks that you can do:

1. Add support for all the themes and modes that supported by ACE editor.
2. Create an better icon for Slim Text



## priority items

182, 142, 135, 68



## todo list

68. auto detect file change outside of the editor and load the newest content into editor
    1. advanced feature, postpone
    2. can check last modified time using boost filesystem api
    3. listen to focus event of document, then check file for each editor
97. enable ace editor features:
    1. remove trailing spaces upon saving
        1. some one hate trailing spaces a lot!
    2. add new line to the end of file upon saving
    4. auto complete
    5. it seems that I have to implment those features myself, ace doesn't provide such features.
105. introduce plugin system
    1. page actions, to change the appearance or behavior of the software, such as change background, such as define new shortcut key 
    2. advanced feature, postpone
    3. is it viable and practical?
111. bug: windows 7 C: / Windows / System32 / drivers, can not see the etc/ folder
    1. and a lot of *.sys files are invisible too.
    2. notepad++ has this issue too
112. bug: slow when open windows 7 C: / Windows / System32
    1. caused by underscorejs filter method?
118. should be able to open a folder quickly.
    1. for example, register a folder as a button, and click that button.
    2. register workspace, quick open
        1. open recent files or folders?
125. launch via command line, such as subl . &
133. open a new tab, default path is the current tab's path?
    1. the same as ubuntu terminal
    2. if already have a window, then no need to open all of the files, just navigate to folder path ?
135. go through this page: http://ace.ajax.org/#nav=production
140. add command line
    1. gcli: https://github.com/mozilla/gcli
    2. research, find the best solution!
142. add increase font-size or decrease font-size to menu ?
    1. and persist locally
    2. when open the editor, first check local storage, then check sync storage, and then last storage. Use the first one found.
157. bug: searchbox too weak, can not specify case-sensitive and regex search
158. chrome history api to go back to last folder?
    1. I think use history api for quick file open is possible. can do free form searching
160. bootstrap Typeahead can replace omnibox
161. a viable quick open solution: 
    1. everyting time open a folder, add the files in the folder into chrome.history
    2. ctrl + P show a input box
    3. use chrome history search to search
    4. bootstrap typeahead to show candidates
    5. select a candidate to open
162. Preview markdown: https://gist.github.com/4670615
163. cvanalyze.com click qq icon can launch qq, investigate
166. spell check (it is an ext of Ace)
169. 这篇文章不错： http://www.ibm.com/developerworks/library/os-extendchrome/index.html
172. differentiate states for some operations
    1. such as show/hide invisibles, two states: show invisibles and hide invisibles
176. compress html files before deployment
177. bug: Emacs ctrl + n conflicts with chrome create a new windows
    1. if I am an Emacs user, I feel quite annoying
182. remove/rename file/folder
    1. show remove/rename icons on the left panel whenever mouse over
188. hidden files, useless files such as *.pyc
    1. some body said that they didn't want to see them
    2. combine this feature together with show invisibles quick button?
191. update the website once standalone version is ready
192. create chrome packaged app version?
    1. there are issue: jquery ui layout does not run in chrome packaged app
        1. packaged app does not support unload event
        2. but I can create the app wihout jquery ui layout
    2. can not list a folder. only file dialog available. 
        1. user have to open a dialog each time he wants to open a file
        2. So NPAPI is still needed
    3. already have chrome extension version and Qt version
    4. at least two users request this
    5. but I cannot see the value. there is no major advantages.
194. file content encode issue on windows
    1. create a text file, contains Chinese characters. The file encoding is ANSI by default
    2. open in Slim Text, Chinese characters are unreadable
    3. bug: chinese encoding decoding issue for C:/QQDownload/From Tyler/01.htm
    4. bug: windows csharp file, show BOM as * (because cannot handle utf8 with BOM)
200. bug: cannot see mounted external dirves in windows. such as virtualbox shared folder
202. Preview HTML
211. two many files opened, tabs bar not enough space to hold them
212. context menu: https://github.com/medialize/jQuery-contextMenu
214. drag & drop tabs
    1. jqueryui sortable kind of buggy
216. popup window task bar icon too small on windows
    1. chrome's bug, postpone: https://code.google.com/p/chromium/issues/detail?id=94301
218. remember the current active tab
220. add google analytics to slimtext.org
221. disable status bar when hover on tabs
    1. no easy way
    2. a possible solution: remove href upon hovering, add href back upon clicking. save href value in data attr
227. encourage user to rate the extension
229. new themes and modes added in the latest ace
230. 
