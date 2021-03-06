# VS Code Setting

## Keybinding Costom Setting

**참고**<br>
https://code.visualstudio.com/docs/getstarted/keybindings#_when-clause-contexts

**텍스트 관련**
* Go to Symbol in Workspace : alt + y
* Insert Line Below : shift + enter
    * settings.action.focusPreviousSetting : 삭제
* Expand Selection : alt + shift + up
* Fold : ctrl + [
    * Outdent Line : 삭제
* Unfold : ctrl + ]
    * Indent Line : 삭제
* Fold Level 1 : ctrl + shift + [
    * When : editorTextFocus && foldingEnabled && resourceExtname == '.js'
* Fold Level 4 : ctrl + shift + [
    * When : editorTextFocus && foldingEnabled && resourceExtname == '.vue'

**Terminal 관련**
* Terminal: Create New Integrated Terminal : alt + t
* Terminal: Focus Next Terminal : alt + pagedown
* Terminal: Focus Previous Terminal : alt + pageup
    * scrollPageDown : 삭제
    * scrollPageUp : 삭제
* Terminal: Focus Terminal : alt + end
* Terminal: Kill the Active Terminal Instance : alt + delete
* View: Toggle Panel : alt + p
    * keybindings.editor.toggleSortByPrecedence : 삭제

**탭 관련**
* View: Focus Next Editor Group : ctrl + alt + pagedown
* View: Focus Previous Editor Group : ctrl + alt + pageup
    * Terminal: Scroll Up(Line) : 삭제
    * Terminal: Scroll Down(Line) : 삭제
* View: Decrease Current View Size : ctrl + alt + =
* View: Increase Current View Size : ctrl + alt + -
* workbench.action.closeEditorToTheRight : ctrl + alt + r
* workbench.action.closeEditorsInGroup : ctrl + alt + w
* workbench.action.closeOtherEditors : ctrl + alt + o
* workbench.action.keepEditor : ctrl + alt + home
* Go to the file path under the cursor : ctrl + alt + p

**Side Bar 관련**
* explorer.newFile : ctrl + n
    * File: New Untitled File : 삭제
* explorer.newFolder : alt + n
* File: Collapse Folders in Explorer : ctrl + shift + [
    * When : filesExplorerFocus
* Search: Collapse All : ctrl + shift + [
    * When : searchViewletVisible && !editorTextFocus
* View: Show Explorer : ctrl + e
    * Go to File : 삭제
    * View: Open Previous Recentrly Used Editor in Group : 삭제


## Extensions

* Eclipse Keymap
* Auto Rename Tag
* Current File Path
* Hexo tag snippets
* JavaScript (ES6) code snippets
* TabOut
* Rainbow Brackets
* CamelCase
    * CamelCase : ctrl + shift + 6
* GitLens - Git supercharged
* Code Runner
    * ctrl + shift + p - Run Code : js 파일 실행
* Vetur
* Vue Peek
* vscode-go-to-file
* ESLint
* Path Intellisense
* Settings Sync
* SQLTools - Database tools


## Setting

* "editor.foldingStrategy": "auto" -> "indentation"
    * JSDoc style, multiline comment fold 가능
* "terminal.integrated.shell.windows": "C:\\dev\\Git\\bin\\bash.exe"
    * git 경로가 default가 아니면 인식하지 못하므로 직접 세팅