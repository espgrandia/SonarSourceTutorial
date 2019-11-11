# Sonar Source 使用心得及教學

* 主要內容如下:
  * sonar source 的用途
  
  * Mac Client 環境建置
  
  * objc/swift 測試專案

  * 測試過程記錄

  * sonar qube 建構環境

  * sonar qube 設定正式的 License Key

---

## 扼要說明

* 靜態程式碼分析軟體

  * 支援多種程式語言

  * 主要區分 SonarQube，SonarLint，Code Analyzers

---

## [SonarSource 說明](./Note/README.md)

## [Developer Edition Trial Install](./Developer_Edition/README.md)

## [Mac Client 安裝環境](./MacEnvInstall/README.md)

## [Delete Project 測試](./Delete_Project_Test/README.md)

## [Sonar Qube 安裝](./SonarQubeInstall/README.md)

## [Sonar Qube 設定 License Key](./Set_License_Key/README.md)

---

## TODO 分析參考

* [SonarSource Price 分析]

---

## 官方參考網址

* [SonarSource](https://www.sonarsource.com/)

* [SonarQube](https://www.sonarsource.com/products/sonarqube/)

* [Code Analyzers](https://www.sonarsource.com/products/codeanalyzers/)

---

## TODO List

* Objective-C 的 Coverage 剖析失敗部分(關鍵字如下)

  * UnitTest 涵蓋率。
  * xcrun command line。

* build wrapper

  * libinterceptor.dylib 有警告訊息

* sonar-scanner

  * 指定不同名稱的 xxx.properties

    * 預設名稱為 (sonar-project.properties)

  * 是否有混合型語言剖析可行性

    * e.g. objc/swift...

  * 排除資料夾

  * 測試 workspace 專案

    * 有使用 cocoapods 的專案

  * properties 是否可以建成樣本

* Price 的確認

  * OLC 行數:
    * 測試結果是全部專案的統計行數。
    * 不過刪除專案行數會降回來

* 結合 ci

  * Jenkins

* sonar qube

  * branch 機制測試

  * 熟悉操作 ...
