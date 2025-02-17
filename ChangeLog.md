### 2022-07-20 v1.6.10

 - 脆弱性警告に対処(terser-webpack-plugin 5.2.5 → 5.3.1)
 - 脆弱性警告に対処(jquery-ui 1.13.0 → 1.13.2)

### 2022-04-17 v1.6.9

 - #100 役牌バックのシャンテン数計算が誤っているバグを修正
 - og:image のリンクを https に修正

### 2022-03-24 v1.6.8

 - 安全牌がなくやや危険な牌を切ってオリたときに、検討モードでその牌が黄色で表示されないバグを修正
 - 脆弱性警告に対処(minimist 1.2.5 → 1.2.6)

### 2022-03-05 v1.6.7

 - #99 副露後に役を崩してしまう打牌をすることがあるバグを修正

### 2022-03-01 v1.6.6

 - 3シャンテン以前の場合、検討モードに牌の危険度レベルが表示されないバグを修正

### 2022-02-27 v1.6.5

 - 検討モードに牌の危険度レベルを表示するよう修正

### 2022-02-15 v1.6.4

 - #97 役なしテンパイから意味のないシャンテン戻しをすることがあるバグを修正
 - #96 シャンテン戻しの判定基準とする「有効牌枚数」の算出方法が誤っているバグを修正

### 2022-01-25 v1.6.3

 - #95 リーチ後に暗槓しないときがあるバグを修正
 - 脆弱性警告に対処(mocha 9.1.3 → 9.2.0)

### 2021-11-29 v1.6.2

 - 牌の危険度計算でゼロ除算が発生する可能性がある問題に対処

### 2021-11-23 v1.6.1

 - #91 三家和が発生した局の牌譜再生が誤っているバグを修正
 - HTTP2 のサーバから牌譜を取得する際にエラーメッセージが正しく表示されない問題に対処
 - webpack が LICENSE.txt を分離出力しないよう修正

## 2021-11-23 v1.6.0

 - #84 牌の危険度の計算方法を改善
 - 牌譜解析ツールを削除
 - 赤牌を識別しやすいデザインに変更
 - パッケージを最新化
   - pug 3.0.1 → 3.0.2
   - webpack 4.40.2  → 5.64.2
   - webpack-cli 3.3.9 → 4.9.1
   - mocha 8.1.1 → 9.1.3
   - stylus 0.54.8 → 0.55.0
   - jquery 3.5.1 → 3.6.0
   - jquery-ui 1.12.1 → 1.13.0
   - 脆弱性警告に対処(ansi-regex 5.0.0 → 5.0.1、path-parse 1.0.6 → 1.0.7)

### 2021-05-10 v1.5.6

 - 脆弱性警告に対処(lodash 4.17.19 → 4.17.21)

### 2021-04-20 v1.5.5

 - 脆弱性警告に対処(ssri 6.0.1 → 6.0.2)

### 2021-03-30 v1.5.4

 - 脆弱性警告に対処(y18n 4.0.0 → 4.0.1)

### 2021-03-09 v1.5.3

 - 脆弱性警告に対処(elliptic 6.5.3 → 6.5.4)
 - npm-force-resolutions で pug のバージョンを固定

### 2021-03-08 v1.5.2

 - package-lock.json の誤りを修正

### 2021-03-05 v1.5.1

 - 脆弱性警告に対処(pug 2.0.2 → 3.0.2)

## 2021-01-03 v1.5.0

 - #81 押し引きアルゴリズムの改善
   - 安全牌がない場合は押す
   - リーチに押すときにシャンテン戻しは選択しない
   - 牌姿の評価値で押し/オリを判断する
   - リーチを受けた後は愚形となる鳴きはしない
 - 牌譜操作時にスクロールキーで画面がスクロールしないよう修正
 - デバッグ用機能の改善
   - 配牌とツモを固定したデュプリケート対局ができるようにした
   - 1ファイル内に複数の牌譜が存在する形式も解析できるようにした
 - node v14 で警告が出るため stylus 0.54.7 → 0.54.8 に最新化

