---
tags: sumitomo, 2252, alphv, vaupell, 
comments: 
---

# 住友ベークライトの海外拠点のインシデント

- 2022-12-01: [住友ベークライト株式会社 | 当社の米国グループ会社に対するサイバー攻撃について](https://www.sumibe.co.jp/topics/2022/pdf/1201_01.pdf)
  > 当社の米国グループ会社がサイバー攻撃を受けた（以下、「本件事案」といいます。）ことが  
判明しました。米国グループ会社は、本件事案の発生を確認後、外部の専門家の協力を得て速  
やかに対応を開始し、本件事案の内容や影響範囲等について調査を進めております。
## ランサムウェア被害
-  
## リークサイト掲載状況
- Alphvリークサイト `http://alphvmmm27o3abo3r2mlmjrpdmzle3rykajqc5xsj7j7ejksbpsa36ad.onion/b4a61f4f-dfc9-4c79-8321-270440b4b43a`
- ALPHV Collections (窃取データ（の一部？）を確認できる別サイト)　`http://kqpmhriaqt4kujfnm3wv7ujgzx5pujqqd4logzgzzq3w5wctm62c5uid.onion/search?text=SUMITOMO`
	- `SUMITOMO` 検索で約1万点のファイルがヒットする
	- 検索結果として並ぶファイル名は`Vaupell` 関連が多い様子 (`https://www.vaupell.com/news/` に該当プレスリリースは無い状況)
		- Vaupell Holdings , Inc. は住友ベークライトが2014年に買収した企業
## 被害組織のダミーサイトを作り（窃取データを載せる？）サーフェスWebへ公開する手口
- [Brett Callow: "A #ransomware gang has created…" - Infosec Exchange](https://infosec.exchange/@brett/109587244356725180)
- [Ransomware gang cloned victim’s website to leak stolen data](https://www.bleepingcomputer.com/news/security/ransomware-gang-cloned-victim-s-website-to-leak-stolen-data/)
- タイポスクワッティングで似たようなドメイン名を用いているとのこと
### Vaupellドメインについてタイポスクワッティング狙いの取得状況
- Domain Typosサイトで確認→ 類似名は8件ヒット、`vaudell.com` が2022年8月に取得されており、同名企業は存在しない。WebサイトはZohoのサイトビルダーの初期？状態にみえる（[www.vaudell.com - urlscan.io](https://urlscan.io/result/78f129c5-b06f-4546-87f1-961427a4a23f/)）  
- [VaUdell.com WHOIS, DNS, & Domain Info - DomainTools](https://whois.domaintools.com/vaudell.com)
  > Domain Name: VAUDELL.COM  
Registry Domain ID: 2719195964_DOMAIN_COM-VRSN  
Registrar WHOIS Server: whois.tucows.com  
Registrar URL: http://tucowsdomains.com  
Updated Date: 2022-08-25T05:54:09  
Creation Date: 2022-08-18T23:41:50  
Registrar Registration Expiration Date: 2023-08-18T23:41:50  
Registrar: TUCOWS, INC.  
Registrar IANA ID: 69  
Reseller: Zoho  

- ほか、2022年6月に取得されている`VauPeli.com`も、Webサイトは無い状況、同名企業は無く注視

