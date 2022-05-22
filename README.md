# 源亜こぶり明朝について
この源亜(げんあ)こぶり明朝は、Amazon Kindle Paperwhite/Oasis上で[源暎こぶり明朝](https://okoneya.jp/font/genei-koburimin.html)を極力適用する為に改良をしたものです。  
Kindleには \\\\Kindle\\fonts フォルダに外部フォントを配置することで、組み込み以外のフォントを使用できる機能が公式に備わっています。  
しかし、組み込み以外のフォントを使用した場合、フォントが斜体のグリフを持っていなければ標準体フォントを参照する仕様があり、これを回避するために源亜フォントを作成しました。  
PC、スマートフォン等、他の端末でも使用できますが、これらの端末は自身で標準体を斜体に見せかける機能があるため、このフォントを使用するメリットはありません。
源暎こぶり明朝を使用することを推奨します。  
名前の由来は基のフォントの名前「源」と亜馬孫/亜馬生(アマゾン)、亜種の「亜」から取っています。<s>語呂が悪い。</s>  

# フォントの使い方
\\\\Kindle\\fonts フォルダに、2つの GenAKoburiMinchoV-\*\*.ttf を入れると縦書き用、 GenAKoburiMinchoH-\*\*.ttf を入れると横書き用がKindle上で設定できるようになります。  
不要の場合はこれらファイルを削除してください。  
書籍によっては明朝体/ゴシック体を指定している箇所があり、本文と違う書体が指定されている場合は組み込みの明朝/ゴシックフォントが読み込まれます。
これは回避できない仕様です。  
なお、これらの.ttfファイルを.ttcファイルにまとめた場合、太字・斜体フォントが動作しませんので、.ttcファイルに改変しての使用はお勧めしません。

# フォントの特徴  
標準(Regular)については、基となった源暎こぶり明朝のグリフを一切変えていません。太字・斜体フォントと互換性を持たせるため、フォント名等の設定調整に留めています。  
斜体はfontforgeの機能で、標準、太字を文末方向へそれぞれ13度斜めに歪ませています。
縦書き用、横書き用で歪ませている方向が違います。  

# 更新履歴  
- ver. 2.00 (2022/05/22)
    - Boldフォントを削除しました。(Kindle Paperwhite(第11世代) ver.5.14.3.0.1にはRegularフォントをBoldのように表示する機能はあるため、基となった源暎こぶりにないBoldフォントを削除しました。)  
    - 縦書きフォントについて、[Unicode Vertical Orientation Revision 17](https://unicode.org/Public/vertical/revision-17/VerticalOrientation-17.html)を基に全てのグリフの傾き方向を見直しました。  
    - Obliqueフォントを作る際のアルゴリズムを見直しました。(従来の作成方法では傾きが上手く適用できていなかったり、傾きが何倍にも増幅する事がありましたが、今回の見直しで改善しました。)  
    - 縦書き用グリフの表示方法を見直しました。(縦書き用グリフを復活し、代わりにLookups.GSUB.vrt2テーブルを削除しました。)  
    - Fontforgeのバージョンを上げました。(FontForge-2020-11-07(FontForge 20th Anniversary Edition) => FontForge-2022-03-08)
- ver. 1.01 (2021/07/29)
    - 縦書きフォントのギリシア文字、キリル文字、一部記号の傾き方向を修正しました。  
- ver. 1.00 (2021/07/24)
    - 初版  

# ライセンス
[SIL Open Font License 1.1](https://github.com/PermanentWave/GenA-Koburi-Mincho/blob/main/LICENSE_OFL.txt)のもと配布いたします。
個人利用・商用利用にかかわらず、無償で使用することができ、再配布やソフトウェアへの組み込み、改変などが可能です。  
その他利用に関する免責条項の詳細は、[SIL Open Font License 1.1](https://github.com/PermanentWave/GenA-Koburi-Mincho/blob/main/LICENSE_OFL.txt)をご確認ください。\([日本語サイトリンク](https://licenses.opensource.jp/OFL-1.1/OFL-1.1.html)\)  
本フォントを使用した事により発生した事象に対し、フォント作成者は何の責任も持ちません。自己責任でお使いください。  
「予約されたフォント名」は日本語表記では「源亜」、アルファベット表記では「GenA」とします。  
本フォントに問題がある場合はGithubのIssueまたは[Twitter](https://twitter.com/O_PermanentWave)に連絡をお願い致します。
御琥祢屋様へのご連絡はお控えください。  

# 謝辞
源ノ明朝/源ノ角ゴシックを配布してくださっている[Adobe-Fonts](https://github.com/adobe-fonts)様  
源暎こぶり明朝およびvmtx修正ソフトウェア[o_vmtx-fix](https://okoneya.jp/font/knowhow.html)を配布、fontforgeで源ノ明朝/源ノ角ゴシックを改変する方法について解説してくださっている[御琥祢屋](https://okoneya.jp/)様  
各グリフの表示を確認する電子書籍を公開してくださっている[wakufactory](https://wakufactory.jp/densho/font/mojitest.html)様  
この場をお借りし、感謝申し上げます。

# 参考
> [源亜こぶり明朝作成の備忘録](https://permanentwave.github.io/2021/07/24/2021-07-24-01/)  
> [fontforge Module attributes](https://fontforge.org/docs/scripting/python/fontforge.html)  
> [OS/2 — OS/2 and Windows Metrics Table](https://docs.microsoft.com/en-us/typography/opentype/spec/os2)  
> [Unicode Vertical Orientation Revision 17](https://unicode.org/Public/vertical/revision-17/VerticalOrientation-17.html)
