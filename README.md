# 美國雲端主機：從節點、線路到價格，選出真正適合你的洛杉磯 VPS

搜尋「美國雲端主機」的人，通常不是單純想找一台放在美國的 VPS。真正影響使用體驗的，往往是三件事：**伺服器在哪裡、走哪條網路、你每月到底拿到多少 CPU、記憶體、儲存與流量**。

尤其是美國西岸主機，對北美使用者、亞洲跨境服務、API、網站、VPN、備份與開發環境的意義完全不同。便宜的美國 VPS 很多，但「美國節點」四個字本身其實沒告訴你路由品質、流量計算方式或高峰時段會不會遇到瓶頸。

DMIT 的洛杉磯（LAX）雲端主機值得單獨拿出來看，原因也很直接：它把洛杉磯節點拆成 **Premium、Eyeball、Tier 1 三種網路系列**，再搭配 AS3、AN4、AN5 三代 AMD EPYC 硬體平台。換句話說，你不是只選「一台美國 VPS」，而是在選「美國位置 + 網路 + 硬體」。

下面把目前公開價格、套餐、限制、退款規則和近期使用者回饋一次整理。

## 美國雲端主機到底要看什麼？

先別急著看 CPU 數字。

### 1. 先看美國哪個位置

如果服務主要給美國客戶使用，伺服器離目標使用者越近通常越容易得到較低延遲；但如果你同時服務亞洲，尤其是跨太平洋流量，洛杉磯這類西岸節點又會變得有吸引力。

DMIT 目前在洛杉磯部署於 CoreSite 與 Digital Realty 兩個資料中心，官方稱這兩個站點整合在同一套 DMIT 網路中，並提供最高 3.8Tbps 對主要 Tier 1 網路的聚合連線，以及通往中國電信、中國聯通、中國移動國際的高容量互連。這些是基礎設施條件，不代表每個使用者在任何時段都會得到同樣的延遲或吞吐量。

### 2. 再看網路系列

DMIT 把 LAX 網路分成三種。

**Premium Network** 使用包含 China Telecom CN2 GIA 在內的高階路由，定位是中國大陸與亞太使用者的低延遲、低丟包場景。官方公開資料將企業網站、跨境應用、影音、遊戲等列為適用案例。

**Eyeball Network** 則走 CMIN2 與其他中國 residential eyeball 網路，介於 Premium 與純 Tier 1 之間，定位比較偏向混合中國／全球使用者、API、SaaS、下載鏡像與遠端開發。

**Tier 1 Network** 不做針對中國大陸的特殊路由優化，重點是北美、亞太與全球的一般連線，官方把它定位在備份、CI/CD、監控、VPN、Proxy 和一般運算等情境。

因此，「哪個網路比較好」不是一個很有用的問題。你真正該問的是：**你的流量從哪裡來、要到哪裡去？**

### 3. 最後才是硬體世代

DMIT 目前在 LAX 公開列出三個硬體平台：

* **AN5**：AMD EPYC 9005、Zen 5，官方定位為高效能平台。

* **AN4**：AMD EPYC 9004、Zen 4，定位為一般用途與穩定運算。

* **AS3**：AMD EPYC 7003、Zen 3，定位為較低成本的入門與測試用途。

這裡有個容易被忽略的細節：硬體新不代表一定適合你的工作負載。單純跑一個小網站或 WireGuard 節點，花較多錢追求更新世代 CPU 未必有必要；反過來說，如果你的應用比較吃 CPU 或需要較高記憶體容量，硬體差異就會放大。

---

## DMIT 美國雲端主機目前價格怎麼看？

DMIT 現行價格頁的 LAX 方案很多，而且不是所有硬體與網路組合都完整交叉存在。

目前公開資料可看到：

* LAX Premium：AS3、AN4、AN5
* LAX Eyeball：AS3、AN4、AN5
* LAX Tier 1：AS3，以及 AN5 的 Volume / General
* 多數常規價格以月付展示
* LAX AS3 Tier 1 的 WEE 另有 **US$36.90/年** 的公開價格

