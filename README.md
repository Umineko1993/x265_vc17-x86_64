# x265_vc17-x86_64
x265_git ( https://bitbucket.org/multicoreware/workspace/projects/PROJ ) をビルドしてます

# 簡単にビルドまでの手順を説明

必要な物
> [Cmake](https://cmake.org/download/)</br>
> [git](https://git-scm.com/downloads/win)</br>
> [Visual Studio 2022](https://visualstudio.microsoft.com/ja/downloads/)

①x265を保存する空ファイルを用意して、空ファイル内でWindowsターミナル又はコマンドプロンプトを開き、
` git clone https://bitbucket.org/multicoreware/x265_git.git ` を実行してクローンを作成。(ここでgit必要)

x265のテスト版?のビルドしたい場合は、` git clone https://bitbucket.org/multicoreware/x265_git_testing.git ` こっちを実行。(x265_git_testingってファイルが出来る)

②x265_gitってフォルダが作成されるので、`x265_git→build→vc17-x86_64`と移動。 

③フォルダ内の`make-solutions.bat`を実行。(ここでCmake必要)

④CMakeのウインドウが開いたら、`Configure`・`Generate`・`Open Project`の順に押すとVisual Studioが起動する。(Visual Studioが起動したらCmakeのウインドウは閉じてOK)

⑤Visual Studioが起動後ウインドウ上部の `ローカルWindowsデバッカー`をクリック。

⑥出力logに `=========== ビルド は -:--:- で完了し、--.--- 秒 掛かりました ==========`  が表示されたら、Visual Studioを終了させる。

⑦`x265_git→build→vc17-x86_64→Debug`のフォルダ内に`x265.exe`が作成されている。
