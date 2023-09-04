# 從Notepad++到JetBrains：我的IDE之旅
---
aliases: [jetbrains, pycharm, webstorm,  vim, acejump, ide, copilot, chatgpt]
---
# 這邊不會說什麼
- 不會有精美的 PPT 只會有樸實無華的日常操作
- 不會說 JetBrains 基本的介紹，這個一堆影片都在教了，我只會講我平常看到一堆人不會做的事情，一般會講的這些皮毛自己看看就好
- 不會說任何 ai 的技術，我最多只會給你們安麗 chatgpt4 還有 copilot/tabnine/ai assistant 這些強大的 ai 工具
- vim 太簡單的我不想說，太難的我又講不了，我不會講的太深，因為他博大精神我也是淺淺的微笑，就像烏梅子醬，我只講我平常的使用方式
	- 你最少要了解什麼是 normal/visual/normal mode 跟 hjkl 這些是什麼
- vscode，因為我完全不會，摸了兩天還是會回到JetBrains，想學 vscode 出門左轉
- 同理，Windows 出門左轉，有些東西在 windows 上的東西我其實也不是很懂，畢竟我只有 Mac
- 學會這些不會讓你變成大神，只會讓你變成一個更成熟的程式搬運工（碼農）

# 這邊會說什麼
- 滑鼠派的請走出去左轉，JetBrains 上很多常用的指令或熱鍵其實幾乎不需要用到滑鼠
	- 我就想要像一個駭客一樣純粹的用鍵盤裝個大逼
	- 一頓操作猛如虎，手法嫻熟猶如舞
- JetBrains 是如何好的一個 IDE 不要再把他當作一個單純的 Editor
	- 很多人根本不認識自己的 IDE
	- 東裝一個套件西裝一個套件，JetBrains已經大部分都打包好了
- 要達到上面的裝逼條件一定要多少認識 Vim
	- vim 他有個學習曲線，剛開始會很痛苦，漸漸會喜歡這痛苦，之後你會無法離開他
	- 我是學了第三次才沒有棄坑直到使用到今天，我很感謝我過去的決定
	- 曾經有人問我如果沒有 JetBrains 跟 Vim 我該怎麼辦？也許我會轉行賣雞排吧
	- 我要把你的方向鍵盤全部換成 hjkl，如果可以我也會把你的esc 改成 caps lock
- 除了 JetBrains 以外我還會常用的幾個工具
	- raycast
	- pastbot(可用 raycast 代替)
	- karabiner
	- always your best friend - chatgpt
	- chrome-extension
- 分享我所有的工具以及我的 setting
	- 這些設定十年磨一*鍵*，濃縮了所有的精華
	- 所有的設定依造你自己的喜歡打造你個人的開發方式，我的不見得適合你

# 前言（廢話）
身為一個工程師，本身就是要不斷的學習加點自己的技能樹，通常都會在專業領域上，但是我個人本身就反骨，人家在學演算法在解決 leetcode 的時候，我在想怎麼樣可以讓開發更輕鬆快速，整天都在想這些有的沒有的。

