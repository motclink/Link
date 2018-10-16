# 壹、資料前處理

* 處理時機：當使用者僅有設備點位資料表格，無 .shp圖檔。

  一、將設備點位資料檔案(須含經緯度座標)轉換成點圖層，並存成 .xls檔案格式。
  
   * **注意：每一筆資料須給定唯一一個ID編號，以利後續進行Link圖層對應。**
     
     
  ![圖1 原始資料範例檔](0/0-1.png)
     
  
  二、將 .xls檔案加進ArcGIS，在檔案上按滑鼠右鍵**Display XY Data**。
  
  
  ![圖2 功能清單之一](0/0-2.png)
     
     
  三、**X Field**、**Y Field**分別選擇設備點位資料所自訂的X、Y座標欄位。
  
  
  ![圖3 Display XY Data功能視窗](0/0-3.png)
     
       
  四、按**OK**後，即於ArcGIS上完成點位定位，後續將此圖層輸出即可開始進行Link圖層對應。
    
  ![圖4 功能清單之二](0/0-4.png)
     
          
  ![圖5 設備點位產出結果示意圖](0/0-5.png)
     
   
  ![圖6 設備點位產出圖層之屬性資料](0/0-6.png)
  

# 貳、設備點位對應Link圖層（方法一）

  一、所需圖資：設備點位圖層、Link圖層。

   * 本案例使用自行新增之點圖層及縣142 Link圖層
   
   ![圖7 設備點位及Link圖層套疊示意圖](1/1-1.png)
 
  二、將縣142 Link圖層RdDirectID欄位數值為0與1的值分別輸出。
  
   ![圖8 LinkID與RdDirectID欄位數值示意圖](1/1-2.png)
  
   1\. 在縣142 Link圖層上點滑鼠右鍵，選擇**Open Attribute Table**功能，開啟圖層屬性表。
   
   ![圖9 功能清單之三](1/1-3.png)
   
   2\. 開啟屬性表點選**Options**選單，選擇**Select By Attributes**條件式查詢功能。
   
   ![圖10 Options功能選單](1/1-4.png)
   
   3\. 開啟**Select By Attributes**條件式查詢後，給予RdDirectID＝0指令，並點選**Apply**。
   
   ![圖11 Select By Attributes功能視窗（RdDirectID＝0）](1/1-5.png)
      
   4\. 在縣142 Link圖層上點滑鼠右鍵，選擇**Data** → **Export Data**功能，將RdDirectID＝0的資料輸出，另存新檔給予自訂檔名（如圖12、13），即可擷取出所有RdDirectID＝0的資料（如圖14）。
   
   
   ![圖12 功能清單之四](1/1-6.png)
   
   
   ![圖13 Export Data功能視窗](1/1-7.png)
   
   
   ![圖14 縣142 Link圖層RdDirectID＝0之輸出結果](1/1-8.png)
   
   
   5\. 擷取RdDirectID＝1的方式請重複3～4的步驟，差別僅在步驟3給予RdDirectID＝1指令（如圖15），即可擷取出所有RdDirectID＝1的資料（如圖16）。
   
   
   

# 參、設備點位對應Link圖層（方法二）

# 肆、自有道路圖資對應Link圖層
