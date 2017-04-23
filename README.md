# tex_gaiyo
for customized gaiyo.sty  
gaiyo.styに色々書き加えています．  

## 置き方
今までgaiyo.styを置いていたところに設置してください．
（Windowsだと， `C:\w32tex\share\texmf-local\tex\platex`かなと思います）

今までgaiyo.styの設定を書いていた部分を，以下に変更してご利用ください．

```
%\usepackage[doctor]{fireport} %博士後期課程の場合
%\usepackage[master]{fireport} %博士前期課程の場合
\usepackage{fireport} %4年次生の場合
%\usepackage[junior]{fireport} %3年次生の場合
%\usepackage[manual,presemi]{fireport} %マニュアル，プレゼミ資料の場合
%\usepackage[report,nosupervisor]{fireport} %レポートの場合
\lecture{hoge} %レポートの場合，hogeを講義名に変える
```

## 使い方
使いたい場合に応じて，上記の `\usepackage`のどれか一つの `%` を外してください．  
また，マニュアルモードの場合は `[]` 内に一緒に `presemi` を書き込むとプレゼミ資料モードになります．  
レポートモードの場合は `[]` 内に一緒に `nosupervisor` をつけると指導教員なしに設定できます．  
例）  
- 3年次生のゼミレポートの場合
```
%\usepackage[doctor]{fireport} %博士後期課程の場合
%\usepackage[master]{fireport} %博士前期課程の場合
%\usepackage{fireport} %4年次生の場合
\usepackage[junior]{fireport} %3年次生の場合
%\usepackage[manual,presemi]{fireport} %マニュアル，プレゼミ資料の場合
%\usepackage[report,nosupervisor]{fireport} %レポートの場合
\lecture{hoge} %レポートの場合，hogeを講義名に変える
```

- マニュアルを作成する場合  
マニュアルの場合は，別途最終ページの右下部に作成した版についての情報を書く欄が必要ですので，マニュアル作成用のTeXファイルをご覧ください．
```
%\usepackage[doctor]{fireport} %博士後期課程の場合
%\usepackage[master]{fireport} %博士前期課程の場合
%\usepackage{fireport} %4年次生の場合
%\usepackage[junior]{fireport} %3年次生の場合
\usepackage[manual]{fireport} %マニュアル，プレゼミ資料の場合
%\usepackage[report,nosupervisor]{fireport} %レポートの場合
\lecture{hoge} %レポートの場合，hogeを講義名に変える
```

- プレゼミ資料を作成する場合
```
%\usepackage[doctor]{fireport} %博士後期課程の場合
%\usepackage[master]{fireport} %博士前期課程の場合
%\usepackage{fireport} %4年次生の場合
%\usepackage[junior]{fireport} %3年次生の場合
\usepackage[manual,presemi]{fireport} %マニュアル，プレゼミ資料の場合
%\usepackage[report,nosupervisor]{fireport} %レポートの場合
\lecture{hoge} %レポートの場合，hogeを講義名に変える
```

- システムプログラミング実習の講義レポートを作成する場合
```
%\usepackage[doctor]{fireport} %博士後期課程の場合
%\usepackage[master]{fireport} %博士前期課程の場合
%\usepackage{fireport} %4年次生の場合
%\usepackage[junior]{fireport} %3年次生の場合
%\usepackage[manual,presemi]{fireport} %マニュアル，プレゼミ資料の場合
\usepackage[report]{fireport} %レポートの場合
\lecture{システムプログラミング実習} %レポートの場合，hogeを講義名に変える
```

- システムプログラミング実習の講義レポートを指導教員を書かずに作成する場合
```
%\usepackage[doctor]{fireport} %博士後期課程の場合
%\usepackage[master]{fireport} %博士前期課程の場合
%\usepackage{fireport} %4年次生の場合
%\usepackage[junior]{fireport} %3年次生の場合
%\usepackage[manual,presemi]{fireport} %マニュアル，プレゼミ資料の場合
\usepackage[report,nosupervisor]{fireport} %レポートの場合
\lecture{システムプログラミング実習} %レポートの場合，hogeを講義名に変える
```

