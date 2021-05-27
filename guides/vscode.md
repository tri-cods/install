# Visual Studio Code
A text editor is a simple notepad type application. For the DRI, we will be using the VSCode text editor because it supports [syntax highlighting](https://en.wikipedia.org/wiki/Syntax_highlighting), is free and open source, and is consistent across OSX, Windows, and Linux systems.

## Install
Download VSCode at https://code.visualstudio.com/ 
* [OS/X instructions](#osx)
* [Windows instructions](#windows)

### Windows
1. *Click* on the VScode installer in your downloads folder:

![installer shortcut - shaded blue box with ribbon logo. It has something like `VSCodeSetup-` at the front of its filename](../images/windows/vscode/vscode00.png)

2. When you see this window, *click* `Next`:

 ![initial installer window](../images/windows/vscode/vscode01.png)
 
 3. Accept the license agreement by *selecting* the first radio button. Then *click* `next`  
 
 ![license agreement install window](../images/windows/vscode/vscode02.png)
 
 4. Choose the folder on the computer that VSCode should be installed in (the default is usually fine). Then *click* `Next`:
 
 ![installation folder selection window with a browse button to enable you to search for an installation folder](../images/windows/vscode/vscode03.png)
 
 4b. Windows only: Choose the folder in the start menu that VSCode should be installed in. Then *click* `Next`:
 
 ![select start menu folder installation window, with a browse button to enable you to search for a folder on the start menu to ](../images/windows/vscode/vscode04.png)
 
 4c. Windows only: Please *check* the box that says `Add to PATH`, which is the fifth (last) box. Check the other boxes at your own discretion. Then *click* `Next`:
 
 ![Select additional tools menu of check boxes. The options are (top to bottom): i. Create a desktop icon, ii. Add `Open With Code` action to Windows Explorer file context menu, iii. Add `Open With Code` action to Windows Explorer directory context menu, iv. Register code as an editor for supported file types, v. Add to Path (available after restart)](../images/windows/vscode/vscode05.png)

5. You should see a window listing the configurations you chose in the previous steps. If they are incorrect, *click* `Back` and redo the previous steps. If they are correct, *click* `Install`:

 ![ready to install window listing configurations](../images/windows/vscode/vscode06.png)

6. Sit back and relax because the install will take a while. You should see a window with a progress bar similar to this:

![progress bar showing how far along the install is](../images/windows/vscode/vscode07.png) 

7. *Check* the "Launch Visual Studio Code" checkbox and then *click* `Next`

![setup finished window with launch visual studio code checkbox](../images/windows/vscode/vscode08.png)

8. [Test Install](#test-install)

### OS/X

To open code from the osx terminal (command line), we need to [add it to path](https://code.visualstudio.com/docs/setup/mac) after the install.

1. [Download VSCode](#download)

1. Drag the Visual Studio Code application to `Applications` folder. 
![osx finder window showing visual studio code icon](../images/osx/vscode/vscode.png)

1. Open VSCode via your preferred method.  *Click* on the icon:

![Visual Studio Code icon - black box with blue ribbon inside](../images/osx/vscode/path00.png)

2. Navigate to the `View->Command Pallet` menu and *click* on `command`

![VSCode top level menu bar, View is the fourth option down](../images/osx/vscode/path01.png)

3. The `Command Pallet` menu looks like this. *Type* `shell` into the text bar. Then choose "Shell Command: Install `code` command in PATH" 

![textbar with menu options underneath](../images/osx/vscode/path02.png)

4. Once the install is finished, you should be able to open a [terminal](osx_terminal.md) and *type* `code` and that should launch VSCode

![OS/X open terminal with the code command](../images/osx/vscode/path03.png)

8. [Test Install](#test-install)

## Test Install

VSCode should now be installed. You should see something like this window when you launch VSCode:

![main vscode screen with side panel menu buttons: file explorer, search, git integration, debugger/variable explorer, extension manager. Second panel is file browser to find file to open, and third panel is to chose customizations](../images/windows/vscode/vscode09.png)

Ignore the warnings about git not being installed. 
