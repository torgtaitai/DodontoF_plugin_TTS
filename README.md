DodontoF_plugin_TTS
===================

TTS plugin for DodontoF

## これは何？
* どどんとふ(DodontoF)にTTS(Text to Speech)機能を追加することを目的としたプロジェクトです。
* どどんとふって何？ → [こちら](http://www.dodontof.com/) をご覧ください。
* TTS って何？ → [こちら](http://ja.wikipedia.org/wiki/%E9%9F%B3%E5%A3%B0%E5%90%88%E6%88%90) をご覧ください。


## 依存しているミドルウェア
* Open JTalk [URL](http://open-jtalk.sourceforge.net/)
* HTS engine API [URL](http://hts-engine.sourceforge.net/)
* MMDAgent Example [URL](http://www.mmdagent.jp/)


## 導入に必要な環境
* Unix
    * サーバ利用を前提としているため、OSXやWindowsOSは対象外です。
* wget
* tar
* unzip
    * これらのコマンドが導入されていない場合は、 apt または yum で導入して下さい。
* ruby
    * 現在(2014-03-06)の時点で安定版とされているバージョン 2.0 系を対象としています。
    * しかし、どどんとふの推奨環境が。まだ、バージョン 1.8 系のため、互換動作を前提としています。


## 導入手順
1. 当プロジェクトサイトより、ソースコードまたはパッケージを取得する。
2. README をざっと目を通す。(*推奨*)
3. Open JTalk インストールスクリプトに実行権限を付与する。
    * インストールスクリプトは *open_jtalk_install.sh* というファイル名です。
    * $ chmod +x open_jtalk_install.sh
3. Open JTalk インストールスクリプトを実行する。(root 権限でなくても良い)
    * $ ./open_jtalk_install.sh
4. サンプルスクリプトで動作確認をしてみる。
    * $ chmod +x sample.rb
    * $ ruby sample.rb
        * この結果、 sample.txt の内容が、 sample.wav 音声ファイルとして出力されれば
        * Open JTalk 環境は正常に動作しています。
5. ここから先はまだ開発途中です。しばらくお待ちください。


## パッケージに含まれるもの
* README.md
* COPYING
* AUTHOR
* TODO.md
* HISTORY.md
* open_jtalk_install.sh
    * Open JTalk 環境をインストールするためのスクリプトです。
* open_jtalk.rb
    * Open JTalk の ruby ラッパーです。
* sample.txt
    * サンプル入力用のテキストファイルです。
* sample.rb
    * サンプル出力用のスクリプトです。
* DodontoFServerTTS.rb
    * どどんとふ用のTTSプラグインです。 DodontoFServer.rb を見様見真似でそれっぽく記述してみました。
    * 詳しくはコメント参照。

## TODO
長いので、別ファイルにまとめておきます。

## COPYING
### Open JTalk
> "The Japanese TTS System 'Open JTalk'
developed by HTS Working Group
http://open-jtalk.sourceforge.net/"


> "Copyright (c) 2008-2013  Nagoya Institute of Technology
                         Department of Computer Science
All rights reserved."


### HTS engine API
> "The HMM-Based Speech Synthesis Engine 'hts_engine API'
developed by HTS Working Group
http://hts-engine.sourceforge.net/"


> "Copyright (c) 2001-2013  Nagoya Institute of Technology
                         Department of Computer Science
              2001-2008  Tokyo Institute of Technology
                         Interdisciplinary Graduate School of
                         Science and Engineering
All rights reserved."



