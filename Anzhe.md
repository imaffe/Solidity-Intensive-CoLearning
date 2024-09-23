---
timezone: Asia/Shanghai
---

---

# Anzhe

1. 自我介绍
大家好，我是 Anzhe，是圖書資訊、資訊工程雙主修的大五學生，對資安領域感興趣，目前一邊補基礎一邊探索資訊、資安各種領域，希望能多多學習各種知識和技術，增加自身能力。
2. 你认为你会完成本次残酷学习吗？
我覺得這次殘酷共學對我來說是了解 Web3、區塊鍊和智能合約的好機會，同時也是對自我的挑戰，我會盡力規劃好時間，努力完成本次的共學目標。
## Notes

<!-- Content_START -->

### 2024.09.23
# Solidty
　　Solidity 是為了全球市值第二的加密貨幣市場乙太坊（Ethereum）創建的程式語言，發布於 2015 年，是為了實現智能合約而設計的物件導向高階程式語言、一種針對以乙太坊虛擬機器的花括號語言，它受到 C++、Python 和 JavaScript 的啟發，用來編寫可以自動執行合約條款的智能合約，更是區塊鍊運行平台的主要使用語言，可以用於創建投票、盲拍、群眾募資、多重簽名錢包等用途的合約。

### Solidity 主要特點
1. 靜態類型語言：編譯時需要指定每個變數的類型。
2. 合約繼承：支持合約的繼承，讓開發者可以重用程式碼。
3. 函數修飾器：用來修改函數的行為，例如限制只有合約擁有者可以調用某個函數。
4. 事件：智能合約可以發送事件，供前端應用或其他合約監聽。
# 智能合約
智能合約是乙太坊最大的創新之一，開發者編寫、部署自動執行合約條款的智能合約到乙太坊區塊鍊上，智能合約在部署到區塊鏈後，能夠不依賴第三方自動執行和記錄交易，並且記錄是不可更改的。
# 乙太坊
乙太坊是一個去中心化的開源區塊鍊平台，主要支援分散式（去中心化）應用和智能合約。和主要用於數字貨幣交易的比特幣和其他區塊鍊平台的差異在於：乙太坊提供了一個能夠執行編程邏輯的區塊鏈環境——乙太坊虛擬機(Ethereum Virtual Machine)，它是一個分散式的計算機網絡，保證每個節點能夠正確執行合約，開發者可以在其上構建和運行去中心化的應用。

---
# Solidity 101
開發工具 `Remix` : [https://remix.ethereum.org](https://remix.ethereum.org)
教程使用 `Remix` 運行 Solidity 合約，`Remix` 是乙太坊推薦基於瀏覽器的智能合約整合式開發環境（IDE）。

## Remix 開發流程
Remix 左側面板，選擇`文件`面板可以新增`檔名.sol`檔案用 Solidity 開始編寫只能合約，快捷鍵 `Ctrl + S` 可以對檔案進行編譯，選擇`部署`面板並點擊 `Deploy` 則可以把智能合約部署到區塊鍊上，`Remix`會分配一些測試帳號給使用者，每個帳號有 100 ETH 的測試幣可以使用，每次部署合約會扣掉一點點。
![](https://i.imgur.com/eBMY37U.png)

## Hello Web3 程式碼
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.21;
contract HelloWeb3{
    string public _string = "Hello Web3!";
}
```
### 說明
1. `//` 是單行註解，說明程式碼使用的 License 許可是 `MIT`，註解的內容不會被執行，若不寫許可程式仍可執行，只是編譯時可能會出現警告。
2. Soldity 語句需以 `;` 結尾。
3. `pragma solidity ^0.8.21;` 宣告文件使用的 Solidity 版本，版本不同會有語法差異，`^` 代表向後兼容，表示允許 0.8.21 版本以上的 0.8.x 版本編譯器編譯，但不包括 0.9.x 或更新的版本。
4. `contract HelloWeb3` 是創建合約，並宣告合約的名稱為 `HelloWeb3`，花括弧內則是合約的內容，宣告了一個字串的變數 `_string` 並賦值為 `Hello Web3!`。

部署完畢後，`部署`面板滑到最下方，可以看到名為 `HelloWeb3` 的智能合約，點擊變數 `_string` 可以看到變數儲存的內容。
![](https://i.imgur.com/JE6E9KQ.png)

<!-- Content_END -->