# SonarSource

# 靜態程式碼分析軟體
 * 支援多種程式語言
 * 主要區分 SonarQube，SonarLint，Code Analyzers

# [Developer Edition Trial Install](./Developer_Edition/README.md)

# [Mac Client 安裝環境](./MacEnvInstall/README.md)

---
# 分析參考
 * [SonarSource ME 分析](https://docs.google.com/spreadsheets/d/10l0t31xGAcZTIaUls2cqtdzK03NYgGvtGsTJg2Y7ru0/edit#gid=37388302)
   * 裡面有 survey 資料及相關連結

 * [SonarSource Price 分析](https://docs.google.com/spreadsheets/d/10l0t31xGAcZTIaUls2cqtdzK03NYgGvtGsTJg2Y7ru0/edit#gid=1476733927)

---
# 參考網址
 * [SonarSource](https://www.sonarsource.com/)
 * [SonarQube](https://www.sonarsource.com/products/sonarqube/)
 * [Code Analyzers](https://www.sonarsource.com/products/codeanalyzers/)


---
# TODOList
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
    * e.g. 08專案
  * properties 是否可以建成樣本


* Price 的確認
  * OLC 行數 : 看起來似乎與原先想的 單一 project 上限似乎有出入。

* 結合 ci
  * Jenkins

* sonar qube
  * 刪除 project
  * branch 機制測試
  * 熟悉操作 ...
