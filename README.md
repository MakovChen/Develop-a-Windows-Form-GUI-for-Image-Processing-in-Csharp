# 自動化光學檢測之Windows Form (C#)釋例

針對未來打算從事或即將從事半導體及電子相關科技產業的IT人員，GUI的開發能力可以說是一項非常重要的基本功。無論過去在學校研究的是**機電控制**、**自動化** 或者是**機器學習(ML)**，這些理論的應用倘若要在企業的系統中實踐，都需要仰賴*與企業資訊系統的高度整合*。

這些內容其實也沒有想像中的那麼複雜，屏除那些原本就是由外包廠商提供的套裝軟體，大部分企業內部的電腦作業程序都是由自身所擁有的工程師撰寫。就如網路服務的部門因為有前/後端、資料庫整合的需求，通常會選擇Java作為主要的程式語言；對於比較強調內部運作、生產線控制與模組開發等封閉系統的部門，則主要會是以能兼顧開發效率、執行與通訊速度的C#作為主要程式語言。

而近年少子化的現象加上AI的高度發展，基於影像的分析在工業系統中被認為是下個世代必備的解決方案，用於協助各種自動化設備完成一些原本只有人類才能執行的高難度任務(關鍵字：工業4.0、智慧製造)。而身為這個領域的開發者，若要在企業原始的系統架構下加入這些新技術，就必須向業者提供**程式串接** 及**使用者管理介面** 的功能。

這份`repository`的內容主要就是在於提供這些流程的開發框架/模板，內容涵蓋了GUI、ML影像處理及基本系統架構的實現與觀念，藉此衍伸出各類專案的設計與開發。

## 目錄

- [開發工具](#背景)
    - [Visual Studio]()
    - [C#(C-sharp)]()
    - [EmguCV]()
- [影像處理]()
    - [影像形態學]()

## 開發工具
### Visual Studio
Visual Studio是Microsoft提供的程式編譯IDE，並以完善的開發工具著名。就以本次要開發的GUI為例，其就提供了拖拉式介面幫助我們編輯GUI的版型，並根據這個版型生成程式碼模板，使我們只要在每個物件寫上客製化的功能就能夠完成開發，減少很多不必要的開發時程。
*/紅色區塊為對應到視窗程序的程式碼*
### C#(C-sharp)
C#則是基於Windows系統衍伸的程式語言(也就是說它在windows上的執行效率最高)，而其也在繼承了C和C++優點的同時去掉了一些複雜繁瑣的功能，幫助我們更快地編輯所需實現的功能。

### EmguCV
EmguCV是一個基於OpenCV且支援$.$NET Framework的影像處理模組，可以直接使用`NuGet`第三方管理工具來獲取所需的套件。
*/[專案]>[管理NuGet套件(N)]*

## 影像處理

