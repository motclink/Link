# 「即時路況資料標準2.0」內容檢視

## VD、CCTV、CMS、eTag 路側設施靜態資料

* Input

  (1)坐標
  
    * PositionLon

    * PositionLat
    
  (2)公路編號/方向/里程
  
    * 如：國道1號/順向/15.3k

* Link相關欄位

  * LinkID

  * Bearing

  * RoadDirection

  * RoadID

  * RoadName

  * RoadClass

## AVI、eTag配對路徑靜態資料

* Input

  (1)起點坐標
  
    * PositionLon1

    * PositionLat1
  
  (2)迄點坐標
  
    * PositionLon2

    * PositionLat2

* Link相關欄位

  * LinkID

  * Geometry


# 基礎路段編碼內容

## 基礎路段編碼原則

* 一般路段：

  * 分向不分道
  
  ＊單行道：雙向編碼，惟status：不啟用。

* 虛擬線段：

  * 不具實質意義，不編碼

## 基礎路段編碼內容

## RoadID/RoadNameID/LinkID關係

* LinkID = 基礎路段代碼
* RoadID = 道路代碼

  * 公路(含市快)：RoadClass (1碼) + RoadNameID (5碼)
  
  * 市區道路：RoadClass (1碼) + RoadNameID (5碼) + CityID (1碼)
  
