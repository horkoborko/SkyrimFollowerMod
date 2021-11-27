Lazy Voice Finder - Fidn voice assets just you want
Version 1.3.7
by BowmoreLover

Official Sites:
- NexusMods Oblivion http://www.nexusmods.com/oblivion/mods/47801/
- NexusMods Fallout 3 http://www.nexusmods.com/fallout3/mods/22552/
- NexusMods Fallout New Vegas http://www.nexusmods.com/newvegas/mods/63317/
- NexusMods Skyrim http://www.nexusmods.com/skyrim/mods/82482/
- NexusMods Skyrim Special Edition http://www.nexusmods.com/skyrimspecialedition/mods/8619/
- NexusMods Fallout 4 http://www.nexusmods.com/fallout4/mods/24309/

Supporters Sites:
- Gamer Mods (Russian) http://gamer-mods.ru/load/tes_v_skyrim/instrumentarij/lazy_voice_finder/59-1-0-5701
- Skyrim Mod Database (Japanese) http://skyrim.2game.info/detail.php?id=82482
- Skyrim Special Edition Mod Database (Japanese) http://skyrimspecialedition.2game.info/detail.php?id=8619
- Fallout4 Mod Database (Japanese) http://fallout4.2game.info/detail.php?id=24309

===================================================================================================================
目次

1. はじめに
2. 制作動機と目的
3. 主要機能
4. 前提条件
5. インストール
6. アンインストール
7. 基本的な使い方
8. 注意/制限事項/既知の問題
9. 今後の計画
10. その他公開中のツールについて
11. クレジット

===================================================================================================================
 1. はじめに
===================================================================================================================

音声ファイルを扱うMOD制作者/翻訳者向けのツールです。
バニラ/MODの音声ファイルの一覧を表示して、対話テキストなどの様々な条件で検索できます。
事前にBSA/BA2/FUZを展開しておかなくても音声ファイルを直接再生/編集(*1)/展開できます。
Oblivion/FO3/FNV/Skyrim LE/Skyrim SE/FO4に対応しています。もちろんSkyrim SEの新BSA形式やFallout 4のBA2形式に対応しています。

主な用途は次のとおりです。
- カスタム音声を編集するためにバニラ/MODの音声ファイルを見つける。
- あなた自身のカスタムボイスmodから不要な(余分な)/不足の音声ファイルをチェックする。
- ただ対話と音声を楽しむ。バニラには未使用の隠された対話や音声があるので、これを見つけるのも楽しいでしょう。

これがあなたの助けになることを願っています。

(*1)一時フォルダに展開して編集しますので、DataフォルダやBSA/BS2ファイル内の音声ファイルを直接編集して更新することはできません。

=========================================================
&nbspOblivion/Fallout3/Fallout NVコミュニティへのご挨拶
=========================================================

このツールを新たなコミュニティに公開できてとても嬉しく思います。
元々このツールはSkyrim用に開発したものです。他のベゼスダゲームでもきっと便利だと思ったので、Oblivion/FO3/FNVをサポートすることにしました。
Oblivionはかなり昔にプレイしましたが最近のモッディング状況は分かりませんし、FO3/FNVはまだプレイしていません。何かおかしい所があるはずですので、遠慮なく指摘してください。


===================================================================================================================
 2. 制作動機と目的
===================================================================================================================

