# 介紹建構 sonar qube 的步驟

* info及安裝方式
  * 環境 : ubuntu
  * 預計安裝方式 : rancher 啟動 container 安裝 sonar qube

---

## 安裝步驟如下

* Step0(切換到 sudo 模式，方便之後安裝 @sonar-qube vm)

  ![Step 0](./pics/00.png)

* Step1(mount data: sonar qube 預設的 db 存放碟 @sonar-qube vm)

  ![Step 1](./pics/01.png)

* Step2(檢視 rancher 對應的 docker 版本 @rancher)

  ![Step 2](./pics/02.png)

* Step3(執行 下載並安裝 docker 命令 @sonar-qube vm)

  ![Step 3](./pics/03.png)

* Step4(執行 下載並安裝 docker 命令 過程 1 @sonar-qube vm)

  ![Step 4](./pics/04.png)

* Step5(檢視 docker 安裝版本是否一致 @sonar-qube vm)

  ![Step 5](./pics/05.png)

* Step6(點選 Add Host @rancher)

  ![Step 6](./pics/06.png)

* Step7(copy register host command @rancher)

  ![Step 7](./pics/07.png)

* Step8(執行 register host command @sonar-qube vm)

  ![Step 8](./pics/08.png)

* Step9(Click INFRSTRUCTURE @rancher)

  ![Step 9](./pics/09.png)

* Step10(Set Label with sonar @rancher)

  ![Step 10](./pics/10.png)

* Step11(Check sonar qube is running @rancher)

  ![Step 11](./pics/11.png)

* Step12(Check sonar qube is running @sonar qube 後台)

  ![Step 12](./pics/12.png)
