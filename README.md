# 交通資訊基礎路段編碼說明文件

&emsp;&emsp;交通資訊除數據本身外，亦須載明資訊所在之位置，始具有實質意義。「路段編碼」是交通資訊一種常用的位置參照表示法，同時也是交通地理資料庫中路段物件的索引，為因應未來多元資訊之蒐集、發布及交換需求，交通資訊「基礎路段編碼」之設計有別於一般編碼系統使用的流水號，採用多碼段、結構化(Structural)的編碼方式，配合適當的字串比對語法，即可快速檢索出所需路段的交通資訊。本計畫執行之基礎路段編碼，主要以車輛行駛之重要路網為對象，以優先滿足交通路況發布應用需求為目標，包含國、快、省、縣道及重要市區道路，並以改變均勻車流之節點為「道路分段點」進行後續編碼作業。

&emsp;&emsp;本書分別透過三大主題加以說明：

 * **路段編碼內容**：說明路段編碼各碼段的定義及編碼方式。
 
 * **路段編碼對應**：提供主題資料(里程、運輸場站、門牌地址及路側設施)對應路段編碼邏輯，以及自有設備或道路圖資透過GIS工具對應至Link圖層之操作說明。
 
 * **系統相關文件**：針對系統LinkID導入工具操作方式進行說明，以及系統API輸出表單內容。
 
 