### 2020-12-19 v1.4.5

 - #83 牌譜ビューアで牌譜が個別に保存できないバグを修正

### 2020-12-13 v1.4.4

 - 脆弱性警告に対処(ini 1.3.5 → 1.3.8)

### 2020-09-11 v1.4.3

 - #80 和了点計算ページで赤牌をカンしての嶺上開花が指定できないバグを修正

### 2020-08-21 v1.4.2

 - #79 スマートフォン用の検討モード画面の表示タイミングを改善
 - #77 アニメーションをjQueryに依存しないようにした
 - 牌譜集計に遷移したとき右側にスクロールした状態で初期表示される問題に対処

### 2020-08-16 v1.4.1

 - 牌譜集計の表をソートできるようにした
 - 牌譜集計の際に最低対戦数を指定できるようにした
 - スマートフォンでの検討モードの表示方法を修正
 - .js、.css のファイル名にバージョン番号を付与するよう修正
 - 印刷用スタイルシートを微修正
 - 表示/非表示のアニメーションを jQuery に頼らないよう一部修正
 - serialize-javascript などの脆弱性対応のために mocha 8.0.1 → 8.1.1 に最新化

## 2020-08-08 v1.4.0

 - #73 #76 牌譜集計機能を追加
 - #74 検討モードがスマートフォンに対応
 - #75 牌譜ビューアのUIを改善
 - IE11 などの古いブラウザのサポートを停止(Babelを使用しないよう変更)
 - 天鳳牌譜変換ツールを削除
 - 牌譜のJSONファイルの形式を一部変更(point: のデータ型を数値→文字列に変更)
 - src/ 配下のソース構成を整理
 - istanbul@0.4.5 → nyc@15.1.0 に最新化

### 2020-07-30 v1.3.9

 - 脆弱性警告に対処(elliptic)

### 2020-07-17 v1.3.8

 - 脆弱性警告に対処(lodash)

### 2020-07-08 v1.3.7

 - 脆弱性対応。jquery 3.4.1 → 3.5.1、mocha 6.2.0 → 8.0.1、istanbul を最新化
 - #68 typo修正。SATRT → START
 - #69 天鳳牌譜変換の東風戦の変換が誤っているバグを修正

### 2019-10-10 v1.3.6

 - 牌画入力ツールを file: から利用しても画像が表示されるよう修正

### 2019-10-08 v1.3.5

 - 牌画のURLを変更し、HTTPSに対応した

### 2019-10-06 v1.3.4

 - #63 オーラス後の集計表から局を選択しても牌譜再生が終了してしまうバグを修正
 - 牌画入力ツールで「消去」を押下したときに入力フィールドにフォーカスするよう修正
 - ゲーム後の集計表がマウスに反応しないようにした
 - www/css/ をGitの管理外に変更

### 2019-10-03 v1.3.3

 - 全画面にバージョン番号を表示するよう修正
 - 牌譜再生のURLフラグメントのオプションに '+' の数分だけ牌譜を進める機能を追加
 - コントローラが目立つようにした
 - 視点切り替えのUIが目立つようにした
 - 使用パッケージを最新化
 - 検討モードで無駄に手牌の評価をしていた処理を削除

### 2019-09-22 v1.3.2

 - 集計表から局を選択したときにすぐに自動生成が停止しないバグを修正
 - カンが連続した場合も音声を連続して再生できるよう修正
 - Safari 13 でaudioのvolumeが調整できない問題に対処

### 2019-09-21 v1.3.1

 - 検討モード表示中に牌譜の自動再生がもたつく問題に対処
 - 牌譜を「戻し」たときに大明槓の直後では停止しないよう修正

