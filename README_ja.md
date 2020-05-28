# VRWorkout
Oculus Quest 向け VR フィットネスゲーム

[![Oculus Quest Download](https://github.com/mgschwan/VRWorkout/raw/master/web_assets/download_button_oculusquest.png)](https://github.com/mgschwan/VRWorkout/releases/latest/download/VRWorkout.apk)

[![Windows Download](https://github.com/mgschwan/VRWorkout/raw/master/web_assets/download_button_windows.png)](https://github.com/mgschwan/VRWorkout/releases/latest/download/VRWorkout_win.zip)

[![SideQuest Install](https://github.com/mgschwan/VRWorkout/raw/master/web_assets/install_button_sidequest.png)](https://sidequestvr.com/#/app/413)


## これはなに？

[Godot Engine](https://godotengine.org) で作られた VR 音楽運動ゲームです。

このゲームは短時間（長時間プレイすれば長時間）の体操に匹敵するであろう魅力的な運動を体験できる VR ゲームです。Beat Saber や BoxVR のような他の音楽ゲームと比較すると、立ち姿勢、スクワット、腕立て伏せ、サイドプランク、腹筋、ジャンプそしてバーピーが切り替わることによって、より筋肉群が活性化されるでしょう。

しかし全てのゲームと同様に、それは動作中にプレイヤーがズルをしないで実際に運動をするかによります。このゲームの唯一の敵はプレイヤー自身の体であり、もしあなたがしっかり自分と向き合えば、しっかりやりきったという感覚を得られます。

### 運動の種類

* 立ち状態 (または、スコアの倍率を上げるために走る)
* ジャンプ：ターゲットに頭で触れるためプレイヤーは少しジャンプする必要があります。
* スクワット： 深いスクワットを行う
* 腹筋：繰り返し腹筋をする必要はないですが、仰向けの状態から頭と両手でターゲットに触れる必要があります。
* 腕立て伏せ：腕立て伏せの姿勢のまま手でターゲットに触れます（片手でパンチすることで体幹の筋肉を活性化できます）。頭のターゲットが上下に動いて腕立て伏せの動きになります。
* バーピー：腕立て伏せの姿勢で頭でターゲットに触れた後、すぐにジャンプをして頭でターゲットに触れます.

単調なワークアウトを避けるために、このゲームではこれらの運動が切り替わります。

**免責事項: 自己責任で使用してください！このゲームはあなたが周辺のものに衝突するかどうか確認しません。これは物理的な運動ゲームなので、怪我をしてしまう可能性がある動きが多く含まれます。このゲームは無料であり、あくまで自己責任で使用するようにご了承ください。**

## インストール

* 直接 [Sidequest](https://sidequestvr.com/#/app/413) からイントールするか、
* 最新の APK ファイルを [Releases](https://github.com/mgschwan/VRWorkout/releases) からダウンロードして、ADB からデバイスにインストールしてください。

このゲームはハンドトラッキングでプレイするのが 1 番です！

## 遊び方

![Handtracking](https://github.com/mgschwan/VRWorkout/raw/master/web_assets/vrworkout_hand_suggestion.jpg)

* 音楽のリズムに合わせて手でターゲットを叩きます。トラッキングしやすくするため **手を開いて** プレイしてください。
* 頭のターゲットには、頭で触れてください。ただ触れるだけで、頭突きをする必要はありません。
* 駆け足をすると最大 4 倍までのスコアボーナスが入ります
* プレイ中に他の運動に切り替えたいときは、右側の運動選択メニューを 2 回タッチしてください

ターゲットを叩く最適なタイミングは、ターゲットの周囲を回転しているマークが、もう 1 つのマークに触れた瞬間です。

ゲーム開始時にいくつかの四角が表示されます。その中のプレイしたい難易度の部分にタッチすると、曲と難易度が選択できます。
左側の運動リストでそれぞれの運動の ON/OFF を切り替えられます。

プレイ中にステージから離脱する：左側の青い柱の上の方にある文字部分からステージを離脱できます。

__フリープレイモード__

自分の持っている曲でフリープレイができます*
バックグラウンドで（恐らく nullnMusic Player を使って）音楽を流しながら、音楽のビートに合わせてメインメニューにあるドラムを叩いてください。
ビートが設定できたら、右側のフリープレイから 1 つを選択してください。すると設定した BPM に合わせてターゲットが流れてきます。ただし一切音楽は再生されません。

__ビーストモード（Quest 版のみ）__

Quest 版のみビーストモードが有効化できます。左側の「Toogle Beat mode」と書かれた四角をタッチすると、爪が有効化されます。手を握ると爪を出して、手を開くとしまえます。
ビーストモードが有効化されているときは、左右の人物が敵として襲いかかってくるようになります。爪を使って襲ってくる敵を倒しましょう。

## VR フィットネスの結果

21 分程度 VRWorkout の "Hard" で全曲を試したところ、288kcal 燃焼できました。

![Workout Statistic](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/workout_statistics.jpg)

測定は Polar H10 心拍数モニターと Polar Beats app を使用しました。

## 開発

これは私(開発者)が初めて作った VR ゲームであり、初めて Godot を使って開発したゲームでもあるため、コードは少し汚いです。

Oculus Quest 版の開発に必要なもの：

* Godot 3.2+  [ダンロードはこちら](https://godotengine.org/)
* アセットライブラリの Godot Oculus Mobile Plugin
* 開発者モードにした Oculus Quest ヘッドセット

PC 版の開発に必要なもの:

* Godot 3.2+ [ダウンロードはこちら](https://godotengine.org/)
* アセットライブラリの OpenVR plugin
* SteamVR

すべてをインストールしたら、godot_project フォルダから project.godot ファイルをインポートして、ゲームの編集を始めてください。



## 簡単なゲームプレイ動画

__最新バージョン__

[![v0.9.7](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/workout_video_playscreen.jpg)](https://www.youtube.com/watch?v=mknXbyVJm3c)

__旧バージョン__

[![Side plank update](https://img.youtube.com/vi/FWY8M-wg_mo/0.jpg)](https://www.youtube.com/watch?v=FWY8M-wg_mo)
[![Beast mode update](https://img.youtube.com/vi/6TnzuIsVT6o/0.jpg)](https://www.youtube.com/watch?v=6TnzuIsVT6o)
[![Sample gameplay](https://img.youtube.com/vi/mSPQulHXlJo/0.jpg)](https://www.youtube.com/watch?v=mSPQulHXlJo)


## スクリーンショット
![Standing left hand hit](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/stand_left_hand2.png.jpg)
立ち状態 - 手のターゲット

![Crunches](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/crunch1.png.jpg)
腹筋 - 手のターゲット

![Crunches](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/crunch2.png.jpg)
腹筋 - 頭のターゲット

![Jumping](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/jump.png.jpg)
ジャンプ

![Pushup left hand hit](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/pushup_left_hand.png.jpg)
腕立て伏せ - 手のターゲット

![Side plank](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/side_plank.png.jpg)
腕立て伏せ - サイドプランク

![Squat hand left](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/squat_hand_left.png.jpg)
スクワット - 手のターゲット

![Squat head](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/squat_head.png.jpg)
スクワット - 頭のターゲット

![Stand head](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/play_screenshots/stand_head.png.jpg)
立ち状態 - 手のターゲット

![Screenshot new 4](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/vrworkout_beast_attack.jpg)
ビーストモード - ビーストアタック

![Screenshot new 3](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/vrworkout_instructor3.jpg)

![Screenshot 1](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/vrworkout_menu.jpg)

![Screenshot 3](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/vrworkout_side.jpg)

![Logo](https://github.com/mgschwan/VRWorkout/blob/master/web_assets/vrworkout_godot_transparent_figures.jpg)


## フィードバック

提案やフィードバックは discord グループ [VRWorkout Dojo](https://discord.gg/Vg3vyah) または、dev@vrworkout.at にメールを送信してください。

## クレジット:

### 音楽
* ‘Duty to Humanity’ composed and performed by Moumoku. [Link to artist](https://artbymoumoku.org/​)
* 'Slayers of the Ice Dragon' composed and performed by Nagoonberries Music. [Link to artist](https://soundcloud.com/nagoonberries)
* Odder Stuff (Duckettized) by 7OOP3D (c) copyright 2019 Licensed under a Creative Commons Attribution Noncommercial  (3.0) license. http://dig.ccmixter.org/files/7OOP3D/60150 Ft: Duckett
* Drive by Alex (c) copyright 2013 Licensed under a Creative Commons Attribution (3.0) license. http://dig.ccmixter.org/files/AlexBeroza/43098 Ft: cdk & Darryl J
* Deeper In Yourself (cdk mix) by Analog By Nature (c) copyright 2012 Licensed under a Creative Commons Attribution Noncommercial  (3.0) license. http://dig.ccmixter.org/files/cdk/39241 Ft: Covert
* Like This (cdk Step This mix) by Analog By Nature (c) copyright 2012 Licensed under a Creative Commons Attribution Noncommercial  (3.0) license. http://dig.ccmixter.org/files/cdk/37315 Ft: 4Nsic
* The Game Has Changed (cdk RumbleStep Mix) by Analog By Nature (c) copyright 2013 Licensed under a Creative Commons Attribution (3.0) license. http://dig.ccmixter.org/files/cdk/41830 Ft: My Free Mickey
* Shameless Site Promotion by Platinum Butterfly (c) copyright 2012 Licensed under a Creative Commons Attribution Noncommercial  (3.0) license. http://dig.ccmixter.org/files/F_Fact/38008 Ft: Alex, Ms. Vybe
* Tiny Spaceships by Hans Atom (c) copyright 2019 Licensed under a Creative Commons Attribution (3.0) license. http://dig.ccmixter.org/files/hansatom/60364 Ft: Donnie Ozone
* The Game Has Changed by My Free Mickey (c) copyright 2013 Licensed under a Creative Commons Attribution (3.0) license. http://dig.ccmixter.org/files/myfreemickey/40672 Ft: Kamihamiha
* Clarity* (a moment of) by Scomber (c) copyright 2014 Licensed under a Creative Commons Attribution Noncommercial  (3.0) license. http://dig.ccmixter.org/files/scomber/48133 Ft: My Free Mickey, Kare Square  & Ms.Vybe

### 3D モデル

* KF2 Berzerker Perk Symbol by DiabolicMaggot
* Low Poly Forest by isbl 
* Floating Islands by Otis25 
* Open Tatami Room by OSad 