官方同時提醒，產品與價格表可能因調整而沒有即時更新，所以結帳前仍應再次確認價格與庫存。

### 全套餐對比表

以下以目前 DMIT 洛杉磯公開定價頁能讀到的所有 LAX 雲端方案整理。價格均為 **USD**；「售罄」表示目前公開頁面顯示 Out of Stock。

| 網路      | 硬體          | 套餐      | vCPU |  RAM |   SSD |                 流量 |   Port |         價格 | 狀態 | 購買                                                           |
| ------- | ----------- | ------- | ---: | ---: | ----: | -----------------: | -----: | ---------: | -- | ------------------------------------------------------------ |
| Premium | AS3         | TINY    |    1 |  2GB |  20GB |                1TB |  1Gbps |   $10.90/月 | 可購 | [👉 查看 TINY](https://bit.ly/DmiT)          |
| Premium | AS3         | Pocket  |    2 |  2GB |  40GB |              1.5TB |  4Gbps |   $16.90/月 | 可購 | [👉 查看 Pocket](https://bit.ly/DmiT)        |
| Premium | AS3         | STARTER |    2 |  2GB |  80GB |                3TB | 10Gbps |   $34.90/月 | 可購 | [👉 查看 STARTER](https://bit.ly/DmiT)       |
| Premium | AS3         | MINI    |    4 |  4GB |  80GB |                5TB | 10Gbps |   $62.90/月 | 可購 | [👉 查看 MINI](https://bit.ly/DmiT)          |
| Premium | AS3         | MICRO   |    4 |  4GB | 160GB |                7TB | 10Gbps |   $87.90/月 | 可購 | [👉 查看 MICRO](https://bit.ly/DmiT)         |
| Premium | AS3         | MEDIUM  |    6 |  8GB | 160GB |               15TB | 10Gbps |  $199.90/月 | 可購 | [👉 查看 MEDIUM](https://bit.ly/DmiT)        |
| Premium | AN4         | MINI    |    4 |  4GB |  80GB |                5TB | 10Gbps |   $72.90/月 | 售罄 | [👉 查看 AN4 MINI](https://bit.ly/DmiT)      |
| Premium | AN4         | MICRO   |    4 |  4GB | 160GB |                7TB | 10Gbps |  $102.90/月 | 售罄 | [👉 查看 AN4 MICRO](https://bit.ly/DmiT)     |
| Premium | AN4         | MEDIUM  |    6 |  8GB | 160GB |               15TB | 10Gbps |  $239.90/月 | 售罄 | [👉 查看 AN4 MEDIUM](https://bit.ly/DmiT)    |
| Premium | AN4         | LARGE   |    8 | 16GB | 320GB |               25TB | 10Gbps |  $459.90/月 | 售罄 | [👉 查看 AN4 LARGE](https://bit.ly/DmiT)     |
| Premium | AN4         | GIANT   |   12 | 24GB | 640GB |               50TB | 10Gbps |  $929.90/月 | 售罄 | [👉 查看 AN4 GIANT](https://bit.ly/DmiT)     |
| Premium | AN5         | MINI    |    4 |  4GB |  80GB |                5TB | 10Gbps |   $79.90/月 | 可購 | [👉 查看 AN5 MINI](https://bit.ly/DmiT)      |
| Premium | AN5         | MICRO   |    4 |  4GB | 160GB |                7TB | 10Gbps |  $110.90/月 | 可購 | [👉 查看 AN5 MICRO](https://bit.ly/DmiT)     |
| Premium | AN5         | MEDIUM  |    6 |  8GB | 160GB |               15TB | 10Gbps |  $289.90/月 | 可購 | [👉 查看 AN5 MEDIUM](https://bit.ly/DmiT)    |
| Premium | AN5         | LARGE   |    8 | 16GB | 320GB |               25TB | 10Gbps |  $499.90/月 | 可購 | [👉 查看 AN5 LARGE](https://bit.ly/DmiT)     |
| Premium | AN5         | GIANT   |   12 | 24GB | 640GB |               50TB | 10Gbps | $1009.90/月 | 可購 | [👉 查看 AN5 GIANT](https://bit.ly/DmiT)     |
| Eyeball | AS3         | TINY    |    1 |  2GB |  20GB |              1.5TB |  2Gbps |   $10.90/月 | 可購 | [👉 查看 EB TINY](https://bit.ly/DmiT)       |
| Eyeball | AS3         | Pocket  |    2 |  2GB |  40GB |                3TB |  4Gbps |   $16.90/月 | 可購 | [👉 查看 EB Pocket](https://bit.ly/DmiT)     |
| Eyeball | AS3         | STARTER |    2 |  2GB |  80GB |                5TB | 10Gbps |   $34.90/月 | 可購 | [👉 查看 EB STARTER](https://bit.ly/DmiT)    |
| Eyeball | AS3         | MINI    |    4 |  4GB |  80GB |               10TB | 10Gbps |   $62.90/月 | 可購 | [👉 查看 EB MINI](https://bit.ly/DmiT)       |
| Eyeball | AS3         | MICRO   |    4 |  4GB | 160GB |               14TB | 10Gbps |   $87.90/月 | 可購 | [👉 查看 EB MICRO](https://bit.ly/DmiT)      |
| Eyeball | AS3         | MEDIUM  |    6 |  8GB | 160GB |               30TB | 10Gbps |  $199.90/月 | 可購 | [👉 查看 EB MEDIUM](https://bit.ly/DmiT)     |
| Eyeball | AN4         | MINI    |    4 |  4GB |  80GB |               10TB | 10Gbps |   $72.90/月 | 售罄 | [👉 查看 AN4 EB MINI](https://bit.ly/DmiT)   |
| Eyeball | AN4         | MICRO   |    4 |  4GB | 160GB |               14TB | 10Gbps |  $102.90/月 | 售罄 | [👉 查看 AN4 EB MICRO](https://bit.ly/DmiT)  |
| Eyeball | AN4         | MEDIUM  |    6 |  8GB | 160GB |               30TB | 10Gbps |  $239.90/月 | 售罄 | [👉 查看 AN4 EB MEDIUM](https://bit.ly/DmiT) |
| Eyeball | AN4         | LARGE   |    8 | 16GB | 320GB |               50TB | 10Gbps |  $459.90/月 | 售罄 | [👉 查看 AN4 EB LARGE](https://bit.ly/DmiT)  |
| Eyeball | AN4         | GIANT   |   12 | 24GB | 640GB |              100TB | 10Gbps |  $929.90/月 | 售罄 | [👉 查看 AN4 EB GIANT](https://bit.ly/DmiT)  |
| Eyeball | AN5         | MINI    |    4 |  4GB |  80GB |               10TB | 10Gbps |   $79.90/月 | 可購 | [👉 查看 AN5 EB MINI](https://bit.ly/DmiT)   |
| Eyeball | AN5         | MICRO   |    4 |  4GB | 160GB |               14TB | 10Gbps |  $110.90/月 | 可購 | [👉 查看 AN5 EB MICRO](https://bit.ly/DmiT)  |
| Eyeball | AN5         | MEDIUM  |    6 |  8GB | 160GB |               30TB | 10Gbps |  $289.90/月 | 可購 | [👉 查看 AN5 EB MEDIUM](https://bit.ly/DmiT) |
| Eyeball | AN5         | LARGE   |    8 | 16GB | 320GB |               50TB | 10Gbps |  $499.90/月 | 可購 | [👉 查看 AN5 EB LARGE](https://bit.ly/DmiT)  |
| Eyeball | AN5         | GIANT   |   12 | 24GB | 640GB |              100TB | 10Gbps | $1009.90/月 | 可購 | [👉 查看 AN5 EB GIANT](https://bit.ly/DmiT)  |
| Tier 1  | AS3         | WEE     |    1 |  1GB |  20GB |                1TB |    未標示 |   $36.90/年 | 可購 | [👉 查看 T1 WEE](https://bit.ly/DmiT)        |
| Tier 1  | AS3         | TINY    |    1 |  1GB |  20GB |                2TB |    未標示 |    $6.90/月 | 可購 | [👉 查看 T1 TINY](https://bit.ly/DmiT)       |
| Tier 1  | AS3         | STARTER |    2 |  2GB |  40GB |                4TB |    未標示 |   $12.90/月 | 可購 | [👉 查看 T1 STARTER](https://bit.ly/DmiT)    |
| Tier 1  | AS3         | MINI    |    2 |  4GB |  80GB |                8TB |    未標示 |   $21.90/月 | 可購 | [👉 查看 T1 MINI](https://bit.ly/DmiT)       |
| Tier 1  | AS3         | MICRO   |    4 |  4GB | 120GB |               16TB |    未標示 |   $32.90/月 | 可購 | [👉 查看 T1 MICRO](https://bit.ly/DmiT)      |
| Tier 1  | AN5 Volume  | V2C2G   |    2 |  2GB |  40GB |   5TB Max (IN/OUT) | 10Gbps |   $14.90/月 | 可購 | [👉 查看 V2C2G](https://bit.ly/DmiT)         |
| Tier 1  | AN5 Volume  | V2C4G   |    2 |  4GB |  80GB |  10TB Max (IN/OUT) | 10Gbps |   $23.90/月 | 可購 | [👉 查看 V2C4G](https://bit.ly/DmiT)         |
| Tier 1  | AN5 Volume  | V4C4G   |    4 |  4GB | 120GB |  20TB Max (IN/OUT) | 10Gbps |   $36.90/月 | 可購 | [👉 查看 V4C4G](https://bit.ly/DmiT)         |
| Tier 1  | AN5 Volume  | V4C8G   |    4 |  8GB | 160GB |  40TB Max (IN/OUT) | 10Gbps |   $52.90/月 | 可購 | [👉 查看 V4C8G](https://bit.ly/DmiT)         |
| Tier 1  | AN5 Volume  | V8C16G  |    8 | 16GB | 240GB |  80TB Max (IN/OUT) | 10Gbps |  $119.90/月 | 可購 | [👉 查看 V8C16G](https://bit.ly/DmiT)        |
| Tier 1  | AN5 Volume  | V12C24G |   12 | 24GB | 320GB | 160TB Max (IN/OUT) | 10Gbps |  $199.90/月 | 可購 | [👉 查看 V12C24G](https://bit.ly/DmiT)       |
| Tier 1  | AN5 General | G2C4G   |    2 |  4GB |  80GB |   4TB Max (IN/OUT) | 10Gbps |   $16.90/月 | 可購 | [👉 查看 G2C4G](https://bit.ly/DmiT)         |
| Tier 1  | AN5 General | G4C8G   |    4 |  8GB | 160GB |   8TB Max (IN/OUT) | 10Gbps |   $36.90/月 | 可購 | [👉 查看 G4C8G](https://bit.ly/DmiT)         |
| Tier 1  | AN5 General | G8C16G  |    8 | 16GB | 320GB |  12TB Max (IN/OUT) | 10Gbps |   $79.90/月 | 可購 | [👉 查看 G8C16G](https://bit.ly/DmiT)        |
| Tier 1  | AN5 General | G12C24G |   12 | 24GB | 480GB |  24TB Max (IN/OUT) | 10Gbps |  $119.90/月 | 可購 | [👉 查看 G12C24G](https://bit.ly/DmiT)       |
| Tier 1  | AN5 General | G16C32G |   16 | 32GB | 640GB |  32TB Max (IN/OUT) | 10Gbps |  $199.90/月 | 可購 | [👉 查看 G16C32G](https://bit.ly/DmiT)       |

以上價格與狀態來自 DMIT 目前公開的 LAX 定價資料；官方頁面明確說明價格表可能因調價而延遲更新，因此「頁面顯示可購」也不應被理解成永久庫存。

## 如果你只是想買一台美國 VPS，怎麼縮小選擇？

49 個公開方案看完，反而更容易讓人不知道該點哪一個。

實際上可以先把需求分成四類。

### 美國網站、API、開發環境：先看 Tier 1

假設你的使用者主要在美國、加拿大、拉丁美洲或其他不依賴中國大陸特殊路由的市場，Tier 1 比較容易對焦。

LAX.AS3.T1 TINY 目前只要 **US$6.90/月**，1 vCore、1GB RAM、20GB SSD、2TB Max（IN/OUT）；再往上一級的 STARTER 是 **US$12.90/月**，2 vCore、2GB RAM、40GB SSD、4TB Max（IN/OUT）。

這類方案適合小型網站、測試環境、CI/CD、監控、VPN 或一般 Linux 服務。DMIT 對 LAX Tier 1 的官方定位也是全球連線、亞太到美洲的低延遲路由，而不是中國大陸優化。

不過 AS3 有一個不能忽略的限制：DMIT 目前在價格頁明確警告，LAX AS3 仍在建置與優化期間，可能出現**較低磁碟效能與較低 SLA**。這不是小字註解，而是選購時應該直接算進風險的條件。

### 需要較多流量：看 AN5 Tier 1 Volume

AN5 Tier 1 的 Volume 系列比較有意思。

V2C2G 是 2 vCore、2GB RAM、40GB SSD、**5TB Max（IN/OUT）**，US$14.90/月；V4C8G 則來到 4 vCore、8GB、160GB SSD、40TB Max（IN/OUT），US$52.90/月。更高階還有 V8C16G 與 V12C24G。

如果工作負載真正吃的是流量，而不是單純 CPU，Volume 比一味往更高硬體規格升級更值得先比較。

### 要新一代硬體：看 AN5

AN5 的 LAX Premium / Eyeball 起點都不是最便宜，但硬體規格往上走時比較完整。

以 Premium 為例，MINI 為 4 vCore、4GB RAM、80GB SSD、5TB 流量、10Gbps，US$79.90/月；MICRO 是 US$110.90/月；MEDIUM 則升到 6 vCore、8GB RAM、15TB、US$289.90/月。

這裡的關鍵不是單看「AN5 比 AS3 新」，而是你是否真的需要較高的 CPU 效能或較完整的高階方案。對一個每天只有幾千訪客的網站，從低階方案直接跳到高階硬體，未必會帶來與價格差距相稱的收益。

### 使用者在中國大陸：先決定 Premium 還是 Eyeball

這是 DMIT 最有辨識度的地方。

Premium 的核心賣點是 CN2 GIA 等高階中國大陸路由；Eyeball 則偏向 CMIN2 與其他中國 eyeball 網路。官方自己也把兩者描述成不同的路由取向，而不是單純「高階版／低階版」。

所以，不要看到 Premium 三個字就直接下單。

假如你的網站大多數使用者其實在美國，偶爾才有中國流量，Tier 1 可能更合理。反過來，若主要需求就是改善跨太平洋到中國大陸的網路路徑，那麼 Premium 和 Eyeball 才是應該認真比較的兩條線。

---

## 月付與年付：目前不要把舊優惠碼當現行價格

這是搜尋美國雲端主機時很容易踩到的地方。

網路上仍能找到 DMIT 2025 年聖誕活動的優惠碼，例如 LAX Pro / EB 年付方案的折扣，以及 Tier 1 的年度折扣。不過 DMIT 的活動頁本身已明確標示 **2025 Christmas Special Promotion has ended**，並寫明優惠碼只在活動期間有效。把這些舊碼直接寫成「現在可用優惠」並不可靠。

目前公開價格頁能直接核驗到的 LAX 年付特殊價格之一，是 **LAX.AS3.T1 WEE：US$36.90/年**；其他主要 LAX 常規方案在現行公開表中主要以月付價格呈現。

因此，看到「DMIT 30% OFF」「DMIT 長期優惠碼」這類舊文章時，最好先看活動日期，不要只看文章標題。

---

## 退款政策其實很值得先看

便宜 VPS 看起來很好買，但真正會影響風險的是買錯之後能不能退出。

DMIT 目前文件寫得很清楚：新購服務在 **3 天內**，符合條件時可以申請全額退款，而且全額退款要求 VM 使用流量不超過 **30GB**；在 **30 天內**則存在按剩餘價值計算的部分退款。

同時也有幾個限制：

* 同一產品系列累計達 3 次退款後，可能不再符合退款條件。
* DDoS、IP 地理位置等情況可能落入不可退款範圍。
* 申請退款後，VM 可能會被停止，以避免繼續消耗流量。
* 確認退款後，服務資料會被刪除且無法恢復。

所以新手第一次買，不建議一上來就購買超長週期並把生產資料搬過去。先用低風險配置驗證自己的應用與網路路徑，這件事比追幾美元折扣更實際。

👉 [先查看目前可用方案](https://bit.ly/DmiT)

---

## 還有兩個容易忽略的限制：Fair Use 與 SLA

DMIT 的服務條款有 Fair Use Policy。

如果 DMIT 判斷某個服務的使用方式不符合它定義的正常、合理使用，條款允許其採取流量限速、調整到標準頻寬計價、暫停甚至終止服務等處置。這表示「標稱 10Gbps」並不等於任何使用條件下都能長時間維持 10Gbps。

條款中的 SLA 也值得留意。DMIT 目前服務條款寫明，現階段能提供的 SLA 是 **99%**；若符合適用條件並低於門檻，才涉及對應補償，而且申請 credits 還有通知時限。

對個人部落格而言，這通常不是決策核心；但如果你把美國雲端主機拿來承載付款、交易、企業 API 或其他高可用服務，就不應只看硬體價格。

---

## DMIT 的公開評價，為什麼不能只看星等？

目前 Trustpilot 上的 DMIT 頁面只有 **4 則評論**，TrustScore 顯示約 **2.6/5**，其中 3 則來自最近 12 個月；Trustpilot 自己也提醒，這個評論樣本很小，可能不具代表性。

近期公開負評的主題包括連線中斷、客服處理方式、退款爭議，以及對特定節點問題的處理速度。這些都是應該知道的風險訊號，但只有 4 則評論，不能合理地把它當成整體客戶體驗的統計結論。

這裡有個很實際的做法：不要問「DMIT 評價好不好」，改問「我的工作負載最怕哪一種問題？」

如果你最怕中國大陸方向的跨境路由問題，就應該優先確認 Premium / Eyeball 的實際路由。

如果你最怕客服處理速度，就不要只看硬體，應該先把售後風險算進去。

如果你最怕成本失控，就該把流量額度、退款政策、續費條件與 Fair Use 一起看。

---

## 從美國雲端主機的搜尋意圖來看，DMIT 適合哪些人？

如果你的需求是「我要一台離美國使用者近的 VPS，價格越低越好，而且最好可以自由選很多美國城市」，DMIT 的優勢並不在於這種市場。

目前 DMIT 的美國站點核心就是洛杉磯，而且它把資源集中在網路與跨太平洋互連。官方也明確把 LAX 描述成連接亞太與北美的重要互連位置。

但如果你的需求接近以下幾種，DMIT 的產品結構就比較有意思：

**跨美國與亞洲的網站或 API**：可以在 Tier 1 與 Premium / Eyeball 之間選擇，按照流量方向決定要不要支付中國優化的網路成本。

**需要較多流量的 VPN、Relay、下載或備份服務**：AN5 Tier 1 Volume 的 5TB、10TB、20TB、40TB、80TB、160TB Max（IN/OUT）層級比較清楚。

**想要較新 CPU 的跨境應用**：AN5 使用 EPYC 9005 / Zen 5，官方將其定位在高流量網站、資料庫與延遲敏感應用。

**測試環境或預算敏感的非關鍵服務**：AS3 Tier 1 的入門價格低，但必須接受官方目前已公開說明的成熟度與 SLA 限制。

---

## 一個比較實際的選購順序

與其從 49 個方案逐個比較，不如先把問題縮成三步。

### 第一步：先決定流量目的地

主要是美國、歐洲、拉丁美洲？先看 Tier 1。

中國大陸與亞太占比很高？再比較 Premium 與 Eyeball。

### 第二步：決定你吃的是 CPU 還是流量

流量需求高，就看 AN5 Volume。

一般用途、網站、應用服務，則比較 vCPU、RAM、SSD 是否匹配。

### 第三步：最後才看 AS3、AN4、AN5

AN5 是更新的平台；AN4 是成熟的中間層；AS3 則更偏低成本。但目前 LAX AS3 仍有官方的性能與 SLA 警告，因此不能只因為價格低就當成 AN4 / AN5 的直接替代品。

👉 [查看 LAX 美國雲端主機方案](https://bit.ly/DmiT)

---

## FAQ：買美國雲端主機前，幾個常見問題

### 美國 VPS 和美國雲端主機有什麼差別？

實際市場上這兩個詞經常混用。對一般使用者來說，比名稱更重要的是 KVM 虛擬化、vCPU、RAM、儲存、流量、Port 上限、IPv4、資料中心與網路路由。

DMIT 的 Cloud Instance 官方描述就是高效能 KVM virtual machines，並提供免費即時部署與 root access。

### 洛杉磯一定比美國東岸好嗎？

不一定。

如果使用者主要在加州、亞太，洛杉磯通常是很自然的候選位置；若主要使用者在紐約、波士頓或歐洲，東岸節點可能更符合需求。位置應該跟使用者與其他依賴服務的位置一起看，而不是只看「美國」這個國家名稱。

### 10Gbps 是不是代表我真的能跑滿 10Gbps？

不是。

DMIT 的產品頁將 Port 數字列為 VirtIO port peak speed；實際速度會受到 VM 性能、國際與本地網路等因素影響。官方舊促銷頁對這一點也有明確註記。

### 有免費退款嗎？

有條件的退款政策。新購 3 天內、VM 傳輸量不超過 30GB 時可申請全額退款；30 天內則可能適用部分退款，但仍受其他條款限制。

### 有沒有目前可以直接用的 DMIT 優惠碼？

目前能核驗到的 2025 年公開優惠活動已經結束，因此舊文章裡的促銷碼不能直接當成現行優惠。現在比較穩妥的做法，是以當下結帳頁實際顯示的價格與可用優惠為準。

---

## 結論：美國雲端主機不是先挑最低價，而是先挑對路線

「美國雲端主機」真正麻煩的地方，不是找不到便宜方案，而是便宜方案太多。

DMIT 的 LAX 產品線把差異攤得相當清楚：Tier 1 偏一般全球與美洲連線，Eyeball 偏中國 residential 路由，Premium 則把資源集中在更高階的中國大陸與亞太網路；硬體則從 AS3、AN4 到 AN5 形成不同層級。

這也代表一個很簡單的選購邏輯：

你的使用者主要在美國，就先看 Tier 1。

你的工作負載非常吃流量，就看 AN5 Tier 1 Volume。

你的服務需要中國大陸跨境連線，就比較 Premium 與 Eyeball。

你只是做測試、監控或小型服務，AS3 的低價可以看，但要把目前官方公布的性能與 SLA 限制一起算進去。

真正該避免的，不是買貴了幾美元，而是買了一台規格看起來漂亮、卻沒有對應到實際流量方向與工作負載的美國 VPS。這件事，往往比價格表上那一兩美元的差距更值得花時間確認。

👉 [從目前方案開始查看 LAX 美國雲端主機](https://bit.ly/DmiT)