## 2019-09-19 v1.3.0

 - #56 牌譜ビューアに「検討モード」を追加
 - #55 HTMLの部品化のために Pug を導入
 - #58 リーチがかかった状況で1シャンテンからテンパイとならない鳴きをする場合があるバグを修正
 - #60 ツモ切りでシャンテン戻しした場合の評価値計算が誤っているバグを修正
 - #59 キャッシュ上の評価値と計算した評価値が不一致となる場合があるバグを修正
 - #57 牌譜ビューアが不要なURLフラグメント更新を行わないよう修正
 - #61 IEで「何切る解答機」を使おうとすると警告を出すよう修正
 - #62 局の途中を指定して牌譜ビューアを起動したときに「前局へ」「次局へ」の機能が有効にならないバグを修正
 - URLフラグメントで、手牌表示ON/OFF、ツモ切り表示ON/OFF、分析モードON/OFF を指定できるようにした
 - スマートフォン用表示の手牌のサイズを大きくした
 - 牌譜ビューア初期表示時に画面が乱れる問題に対処
 - 牌理で5枚目の牌をツモできるバグを修正
 - Node v12 でテストが失敗するバグを修正
 - Node v12 で npm ci が失敗する問題に対処

## 2019-07-28 v1.2.0

 - #53 自動対戦のページに以下の機能を追加
   - 牌譜ダウンロード
   - 手牌表示
   - ツモ切り表示
 - 牌譜ビューアがURLフラグメントを表示するようにした
 - 牌理のページでURLフラグメントで牌姿を指定できるようにした
 - 和了点計算のページでURLフラグメントで入力を指定できるようにした
 - Home と GitHub へのリンクを追加

### 2019-07-14 v1.1.6

 - babel と mocha の使っているモジュール lodash に脆弱性がある問題に対処

### 2019-07-14 v1.1.5

 - webpack の使ってるモジュール set-value と mixin-deep に脆弱性がある問題に対処

### 2019-07-03 v1.1.4

 - 何切る解答機が評価値 0 のシャンテン戻しを表示しないよう修正

### 2019-05-29 v1.1.3

 - 何切る解答機の初期表示の乱れを修正
 - スマートフォンで音声が再生されないバグを修正

### 2019-05-21 v1.1.2

 - 長時間利用すると音声が再生されなくなる場合がある問題に対処
 - 役満和了時にドラの効果音を鳴らすようにした
 - 初回起動時に空白の画面が表示される時間が長い問題に対処

### 2019-05-13 v1.1.1

 - #52 Safariで「何切る解答機」のfragmentの指定が正しく反映されないバグを修正
 - #49 リーチ後に暗槓しない場合があるバグを修正

## 2019-05-06 v1.1.0

 - #48 「何切る解答機」のページを追加
 - #50 webpack4に対応
 - README中のブログのURLを変更
 - HTMLでファイルごとに音量を指定できるよう修正
 - スマートフォン用の表示でもナビゲーションを常に表示するよう修正

### 2019-04-21 v1.0.1

 - #47 index.html に存在しない音声ファイル Basso.wav が記述されているバグを修正
 - #46 mochaの使っているモジュールgrowlに脆弱性がある問題に対処

# 2019-04-21 v1.0.0

 - #24 Node.js 対応
   - #10 ビルドツールとして webpack、stylus を導入
   - ユニットテストを実施するために mocha、istanbul を導入
   - IEに対応するために babel を導入
 - 画面表示/UIを改善
   - ツモ切り表示をよりわかりやすくした
   - 牌譜操作のUIを充実させた
   - 牌譜の並び替えをできるようにした
 - ネット上の牌譜を読み込む機能を追加
 - 天鳳形式の牌姿文字列は廃止、電脳麻将形式に統一
 - 明槓の槓ドラめくりのタイミングを変更
 - #9 jQueryの古い書き方を修正
 - #4 牌譜再生中にカンが連続して発生した場合、音声が乱れる問題に対処
 - #44 最新のMacのChromeで見ると和了役表示の行間が空きすぎている問題に対処
 - #45 localStorageの制限を超えた場合、牌譜の削除が行えなくなる場合があるバグを修正

### 2018-09-07 v0.9.9

 - #43 未宣言の変数使用により意図しないグローバル変数を作成しているバグを修正
 - #42 喰替え時に打牌できなくなる場合があるバグを修正
 - #41 AIが牌姿を評価する時に槓ドラの増加を考慮していないバグを修正
 - #40 天鳳牌譜変換ツールの流局時の牌姿が誤っているバグを修正

