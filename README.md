# cow_management (乳牛管理ソフト)
+ 乳牛の体調をモニタリングすることで、発情兆候の早期発見や、牧場特有の疾病の発見に繋げることで、分娩間隔の適正化や疾病の減少、乳牛の生産性を向上させるためのソフト。  
+ また、日々の管理だけではなく、年次データを集積することで、遺伝的改良方向の検討、疾病数の増減状況の確認、対策などに利用する。
+ さらに、発情予定日の警告自動化、特定疾病の増加自動アラートにより早期対策を行い、生産性の減少防止に役立てる。
<br>  

## プログラム仕様
+ office2003-エクセルVBAで作成  
+ office2016での動作未確認  
+ データの保存方法は、RDBの考え方で、各シートを一つのテーブルと見立てて、シートごとに関連データを保存。
+ データの入出力・確認は、別途作成したウィンドウで行う。
<br>  
  
## 画面構成  
<br>

### ー 個体管理画面トップ ー  
  
![flddiinefeldfppi](https://user-images.githubusercontent.com/61402011/86435738-a6f4c280-bd3b-11ea-8ec4-0a290664c6a6.png)  
+ 各乳牛の基本情報入力・確認画面
  + 乳牛精液NO、母牛耳標識NOを入力することで系統的な遺伝的特徴の把握に繋げる。
  + 下段の各タブに、「発情」「受精」「分娩」「乳房炎」「疾病・事故」「BCS」「フェーズ」「乳量」に関する情報入力・確認欄がある。
<br>

### ー 発情管理タブ ー  

![hatuzyou](https://user-images.githubusercontent.com/61402011/86440865-31daba80-bd46-11ea-8678-02a8c7c491d9.png)  
+ 発情に関わる各種情報入力・確認欄  
  + 分娩日より、初回発情予定日を自動計算し、本日の予定ページにて通知する。
  + 発情日を入力後、次回発情予定日を自動計算し、本日の予定ページにて通知する。
  + 発情周期データを蓄積することで、健康状態の把握、遺伝的な発情力の把握につなげ、飼養管理に活かす。
<br>

### ー 授精管理タブ ー  
  
![zyusei](https://user-images.githubusercontent.com/61402011/86441330-ff7d8d00-bd46-11ea-8784-3398280cdd2c.png)  
+ 授精に関わる各種情報入力・確認欄
  + 精液Noを記録し続けることで、牛毎の授精適性の把握に繋げる。  
<br>

### ー 分娩管理タブ ー  
  
![bunben](https://user-images.githubusercontent.com/61402011/86441964-f7721d00-bd47-11ea-9569-f3ee4c805730.png)  
+ 分娩に関わる各種情報入力・確認欄
  + 分娩難易度を牛毎・産次に記録することで、時系列での分娩状況の改善状況を把握する。
  + 後産状況の記録により、後産が出やすくなっててきいるか、種的に出づらい系統か確認する。
  + 初乳比重の記録により、乾乳期の管理状況の良し悪しに繋げる。  
<br>  
  
### ー 乳房炎管理タブ ー  

![nyubouen](https://user-images.githubusercontent.com/61402011/86444137-479eae80-bd4b-11ea-87d0-fe2c56fff42e.png)  
+ 乳房炎に関わる各種情報入力・確認欄
  + 原因菌を記録することで、牧場内で発生しやすい菌を特定し、対策に役立てる。
  + 損失乳量は、乳量タブのデータより自動計算される。  
<br>

### ー 疾病・事故管理タブ ー  
    
![sippei](https://user-images.githubusercontent.com/61402011/86447209-f8a74800-bd4f-11ea-98d7-f26ee05c6fd1.png)  
+ 疾病・事故に関わる各種情報入力・確認欄
  + 疾病は、乳房炎以外の病気について記録する。
  + 事故データにより、牛舎内での滑りやすい位置などの問題点を発見し、牛舎環境の改善に繋げる。
<br>  
  
### ー BCS管理タブ ー  

![bcs](https://user-images.githubusercontent.com/61402011/86447816-d6fa9080-bd50-11ea-8e3d-847946d90921.png)  
+ BCS(ボディコンディションスコアリング)に関わる各種情報入力・確認欄
  + 各フェーズ毎のBCSを記録することで、フェーズ毎の飼養管理が適切に行われているか確認する。
  + BCSチェック日は、分娩月日より自動計算される。
<br>  
  
### ー フェーズ管理タブ ー  

![fase](https://user-images.githubusercontent.com/61402011/86448378-a49d6300-bd51-11ea-9d26-ac154b8d12b4.png)  
+ フェーズ移行日入力・予定日確認欄
  + 分娩月日より各フェーズ移行日を自動計算し、予定日１週間前より通知。
  + 通知に合わせ、餌を徐々に切り替える。
<br>  
  
### ー 乳量管理タブ ー

![nyuryo](https://user-images.githubusercontent.com/61402011/86449436-280b8400-bd53-11ea-981a-73ba9a2412dd.png)  
+ 乳量データ入力・確認欄
  + 乳検乳量データを入力する。
  + 年次データを蓄積することで、牛ごとの乳量増加量を確認し、遺伝性やボディコンディションの管理に役立てる。
<br>  
  
### ー 日常管理項目通知画面 ー  

![notice_screen](https://user-images.githubusercontent.com/61402011/86449791-a0724500-bd53-11ea-914e-5a4448981181.png)
+ その日のチェック項目とチェック対象牛を通知する画面。
  + 毎朝画面を確認することで、チェック対象牛を漏れなくチェックできるようにする。
<br>

## 備考
+ ソフト利用対象牧場サイズ：成牛80頭程度まで。（100頭超えると、日々の入力作業に時間を取られるので、別スタッフが必要になりそう。）