最近バニラ音声を使ったスカイリムのMOD音声の日本語化をしました（Skyrim用MOD Minerva - Custom High Elf Voiced Follower (http://www.nexusmods.com/skyrim/mods/74256/) by cloudedtruth and rxkx22 など）。
この作業で一番大変なのはバニラ音声から必要なものを見つけ出すことです。
この手の作業にはgreentea101さんのVoice File Reference Tool (http://www.nexusmods.com/skyrim/mods/28462/) がかなり便利で、対話テキストから音声ファイル名を見つけることができます。
しかし、音声ファイルを扱うためにはBSAファイルを展開して音声ファイルを見つける必要があります。それに事前にツール用の辞書の作成も必要ですし、バニラ音声以外を探すこともできません。
このツールは以上の課題解決を試みます。

とはいえ、greentea101さんのツールはとても便利なものでしたし、このツール開発の大きなきっかけを与えてくれました。本当にありがとう！

追記:
このツールのリリース後、FO4 Voice File Reference Tool (http://www.nexusmods.com/fallout4/mods/12132/) が既にリリースされていてba2/fuzからの音声再生/展開ができることを知りました。すごい！ あなたがFO4のモッダーでバニラ/DLCからの検索ができれば十分ならVFRTが最高のチョイスです。これ知っていればツールを開発しなかったかもしれませんが、時すでに遅しです。
VFRTと本ツールのコンセプトを大きく異なります。VFRTは辞書ファイルによる高速検索と使いやすさがウリですが、あらゆるプラグインを即座に開けるわけではありません。本ツールはあらゆるプラグインを開けますが、検索性能はさほどでもなく少し複雑です。
どんなツールにも言えることですが、用途に応じていろんなツールを使い分けることが重要です。


===================================================================================================================
 3. 主要機能
===================================================================================================================

サポートするゲーム:
- Oblivion
- Fallout 3
- Fallout New Vegas
- Skyrim Legacy Edition (Skyrim LE)
- Skyrim Special Edition (Skyrim SE)
- Fallout 4
- Fallout 76 (実験的)

多言語サポート:
- UIの言語:
  - 英語
  - 日本語
  - ロシア語  (翻訳者 anizorda http://gamer-mods.ru/index/8-16387)

  UI翻訳リソースファイルが利用可能になりました (Miscセクションにあります) : http://www.nexusmods.com/skyrim/mods/82482/?
  リソースファイルを自由に翻訳して再配布できます (依然メインファイルは再配布不可な点に注意してください)。
  翻訳ファイルを私（作者）に送っていただければ幸いです。メインファイルにバンドルして翻訳者の名前をクレジットさせていただきます。

- プラグインの言語 (リクエスト歓迎):
  Arabic, Baltic, Chinese, Czech, Danish, English, Finnish, French, German, Greek, Hebrew,
  Hungarian, Italian, Japanese, Korean, Norwegian, Polish, Portuguese, Russian, Spanish(Spain/Mexico), 
  Swedish, Thai, Turkish, Vietnamese
  言語メニューの"カスタム"から任意の言語やコードページが選べます。
  Data/GameLang_*.txtで任意の言語やコードページを追加することもできます。ファイル内のコメントを参照してください。

- Oblivion/FO3/FNVユーザーへの注意事項
  - Oblivion/FO3/FNVは多言語をサポートしていませんので、一度に表示できる言語は一つだけです。
  - Oblivion/FO3/FNVの公式ローカライズ言語はごくわずかであり、他の言語へのローカライズにはMODを使います。しかしながらどの言語にローカライズされているのか、各言語でどのコードページが使われているのか分かっていません。ですのでローカライズ用MODをお使いの場合、MODに合わせてData/GameLang_*.txt中のコードページを変更する必要があります。私はこの種の情報にとても興味があるので、教えていただけると幸いです。

サポートする音声ファイル形式：
- Oblivion: mp3/lip
- Fallout 3/Fallout NV: ogg/lip
- Skyrim LE/Skyrim SE/Fallout 4/Fallout 76: fuz/xwm/wav/lip

プラグインの選択:
- ゲームのプラグイン一覧からプラグインを選んでロードできます。
- Dataフォルダ以外のプラグインをロードできます。ドラッグ＆ドロップでプラグインファイルをロードすることもできます。
  開くプラグインの種類によってゲームモードを自動的に選択するオプションもあります。

便利なスプレッドシート:
- ExcelやOpenOfficeと同様に次の操作が行えます:
  - ソート
  - テキストや項目チェックによるフィルタリング
  - 列の表示/非表示
  - 列位置の変更
- 表の列は次とおり。どの列も好みに合わせて表示/非表示できます:
  - State : 以下の情報/警告。アイコン表示ですがツールチップでテキスト表示できます。
    - ファイル名不正 : 規定外の音声ファイル名
    - パス名不正 : 規定外の音声ファイルパス
    - オーバーライド : ゲームエンジンの規則に従って同名の音声ファイルでオーバーライドされた
    - 対話なし : 対応する対話応答レコード(INFO)がない
    - テキストなし : STRINGSファイル中に対話テキストがない（レアケース）
    - Stringsファイルなし : ローカライズされたプラグインのSTRINGSファイルがない
    - 音声ファイルなし : 対話応答レコード(INFO)に対応する音声ファイルがない
    - マスターレコード参照 : マスタープラグインの対話応答レコード(INFO)を参照している
  - Index : プラグインのロード順
  - Plugin : プラグイン名
  - Last Modifier : 対話返答レコード(INFO)の最終更新プラグイン名
  - FormId : 対話返答レコード(INFO)のForm Id - ロード順は含まない（つまり常に"00"で始まる）
  - Response Num : 対話返答レコード(INFO)の返答番号
  - Edid : 対話返答レコード(INFO)のエディタID
  - Topic FormId : 対話トピックレコード(DIAL)のForm Id
  - Topic Edid : 対話トピックレコード(DIAL)のエディタID
  - Topic Text : 対話トピックレコード(DIAL)のテキスト
  - Quest FormId : 関連付けられたクエストのForm Id
  - Quest Edid : 関連付けられたクエストのエディタID
  - Quest Name : 関連付けられたクエストの名前
  - Category/Subtype
    - 対話分類 : Topic/Favor/Scene/Combat/Favors/Detection/Service/Misc/etc...
    - 対話サブタイプ (DIAL:SNAM) : Attack/PowerAttack/Hello/Goodbye/etc... (TES4/FO3/FNVでは空白)
  - Emotion : 感情 - Neutral/Anger/Disgust/Fear/Sad/Happy/Surprise/Puzzledなど
  - Conditions : 対話返答レコード(INFO)の条件判定。NPC/場所/プレイヤー性別条件が表示されますが不完全です。
  - Bsa Name : 音声ファイルが格納されたBSA/BA2ファイル名 または "Loose"
  - Full Path : 音声ファイルのフルパス
  - Base Path : DataフォルダまたはBSA/BA2ファイルのフルパス
  - Path : Dataフォルダからの相対パス
  - File Name : 音声ファイル名
  - Extensions : 音声ファイルの拡張子 - fuz/xwm/wav/lip/ogg/mp3
  - Voice Type : ボイスタイプ
  - Script Notes : 台詞メモ (INFO:NAM2)。このテキストはローカライズされず英語のままとなります。
  - Edits : 補足 (INFO:NAM3)。このテキストはローカライズされず英語のままとなります。
  - Prompt : 対話のプロンプト (INFO:RNAM)。Skyrimで言う'Prompt override'です。FO4の対話選択肢ではTopic Text (DIAL:FULL)はあまり使われず、Promptに置き換わったようです。FO4ではTopic Text列の代わりにPrompt列を使ってください。
  - Dialogue 1 : 対話テキスト。設定ダイアログで言語の選択が可能
  - Dialogue 2 : 対話テキスト（オプション）。設定ダイアログで言語の選択が可能
  - Keyword : Fallout 4/Fallout 76でのみ有効。AO_Comment, CAT_CustomEvent, CAT_Eventといったキーワード (DIAL:KNAMレコード、コンパニオンに対して特定の状況を示すキーワードを提供する仕組み)
  - StringId : 対話テキストのString Id

音声ファイルの検索:
- 検索対象:
  - 対話テキスト
  - Form Id
  - Edid
  - ファイル名
- 検索モード:
  - 部分一致
  - 正規表現
  - AND検索 : 空白で区切られたテキストのAND条件で検索します。空白を含むテキストを指定する場合は引用符(")で囲みます。
  - OR検索 : 空白で区切られたテキストのOR条件で検索します。空白を含むテキストを指定する場合は引用符(")で囲みます。
  - 前方一致
  - 後方一致
  - 完全一致
- 検索オプション:
  - 大文字と小文字を区別
  - ワード単位 : 例えば、"bye"で検索しても"Goodbye"がヒットしないようにできます。
  - Migemo検索 : ローマ字や英単語で日本語の対話が検索できます。詳細は「7. 基本的な使い方」の「Migemoの使い方」を参照してください。
- テキスト検索ボックスのオートコンプリートに対応。検索対象列の実データに基づいてオートコンプリートされます。このオプションはオプションメニューで切り替えられます。
- 検索履歴を最大40個まで保存。テキスト検索ボックスのドロップダウンから呼び出せます。

音声ファイルの操作:
  - サウンドの再生。Pauseキーまたはツールボタンで再生を中止できます。
  - サウンドの編集 : Audacity (またはほかのサウンドエディタ) で音声ファイルを編集
    ファイルを対話テキストでリネームして編集することもできます。このオプションは設定ダイアログで有効化にできます。
  - 展開したフォルダを開く : 音声ファイルを一時フォルダに展開/コピーして開く。FUZ/XWM/MP3/OGGファイルはWAVファイルに変換される。LIPファイルも一緒に展開/コピー可能
    ファイルを対話テキストでリネームして展開することもできます。このオプションは設定ダイアログで有効化にできます。
- "元のフォルダを開く" : 音声ファイルのあるフォルダを開きます。BSA/BA2ファイルに格納されている場合はBSA/BA2ファイルのフォルダを開きます。
- "音声ファイルをコピー" : 音声ファイルをクリップボードにコピーします。LIPファイルがあれば一緒にコピーします。
- "音声ファイルをWAV形式でコピー" : 音声ファイルをWAV形式でクリップボードにコピーします。LIPファイルは一緒にコピーされません。
- "音声ファイルをクリップボード内名称でコピー" : 音声ファイルをクリップボード内のテキストでリネームしてクリップボードにコピーします。LIPファイルがあれば一緒にコピーします。
- "選択したテキストをコピー" : 選択されたセル内のテキストをクリップボードにコピーします。複数選択に対応しています。
- "選択行のファイル名をコピー" : 選択された行の音声ファイル名をクリップボードにコピーします。複数選択に対応しています。
- "選択行のアセットパスをコピー" : 選択された行の音声ファイルのアセットパスをクリップボードにコピーします。複数選択に対応しています。
- "選択行のファイルをエクスポート" : 選択された行の音声ファイルを"<インストールフォルダ>/Export"フォルダにエクスポートします。ファイルは常に上書きされます。エクスポート処理は'Pause'キーでキャンセル可能。大量のエクスポートは想定外のため、Yakitori Audio Converterなどその他のツールを利用のこと。

クリップボードで検索:
- クリップボードにコピーされたテキストで自動検索します。このオプションはオプションメニューで切り替えられます。
- xEdit や xTranslator と一緒に使う際に便利かもしれません。
- 検索対象はテキストの形式によって次のように自動的に切り替わります:
  - Form Idで始まる場合 :Form Id
  - '[]' で囲まれたForm Idで始まる場合 : Form Id
  - '<>' で囲まれたEditor Idの場合 : Edid
  - 音声ファイルの拡張子で終わる場合 : File Name
  - その他の場合 : Dialogue 1 または Dialogue2 (最後に選んだもの)

その他の機能:
- 行の高さが変更できます : 自動 / 1～5行
- オプションメニューでツールのウィンドウを最前面に固定できます。
- オプションメニューで列をウィンドウ幅に収めるかどうかを選択できます。
- 現在表示されているレコードをCSVファイルにエクスポートできます。CSVエクスポートダイアログでお使いのスプレッドシートアプリに合ったオプションを選んでください。
- "ファイル - 最近使ったファイル"メニューから、最近使ったファイルを開きなおすことができます。
- "現在のファイルをリロード"ボタンを使って現在開いているファイルをリロードすることができます。


===================================================================================================================
 4. 前提条件
===================================================================================================================

必須:
- Windows 7 or later (Windows 10でテスト済)
- Microsoft Visual C++ 再頒布可能パッケージ:
  LazyVoiceFinder.exe(64ビット版)を使う場合はx64を、LazyVoiceFinder32.exe(32ビット版)を使う場合はx86をインストールしてください。
  - Microsoft Visual C++ 2010 Redistributable Package (x86) (https://www.microsoft.com/en-us/download/details.aspx?id=5555)
  - Microsoft Visual C++ 2010 Redistributable Package (x64) (https://www.microsoft.com/en-US/download/details.aspx?id=14632)
  - Microsoft Visual C++ 2015 Redistributable Update 3 (https://www.microsoft.com/en-US/download/details.aspx?id=53587)
  - Visual C++ Redistributable for Visual Studio 2017 (https://www.visualstudio.com/downloads/)
- ゲーム本体 (Oblivion/Fallout 3/Fallout New Vegas/Skyrim LE/Skyrim SE/Fallout 4/Fallout 76, DLCはオプション)
  !!! 一度ゲームをベゼスダのランチャーで起動してください。そうしないとツールがゲームのインストールフォルダを検知できません。設定ダイアログで明示的にゲームのインストールフォルダを設定することもできます。 !!!

Windows XP/Vista/7/8でテストしていませんが、.NET Framework 4.6.1がインストールされていれば動作するはずです。

オプション:
- Audacity (http://www.audacityteam.org/)
  音声ファイルの編集に必要です。私は2.1.2を使っていますが別のバージョンでも動くはずです。
  他のサウンド編集ソフトでも動くはずですがテストしていません。

オプション(Skyrim用):
- Multiple Languages Strings Unified Central by Francisco Pozo - DJ FrANKy EHP (http://www.nexusmods.com/skyrim/mods/82578/?)
- Multiple Languages Strings Unified Central SSE by Francisco Pozo - DJ FrANKy EHP  (http://www.nexusmods.com/skyrimspecialedition/mods/4505/?)
  他の言語のstringsファイルを探しているならここで見つけられます。
  注意：stringsファイル名の一部はEnglishとなっているので、このツールで使うには適切な言語名にリネームする必要があります。

オプション(Migemo機能を使う場合):
- C/Migemo for Windows 32bit Version 1.3 (https://www.kaoriya.net/software/cmigemo/)


===================================================================================================================
 5. インストール
===================================================================================================================

ダウンロードしたファイルを任意のフォルダに展開します。
Windows/Program Files/ゲームのインストールフォルダにはインストールしないでください。

旧バージョンからアップデートする場合は、基本的には単純に上書きします。
ただし、v1.2.0でファイル構成が大きく変化しました。v1.2.0より前のバージョンからアップデートする場合はきれいなフォルダにインストールすることをお勧めします。

注意: v1.3.0より、.NET Frameworkの前提バージョンが4.6.1に変更されました。ツールが起動できない場合、前提条件に書かれたurlから.NET Frameworkをアップグレードしてください。

=== Migemo検索機能を使う場合 ===

v1.3.5で、ローマ字や英語で日本語テキストを検索するMigemo検索機能がサポートされました。
この機能を使う場合、以下の手順でC/Migemoの辞書をインストールします。
- Kaoriya.net (https://www.kaoriya.net/software/cmigemo/) からC/Migemo for Windows 32bitをダウンロードします。
- ダウンロードしたzipファイルを展開し、dictフォルダを'ツールのインストールフォルダ/Migemo'にコピーします。
- ツールを起動すると辞書の再構成が行われ、ツールバーに「み」アイコンが表示されます。


===================================================================================================================
 6. アンインストール
===================================================================================================================

フォルダごと削除します。レジストリは使っていません。


===================================================================================================================
 7. 基本的な使い方
===================================================================================================================

=== 起動＆プラグインの選択 ===

- LazyVoiceFinder.exe を起動する
  旧Mod Organizerのような32ビットプログラムから起動する場合、LazyVoiceFinder32.exeを起動する
- "オプション"-"設定メニュー"を開いて"一般"ページのUI言語を変更する
- "ゲームモード"メニューでゲームを選択 (Oblivion / Fallout 3 / Fallout NV / Skyrim LE / Skyrim SE / Fallout 4 / Fallout 76)
- "開く"ボタンを押す
- プラグインを選択する。"全解除"ボタン、"バニラ+DLC選択"ボタンを押してバニラ+DLCだけを選択できる。最後に"OK"ボタンを押す。
- 少し待つと表に音声ファイルの一覧が表示される。対応する対話レコードがあれば対話テキストなども一緒に表示される。

=== テキスト検索 ===

- テキスト検索ボックスに文字を入力して検索できる。
  デフォルトの検索対象は"Dialogue 1"。左のコンボボックスで検索対象を変更できる。

=== 音声ファイルの操作 ===

音声ファイルを操作するには表を右クリックして操作メニューを開く。

- "サウンドの再生" : 音声ファイルを再生する。
- "サウンドの編集" : 音声ファイルを編集する。メニューが選べない場合は設定ダイアログでサウンドエディタのパスを設定する。
- "展開したフォルダを開く" : 音声ファイルを一時フォルダに展開/コピーして開く。FUZ/XWM/MP3/OGGファイルはWAVファイルに変換される。LIPファイルも一緒に展開/コピーされる。
- "元のフォルダを開く" : 音声ファイルのあるフォルダを開く。BSA/BA2ファイルに入っている場合はBSA/BA2ファイルのフォルダを開く。

=== 表のソート/フィルタリング/カスタマイズ ===

ExcelやOpenOfficeと同じようなことが行える。

- ソート : 列ヘッダをクリック。クリックするたびにソート順が反転する。
- フィルタリング : 列ヘッダの矢印ボタンをクリックしてフィルタメニューを表示する。
- フィルタリング解除 : 列ヘッダを右クリックしてメニューを選ぶ。
- 列位置の変更: 列ヘッダをドラッグする。
- 列の非表示/再表示 : 列ヘッダを右クリックしてメニューを選ぶ。

== 対話の言語変更 ==

- "オプション-ゲーム毎の設定"メニューを選んで各ゲームのページを開く。対話の言語を二つまで選べる。
  言語はプラグインのロード時に反映される。
  注意: 言語を選んでも対応するSTRINGSファイルがないと正しく表示されない（英語で代用される）。

== ショートカットキーと便利な操作 ==

(メイン画面)
F5 : プラグインを開く
F9 : 全般設定
F10 : ゲーム毎の設定
Ctrl+F1 : ゲームモード - Oblviion
Ctrl+F2 : ゲームモード - Fallout 3
Ctrl+F3 : ゲームモード - Fallout New Vegas
Ctrl+F4 : ゲームモード - Skyrim Legacy Edition
Ctrl+F5 : ゲームモード - Skyrim Special Edition
Ctrl+F6 : ゲームモード - Fallout 4
Ctrl+F7 : ゲームモード - Fallout 76
ESC/F2 : テキスト検索ボックスに移動
Enter : テキスト検索
Ctrl+Enter : 検索対象 "Dialogue 1" と "Dialogue 2" を切り替えて検索
Ctrl+1 ～ Ctrl+5 : 検索対象の切り替え
Alt+N/Alt+E/Alt+A/Alt+R/Alt+P/Alt+S : 検索モードの切り替え
Alt+Down : 検索履歴の表示
Pause : 音声停止/検索の中断

(表)
右クリック/メニューキー : 音声操作メニューの表示
Enter/Space/Ctrl+P/ダブルクリック : 音声ファイルの再生（トグル）
Ctrl+E : 音声ファイルの編集
Ctrl+O : 展開したフォルダを開く
Ctrl+A : セルの全選択
Ctrl+C : セルのテキストをコピー
Ctrl+Shift+C : 音声ファイルのコピー
Alt+Up/Alt+Down : フィルタメニューの表示
左上のセルをクリック : 左上メニューの表示。フィルタの全リセットが可能

(ログ画面)
Ctrl+A : 全選択
Ctrl+C : コピー
右クリック : ログメニューの表示

== Migemo検索について ==

- ローマ字や英単語で日本語のテキストを検索できます。入力した文字をMigemo辞書と照らし合わせることで、ひらがな、カタカナ、漢字、英単語などの候補を作り出して検索する仕組みです。
- 本機能を使うには別途Migemo辞書をインストールする必要があります。インストール方法については「5. インストール」を参照してください。
- 入力した文字そのものも検索候補となるので、英語のテキストに対してMigemo検索しても問題ありませんが、検索速度は低下します。これを避けるため、Migemo検索の指定は検索対象のゲームと対話言語毎に記憶する仕組みとなっています。
- ローマ字は半角英字、ハイフン、アポストロフィで記述します。
  - 「ん」はn', nn, nのいずれかで入力： ton'nel=トンネル  hannou=反応  kanji=漢字
  - 小文字(ァ等)はl, xのどちらかと母音で入力: arudoluin=アルドゥイン   sukuxu-ma=スクゥーマ
  - 長音符はハイフン(-)で入力: suke-ru=スケール
  - 文節の区切りは英大文字とします。Migemoは厳密な日本語解析処理を行わないので、使い手が明確に文節を区切る必要があります: koreHaPenDesu = これはペンです
- Migemo検索ボタンの右クリックで2つのモードが選択できます。
  - 標準モード: 英単語の検索に向いています。半角の記号を特別あつかいせず、そのままMigemo検索します。英語の記号を含む検索ワード、例えば"Mr.Handy"で「Mr.ハンディ」を検索できます。一方で、日本語の記号「、」「。」を検索するために "Ten" "Maru"といった指定をする必要があり、日本語の検索が少し面倒です。VimやEmacs等のMigemo機能と同等の仕様です。
  - 拡張モード: ローマ字での検索に向いています。標準モードの欠点を改善し、引用符、カンマ、ピリオド等の記号を文節区切りとすることで、日本語の記号を検索しやすくします。例えば "sate, sigoto" で「さて、仕事」が検索できます。一方で、記号を含む英単語が上手く検索できない場合があります。例えば、"Mr.Handy"で「Mr.ハンディ」が検索できなくなります。
- 本ツールにはTES/Falloutの用語を収録したMigemo追加辞書が添付されています。Migemo辞書さえインストールしてツールを起動すれば、自動的にMigemoの辞書とマージされて利用できます。
- Migemoの仕組みや詳しい入力方法についてはMigemo: ローマ字のまま日本語をインクリメンタル検索 (http://0xcc.net/migemo/)を参照してください。
- Migemo検索すると、検索ボックスに内部的な検索条件が表示されます。どういった用語が検索候補なのか、なぜヒットしないのかを知りたいときに便利です。
- Bannered Mareではバナード・メアがヒットしません。これは、英大文字が文節区切りと扱われ、文節毎に辞書参照を行うというMigemoの仕様によるものです。Bannered mareのようにするとヒットします。


===================================================================================================================
 8. 注意/制限事項/既知の問題
===================================================================================================================

- 音声ファイルを編集して再配布する場合、必ず作者から許可を取ってください。

- バニラの音声ファイルであっても再配布には一定の制限があります。一般的に、バニラの音声ファイルを（たとえベゼスダのゲームであっても）別のゲームのMODに利用することはできません。バニラのアセット利用の際にはゲーム/CKのEURA（ユーザー利用許諾書）を確認してください。

- バグがあるかもしれません。必ずゲームファイルやMODファイルのバックアップを取ってください。

- 下手な英語。英語話者ではありません。文章改善の提案は歓迎です。

- 処理時間はプラグイン/音声ファイル数に依存します。

- "Conditions"列の値は不完全です。認識できる条件式はごくわずかで、エイリアスも認識できません。あくまでも参考程度にとどめてください。

- 現時点では、すべてのレコードが異なるform idを持つ（つまりform idの重複がない）ことを前提に実装しています。
  Enderalのような一部のプラグインでは、別の対話応答レコードが同じform idを持つ場合があります。
  例えばEnderal(2016/8頃のバージョン)では、異なる対話応答レコードが同じform id "00096693" を持っています。
    [00] Skyrim.esm \ Dialog Topic \ 0009665E <MQ11c_Generic_YalKajshimTopic002> \ 00096693    "Danke."
    [00] Skyrim.esm \ Dialog Topic \ 00096675 <MQ11c_Generic_OlielTopic005> \ 00096693    "Take care, and enjoy your stay here. "
  この場合、一部のレコードは表示されず、レコードと音声ファイルの一部は正しくマッチングされません。
  音声ファイル名は対話トピックのform idを持たないため、単純にレコードとマッチングできないためです。理論的には解決可能ですが、性能が遅くなるかもしれないためこのままとします。
  要望があれば対策を検討します。

- 一部の言語では、プラグインの言語をローカルコードページに変換しないとCreation Kitがクラッシュする可能性がある問題があります。例えば日本語ではシフトJISコードページへの変換が必要です。
  このようなローカルコードページを持つプラグインを開きたい場合、Data/GameLang_*.txtファイルを開いて定義を追加してください。


===================================================================================================================
 9. 今後の計画
===================================================================================================================

- 当面はバグ修正と操作改善を継続します。

- 提案やアドバイスは歓迎です。

- 簡単なチュートリアルページを作る計画があります（永遠に計画中…）。


===================================================================================================================
 10. その他公開中のツールについて
===================================================================================================================

その他興味を持ってもらえそうな私のツールについて紹介します。興味があれば是非試してください。

- Yakitori Audio Converter - Convert fuz-xwm-wav-various audio files (全ゲーム用)
  http://www.nexusmods.com/skyrim/mods/73100/?
  http://www.nexusmods.com/fallout4/mods/9322?
  fuz/xwm/wav/mp3/oggなど多くの音声形式に対応したGUIベースのオーディオ変換ツール。動画からの音声変換もできます。
  他のツールと比較して、プログラム自身の安定性と、変換ツール(lame, ffmpeg)に対するパラメータの多彩さ/透明性に優れています。
  bsaファイルからサウンドファイルを直接開くこともできますが、旧Skyrimのbsa形式にしか対応していません。全bsa/ba2形式への対応を計画中です。

- TesvCheckEspFiles - Check the missing resource files (SkyrimLE/SE用)
  http://www.nexusmods.com/skyrim/mods/71112/?
  esm/espファイルで使われているファイルが存在するかチェックするユティリティです。
  一般的に、MODはプラグインファイル(esm/esp)と、スクリプト/音楽/テクスチャ/メッシュといったアセットファイルのセットで構成されています。
  リソースファイルが不足していると、MODが正しく動作しなかったり、表示が不正になったりします。
  このユティリティを使えば、不足しているファイルをリストアップすることができます。
  正直なところ、このツールの意図は私の能力を超えたものであり、いまだ未完成です。とはいえ、アセットの一部をチェックするには十分です。

- TesvRefidPicker - Showing RefID of NPC (SkyrimLE/SE用)
  http://www.nexusmods.com/skyrim/mods/72356/?
  このユティリティはNPCのRefID(Reference ID/参照ID)を表示するものです。 RefIDとNPCの情報は表形式で一覧表示されます。
  行をフィルタ・ソートしたり、列の並びの変更・表示・非表示することができます。
  一覧に表示されたNPCすべてにに対するコンソールコマンドをクリップボードにコピーすることもできます。

- SSLXLTNtoXML - Translation File Converter (SkyrimLE用, MOD翻訳者向け)
  http://www.nexusmods.com/skyrim/mods/77759/
  Skyrim String Localizer用の日本語化ファイル(SSLXLTN)をTESVTranslator用の日本語化ファイル(XML)に変換します。
  あるMODを日本語化したいけれど、過去バージョンのSSLXLTNしか入手できず、しかも対応するプラグインも入手できないのでTESVTranslatorの差分機能も使えない… という場面を想定して作成しました。
  Skyrim String Localizerはもはやアップデートされないので、過去の翻訳ファイルを変換して再利用するのに役立ちます。

- TESVKanjiChecker (SkyrimLE/SE/The Witcher 3用、日本のモッダー/翻訳者向け)
  http://www.nexusmods.com/skyrim/mods/66768/?
  一般にコンピューターで使える漢字は8000種類以上ありますが、Skyrim日本語版(バニラ)では2300種類程度の漢字しか表示することができません(第一水準の約3,000文字よりもさらに少ない)。
  このツールは日本語化されたMODや日本語化ファイルに含まれる、バニラでは表示できない文字をチェックします。オプションファイルでThe Witcher 3もサポートします。

- Japanese Phonetic Text Converter - Convert dialogue text to romaji from kanji (SkyrimLE/SE/Fallout4用、日本のモッダー/翻訳者向け)
  http://www.nexusmods.com/skyrim/mods/83033/?
  http://www.nexusmods.com/skyrimspecialedition/mods/9190/?
  http://www.nexusmods.com/fallout4/mods/23253/
  Creation KitのFacial Animation Generatorは一部の言語にしか対応しておらず、日本語のLIPファイルを生成できません。
  このツールは日本語の対話応答テキストをCreation Kit内蔵のFacial Animation (LIP) Generatorが「発音」できるテキストに変換します。
  このツールは日本語テキストをローマ字表記に変換することで、LIPファイルを生成できるようにします。
  音声読み上げソフトSofTalkとの連携も可能で、変換結果を音声読み上げで確認することもできます（目の悪い自分用の機能）。

- WinMerge Plugins for TES-FO-TW3 Modders (SkyrimLE/SE/Fallout4/Witcher3用、モッダー向け)
  https://www.nexusmods.com/skyrim/mods/98565
  https://www.nexusmods.com/skyrimspecialedition/mods/27347
  https://www.nexusmods.com/fallout4/mods/40012
  WinMergeを使ってMODのファイルを比較するためのWinMergeプラグインです。


===================================================================================================================
 11. クレジットと謝辞
===================================================================================================================

Lazy Voice Finder Copyright(c) 2017-2018, BowmoreLover, All Rights Reserved.
わたくしBowmoreLoverが開発しました。以下のライブラリ/ツール以外は自分で一からコーディングしています。

=== UI 翻訳 ===

ロシア語 by anizorda (http://gamer-mods.ru/index/8-16387)
すべての翻訳者に大きな感謝を！

=== 外部ライブラリ/ツール ===

LZ4 for .NET (https://github.com/IonKiwi/lz4.net)
Copyright(c) 2016, IonKiwi
Copyright(c) 2011-2014, Yann Collet, All rights reserved.

NAudio (http://github.com/naudio/NAudio)
Copyright(c) 2001-2017, Mark Heath

NAudio.Vorbis (https://github.com/NAudio/Vorbis)
Copyright(c) 2015, Andrew Ward

NVorbis (https://github.com/ioctlLR/NVorbis)
Copyright(c) 2016, Andrew Ward

C/Migemo (http://www.kaoriya.net/)
Copyright(c) 2003-2007 MURAOKA Taro (KoRoN)

kanaxs ex C# (https://dobon.net/)
Copyright(c) 2011, DOBON! <http://dobon.net>, All rights reserved.

Microsoft (R) xWMA Encoding Tool Copyright (C) 2009 Microsoft Corporation. All rights reserved.

=== 謝辞 ===

greentea101と彼のVoice File Reference Toolに (http://www.nexusmods.com/skyrim/mods/28462/)
    彼の作品は本ツール開発の大きなひらめきを与えてくれました。本当にありがとう！
Unofficial Elder Scrolls PagesのMODファイル形式ページに (http://www.uesp.net/wiki/)
    このページの情報は私にとってとても有用でした。
内田明さんと彼のOradano Mincho Fontに (http://www.asahi-net.or.jp/~sd5a-ucd/freefonts/Oradano-Mincho/)
    彼の美しいフォントをアイコンの文字に使っています。
Francisco Pozo - DJ FrANKy EHPと彼のMultiple Languages Strings Unified Centralに
    Multiple Languages Strings Unified Central (http://www.nexusmods.com/skyrim/mods/82578/?)
    Multiple Languages Strings Unified Central SSE (http://www.nexusmods.com/skyrimspecialedition/mods/4505/?)
    彼の多言語stringsファイルは開発とテストに大いに役立ちました。
AFK Modsフォーラムメンバーによるプラグインファイル形式の情報に (https://afkmods.iguanadons.net/)
    フォーラムでのFallout 4のファイル形式に関する議論は大いに役立ちました。
ElminsterAUとxEdit開発チームに
    TES4Edit (http://www.nexusmods.com/oblivion/mods/11536/)
    FO3Edit (http://www.nexusmods.com/fallout3/mods/637/)
    FNBEdit (http://www.nexusmods.com/newvegas/mods/34703/)
    TES5Edit (http://www.nexusmods.com/skyrim/mods/25859/)
    SSEEdit (http://www.nexusmods.com/skyrimspecialedition/mods/164/)
    FO4Edit (http://www.nexusmods.com/fallout4/mods/2737/)
    xEditはプラグイン形式の調査と理解に欠かせないツールです。素晴らしい仕事です！

モッディングコミュニティ全体、Nexus mods、そしてもちろんベゼスダに感謝します。

=== 開発ツール ===

Microsoft Visual C# 2015 + .NET Framework 4.0/4.6.1
TES4Edit by ElminsterAU (http://www.nexusmods.com/oblivion/mods/11536/?)
FO3Edit by ElminsterAU (http://www.nexusmods.com/fallout3/mods/637/?)
FNVEdit by ElminsterAU (http://www.nexusmods.com/newvegas/mods/34703/?)
TES5Edit by ElminsterAU (http://www.nexusmods.com/skyrim/mods/25859/?)
SSEEdit by ElminsterAU and SSEEdit team (http://www.nexusmods.com/skyrimspecialedition/mods/164/?)
FO4Edit by ElminsterAU (http://www.nexusmods.com/fallout4/mods/2737/?)
GIMP (グラフィックリソース編集に使用) (https://www.gimp.org/)
Audacity (http://www.audacityteam.org/)
ScreenToGif (アニメーションGIF作成) (http://www.screentogif.com/)

//