### 2018-07-28 v0.9.8

 - #39 天和を地和と誤認しているバグを修正

### 2018-04-27 v0.9.7

 - #38 AIが牌姿を評価する時にキャッシュが正しく利用されない場合があるバグを修正

### 2018-02-25 v0.9.6

 - #26 人間のPlayerが立直後に大明槓できるバグを修正

### 2018-02-13 v0.9.5

 - #37 和了牌見逃し後のフリテン判断が誤っているバグを修正
 - #36 赤牌打牌時のフリテン判断が誤っているバグを修正

### 2018-02-02 v0.9.4

 - #35 ダブロンの牌譜の2つ目の和了の点数表示がおかしいバグを修正
 - #34 天鳳牌譜変換ツールで加槓と暗槓が’連続した場合の変換が誤っているバグを修正
 - #32 和了形が複数ある場合の選択方法に誤りがあるバグを修正
 - #31 九蓮宝燈の和了形判定が誤っているバグを修正
 - #33 牌画入力ツールの表示改善。"-" の直後でも重なりを解除するようにした

### 2018-01-21 v0.9.3

 - #30 天鳳牌譜変換ツールが槍槓の和了があった次の局の第一ツモを槓自摸と誤認するバグを修正

### 2017-12-19 v0.9.2

 - 天鳳牌譜変換ツールで作成する牌譜のタイトルに牌譜IDを付加できるようにした
 - 天鳳牌譜変換ツールで作成する牌譜のプレーヤー名と段位の間に改行を入れるようにした
 - 牌画入力ツールの牌画像のURLを変更
 - #29 オーラスが途中流局なのに半荘が終了する場合があるバグを修正
 - #28 三家和を途中流局と扱わない場合があるバグを修正
 - #27 リーチ一発と槍槓が複合しないバグを修正

### 2017-09-17 v0.9.1

 - #25 少牌・多牌の場合の向聴数計算が誤っているバグを修正

## 2017-08-27 v0.9

 - #19 AIが打点を意識した手作りをするようにした
 - #20 ゲーム進行速度調整の方式を変更
 - #23 牌画入力ツールが \ で次の1文字をエスケープできるようにした
 - #6 牌譜ビューアが三家和を正しく表示できるようにした

### 2017-07-30 v0.8.8

 - AIが副露後に打牌しない場合があるバグを修正
 - 天鳳牌譜変換ツールを提供
 - README.md を初期登録

### 2017-07-22 v0.8.7

 - 孤立牌の評価に赤牌でターツができる場合の考慮を加えた
 - 字牌がドラの場合の孤立牌の評価値が誤っているバグを修正
 - 喰替え時に打牌できなくなる場合があるバグを修正
 - 牌画入力ツールで牌のサイズを選べるようにした
 - 牌画入力ツールで作成した加槓の牌画がFirefoxで正しく表示されないバグを修正

### 2017−01−20 v0.8.6

 - Windowsのchromeの場合、不要なスクロールバーが表示されることがあるバグを修正

### 2017-01-06 v0.8.5

 - スマートフォンの「Webアプリモード」対応をやめた

### 2017-01-05 v0.8.4

 - スマートフォンの「Webアプリモード」に対応

### 2017-01-02 v0.8.3

 - ライセンスを明確にした(MITライセンス)

### 2016-12-31 v0.8.2

 - 牌譜再生後の対局画面でポン、チー、カンなどの発声キャプションが表示されたままになるバグを修正

### 2016-12-31 v0.8.1

 - 牌譜に対局開始画面を追加した
 - スマートフォン用の表示でも牌譜リストの画面上部にナビゲーションリンクを表示するようにした
 - 保存された対局結果を削除できるようにした
 - 「ゲーム開始」→「対局開始」にボタン名を変更し、最上部に表示するようにした