為了想要達成這個目的開始自學搜尋網路上的資料，直到我找到了這個啟蒙課程 [91 極速開發](https://tdd.best/courses/)
但是其實太貴而且是在台北所以我從來沒有去上課，我只有看他們練習的影片去尋找他們的方法
Reference:https://www.youtube.com/results?search_query=91+%E6%A5%B5%E9%80%9F%E9%96%8B%E7%99%BC
因為我也沒有上課，我只能說我也許也只學到很皮毛的東西，但是這些對我來說就非常實用了
如果你們聽完這堂分享會如果有更多的興趣的話
- 我非常歡迎隨時跟我討論（我很喜歡討論這種事情，也許你的問題也可以幫助我更加完善我的系統）
- 上 91 課程
- follow 91 極速開發 或是 kata 相關訊息
# JetBrains
他的付費解鎖以後功能真的很強大，身為工程師投資點錢在自己的工具上不為過吧？
但是我接下來會安麗的東西的確有些都要錢
## 常用 default 工具
### Git
![[Pasted image 20230903143731.png]]
豐富的 GUI 介面，以及常用功能，你可以快速的 checkout your branch，因為不是 git 教學，這邊不再著墨，最簡單就是上面那些點選
### Database
很多人喜歡 IDE 用 JetBrains 但是再用其他套的 Database 工具，我自己是覺得他的全家桶已經非常的厲害了，不需要做這些事情
![[Pasted image 20230903144101.png]]

### Remote Host
如果你們有機會要遠端 code 在某一台上面跑的話，你可以設定 ssh 以及你要 synchronize 的 path ，跟你最後要跑的 python environment

![[Pasted image 20230903144635.png]]
Note: 通常會到這樣的話，可能就是你的專案跟某些服務的耦合度非常高，你必須要 remote 在那台 server 上跑，但是業務邏輯或是各種原因條件無法允許，才需要這種特殊的做法

### Scientific mode +SciVIew
![[Pasted image 20230903153749.png]]
SciVIew: 你可以知道 pandas+plots 一些圖片等資料
Pycharm only，但是我非常喜歡的，平常要寫一些 demo code 的話我都會用這個
用起來很像 jupyter
你可以在你的 code 上
```python
# %%
```
加上這個後他就會自動換行
![[Pasted image 20230903154420.png]]
你可以執行 ctrl+enter run cell code
並且可以知道你右邊的變數是什麼
![[Pasted image 20230903154607.png]]

## Live Templates
![[Pasted image 20230903155127.png]]

### Surround with cmd+option+T
![[Pasted image 20230903160941.png]]
## 好用的 plugins

### Auto Completion
- AI Assistant
- Github Copilot
- Tabnine
### UI
- Indent Rainbow
- Rainbow Brackets Lite
- Rainbow CSV
- Solarized Themes(因為我很喜歡這種風格)

### Operation
- IdeaVim
- AceJump
- Tab Shifter
	- https://plugins.jetbrains.com/plugin/7475-tab-shifter
	- 現在每個人的螢幕都很大，不太可能一個 IDE 都只顯示一個 code
## 熱鍵/Setting
Ref: https://github.com/s724959099/jetbrains-setting
### Keyboard shortcut
![[Pasted image 20230903152538.png]]
可以看到很多 cmd+U, A 就是先按了第一個以後再看第二個
比如說我也很多設定 debug ....etc 等等之類的熱鍵，這些我就不一一贅述，因為我的不一定是好的，有些設計我覺得可以在優化，可是我已經習慣了
但是如果你有用我的 setting 的話你可以找找看我有異動的 keymaps

### Find Action option+a
有時候你不知道你的指令，但是你可以大概猜你想要做什麼事情，或是有些不常用的指令我不想設定熱鍵，我就會用這樣的方式去找
![[Pasted image 20230903152330.png]]

### Find in Files cmd+shift+f
![[Pasted image 20230903152836.png]]
你可以在專案上找尋你特定想要找的 code，可以整個 project or 特定的 directory

### Files cmd+shift+o
適合你要找特定的 module
![[Pasted image 20230903153009.png]]

### Recent Files cmd+4
除了找你最近使用的 我也很常用來打開 周遭的 tool，也可以透過這邊去看有些你有設定的熱鍵
![[Pasted image 20230903153107.png]]

### File Structure cmd+u,s(特別設定)
![[Pasted image 20230903153453.png]]


## IdeaVim or Keymaps
Note: 我不會介紹一些簡單的按鍵是因為有一些常用的我根本不會用 比如 yy 我還是比不是 cmd+c/v，比如說 p 我卻把他拿來改成其他的按鍵使用
我的想法很簡單，工具是幫助你節省時間的，不是給你製造壓力的，不代表你一定要完全100%按照別人說的去做，像我覺得 yy 雖然很好用，但是 cmd+c 是我最習慣的，並且結合平常的使用，平常在其他的時候可沒有 yy 這個指令，所以思考過後我還是會使用 cmd+c
當然這只是我的一個準則，你不一定要 follow

Note2: 其實 yy 也只是因為他是基於某些單字 比如 p: past, y: yank u: undo...etc，所以也不會太難記憶

### 常用的按鍵
leader: space
- 很多的 shift 通常是往回一個 
- ctrl+G select 重複的單字
- w/e or shift+w/e select previous/next word
- shift+hl 最左邊最右邊  / insert mode: shift+cmd+hl
- shift+v 整個 line
- v then (shift)+w/e
- s/d/S/C
- v+u or ~ 大小寫
- option+shift+j/k multiple cursor

- f: acejump
- p/shift+p select multiple chunks
	- 有很多操作我不會我都是直接用這個代替
- selected:
	- shift+S+f: function
	- shift+S :()"" / []...etc
- vim-surround: https://github.com/tpope/vim-surround
- . -> 重複上一個動作 ex cs"'
Q macros
```
a = 1  
b = 2  
c = 3
```
- shift? search
	- n & shift n next/previous

regular expression
- leader+sc clean old selected data
- :%s/<第一匹配>/<替代後的資料> /g 全部
- :%s/\(.*\):\n\(.*\)/'\1':'\2', /g
- *start 替代目前現有的字


- Window 放大或縮小: ctrl+option+hjkl
- 同一個 tab 遊走: ctrl+option+cmd+hjkl
- IDE editor 邊界放大縮小  leader+方向鍵
- close window: cmd+w
### Move Window
```
" Window operation  
nnoremap <Leader>ww <C-W>w  
nnoremap <Leader>wd <C-W>c  
nnoremap <Leader>wj <C-W>j  
nnoremap <Leader>wk <C-W>k  
nnoremap <Leader>wh <C-W>h  
nnoremap <Leader>wl <C-W>l  
  
  
  
  
nnoremap <Leader>ws <C-W>s  
nnoremap <Leader>w- <C-W>s  
nnoremap <Leader>wv <C-W>v  
nnoremap <Leader>w\| <C-W>v  
nnoremap <Leader>wm :action MoveEditorToOppositeTabGroup<CR>
```
# Karabiner
Setting Referenece:https://github.com/s724959099/jetbrains-setting/blob/master/karabine_setting.json
#### 設定說明
1. **CAPS HJKL to arrow keys p/u PAGE UP/DOWN**
    
    - 當 CAPS LOCK 被按下，`H`, `J`, `K`, `L` 對應到箭頭鍵。
    - `D` 和 `E` 分別對應到 PAGE DOWN 和 PAGE UP。
2. **grave_accent_and_tilde to right_shift**
    
    - 把按鍵 `~` (`grave_accent_and_tilde`) 轉換成 `Right Shift`。
3. **ctrl+grave_accent_and_tilde to grave_accent_and_tilde**
    
    - 當按下 `Ctrl + ~`，它會照常輸出 `~`。
4. **Ctrl+Caps Lock to Caps Lock**
    
    - 當按下 `Ctrl + Caps Lock`，它會輸出 `Caps Lock`。
5. **Option + HJKL to arrow keys**
    
    - 當按下 `Option + H/J/K/L`，它會模擬對應的箭頭鍵，並保留 `Option` 修飾鍵。
6. **Caps Lock + nm,. to Option + arrow keys**
    
    - 當 CAPS LOCK 被按下，`N` 和 `M` 會對應到 `Option + Left/Right Arrow`。
7. **Caps Lock + yuio to Option + Shift + arrow keys**
    
    - 當 CAPS LOCK 被按下，`Y` 和 `U` 會對應到 `Option + Shift + Left/Right Arrow`。
8. **Caps Lock + q to Backspace**
    
    - 當 CAPS LOCK 被按下，`Q` 會對應到 `Backspace`。
9. **caps_lock to escape**
    
    - 把 `Caps Lock` 鍵轉換成 `Escape` 鍵。

最關鍵的就是 Caps Lock，加上 hjkl 可以讓你平時做文書編輯的時候 不一定要在 coding 才可以模擬 vim，而且 Caps Lock 本身對應 `ESC` 按鍵，在 vim 的操作下其實你會很成按 `ESC` 但是其實他的距離有點遠，如果換成 Caps Lock 的話距離其實近很多，加上按的頻率差很多
我自己的個人理念是，盡量手指在 asdf jkl; 這些上 盡量不要移動超過這個地方

Note: 2, 3 點是為了個人需求 ，因為我同時搭配了超注音這個輸入法，所以需要有這個設定
讓我再按下 `~` 時可以切換中/英文 同時加上 ctrl 可以保留原本的功能

小插曲: 另外我個人非常推薦這個輸入法 `超注音` 如果是有用注音且喜歡不用打完整猜你打的字的話，可以試試看，但是需要付費，一次性的，我個人覺得非常值得，但是我沒有收到他們的贊助，我的幅度就不會過多的介紹 XDD（開玩笑的），是因為太簡單了 就是單純一個分享而已。

我曾經想要嘗試大陸的拼音輸入法，但是不太習慣，且要花的時間過多，所以如果你本身就是在用注音的人可以無痛轉換


# Chrome-extension
## [Vimium](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb/related)
Reference: https://github.com/philc/vimium
### Custom key mappings
```
# Insert your preferred key mappings here.
map a scrollDown
map s scrollUp
map h scrollPageDown
map l scrollPageUp
map e scrollPageUp
unmap b
```
- Shift+ J/K 切換 tab
- f called `acejump`
- command + [/] previous/next page
- operate like vim (j/k/ gg/shift+g)
- e/d scroll page
- o(網頁搜尋) & T(page tab)
- yy -> cmd+l cmd+c
- Comand t/w command+shift+t 都是基操勿6 
- yt: duplicate current tab
- W: move current tab to new window
