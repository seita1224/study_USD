# 大輝お勉強

## URL

[マーケット 米国債・金利](https://www.bloomberg.co.jp/markets/rates-bonds/government-bonds/us)

## 取得対象データ

- 米国債１０年
  - 利率
  - 価格
  - 利回り
  - １ヶ月利回り変化幅
  - 年間利回り変化幅
  - 更新日時

## 取得する方法について

### ブラウザスクレイピングで取得する

- main.py
  - このファイルをキックすると情報の取得が始まる(scraper.py)
  - 取得したデータをスプレッドシートとして出力する(output.py)

- scraper.py
  - ブラウザからURLを対象にアクセスする
  - ブラウザのHTMLを取得する
  - 取得してきたHTMLから取得対象データ(UsaDataModelクラス)を作成する
  - 作成したデータを返却する

- usa_data_model.py
  - UsaDataModelクラスに取得対象データを定義する
  - ゲッターセッターを作成する

- output.py
  - 入力されたデータをスプレッドシートとして出力する

## 参考URL(test)

- [【もう迷わない】Pythonでスプレッドシートに読み書きする初期設定まとめ](https://tanuhack.com/operate-spreadsheet/)
- [Selenium Python](https://www.seleniumqref.com/api/webdriver_abc_python.html)

test