## 2016-12-31 v0.8

 - 牌譜ビューアを追加
 - 牌譜再生の際に手牌表示のON/OFF、ツモ切り表示のON/OFFを選べるようにした
 - 牌譜再生の際に視点を選べるようにした
 - 牌譜再生の際に集計表をいつでも表示できるようにし、そこから局を選択できるようにした
 - ゲームの結果を10局分ブラウザに保存するようにした
 - ゲームの結果を牌譜としてダウンロードできるようにした

### 2016-12-22 v0.7.1

 - 印刷用のスタイルを追加
 - 和了画面、終局画面がはみ出したときにスクロールできるようにした

## 2016-12-21 v0.7

 - 音声出力の方法を修正
 - スマートフォンの「ホーム画面に追加」の際のアイコンを指定した
 - チー、ポンなどの発声にキャプションをつけるようにした
 - 画像ダウンロード中に "Loading" の文字を表示するようにした
 - 牌画入力ツールを追加
 - 画面右上にナビゲーションのリンクを追加
 - スマートフォン、タブレット用のCSSを追加

### 2016-12-11 v0.6.1

 - 立直後とハイテイに鳴ける牌が打牌されたときにエラーが発生するバグを修正

## 2016-12-11 v0.6

 - 鳴いて手作りできるようにした

## 2016-12-03 v0.5

 - 回し打ちを仮実装
 - 立直に対してベタオリするようにした
 - Majiang.SuanPai に赤牌の数が正しく反映されないバグを修正

### 2016-01-05 v0.4.1

 - 四風連打が正しく判定されないバグを修正

## 2016-01-01 v0.4

 - ダブロンの発声が完全に重ならないよう調整
 - 牌譜のUIの改善: shift + ↑ で配牌、shift + ↓ で和了・流局に移動できるようにした
 - 牌譜再生時に供託立直棒が表示上増えないバグを修正
 - 牌効率向上: 孤立牌の打牌を評価値にしたがうよう変更
 - 牌効率向上: 受けの枚数を論理値から実数に変更
 - 牌効率向上: 受けの種類数重視から枚数重視に変更

### 2015-12-23 v0.3.2

 - 牌譜再生時にダブロンの2人目の和了が表示されないバグを修正
 - 符計算および和了役判定の際の雀頭の扱いを変更
 - ポンでも「スジ喰替え」と判定されることがあるバグを修正

### 2015-12-21 v0.3.1

 - 単騎待ちの2符を加えていないバグを修正

## 2015−12−20 v0.3

 - 意図せずグローバル変数を作ってしまっているバグを修正
 - カーソルキーで牌譜の局の移動・打牌の戻しを行ったとき、自動再生を停止するようにした
 - ゲームの速度と音量を変更できるようにした
 - 一般手の和了形判定で、4面子1雀頭そろっていない場合も和了形としていたバグを修正
 - 満貫〜数え役満の表示上の判定方法を修正
 - 不正な牌姿のときにTypeErrorが発生するバグを修正
 - ゲームのスピード調整の方法を微修整
 - 牌譜再生機能を追加

### 2015-12-18 v0.2.2

 - ダブロン以上のとき同時に発声するようにした
 - 暗槓に関して槓自摸と開槓の牌譜上の記録順序を変更
 - ゲームのスピード調整の方法を改善
 - 音声出力が重なったときにもたつかないように修正

### 2015-12-13 v0.2.1

 - 嶺上開花と海底摸月が複合してしまうバグを再修正
 - 手牌4枚の状態で喰替えとしかならないチーを禁止した(打牌できなくなるため)
 - 赤牌4枚使用の場合、槓できないバグを修正
 - 立直後の送り槓と待ちの変わる暗槓を禁止した
 - 喰替えを禁止した
 - 自己の4枚使いで待ち牌のない聴牌形の立直を禁止した
 - 役満のパオの得点計算に対応

## 2015-12-11 v0.2

 - jsファイルを機能ごとに分割
 - 赤牌に対応
 - ツモ切りを識別できるようにした

# 2015-12-10 v0.1

 - 初期リリース
