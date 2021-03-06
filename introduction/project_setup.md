## プロジェクトのセットアップ {#project-setup}

説明を始める前に、どのようにVisual StudioまたはXamarin等でプロジェクトをセットアップするかを示す。

1. 新規プロジェクトを作成する（.NET 4.5以上）
2. ソリューションエクスプローラーの「参照」で右クリックし、「NuGet パッケージの管理」をクリック
3. 「**NBitcoin**」を検索しインストールする。
   ![](../assets/nuget_jp.png)  

> **ヒント:** MacやLinuxでも、NBitcoin.Monoではなく、NBitcoinを使うこと。

NBitcoinは、この本のメイン筆者であるNicolas Dorierがメンテナンスしている、.NETで作られたオープンソースライブラリである。C\#でビットコインのソフトウェアを開発するのであれば、このライブラリを使うべきだろう。NBitcoinはクロスプラットフォームアプリケーションをサポートする。

### NBitcoinのソースコードをデバッグする方法（オプション）

いろいろと簡単に調べられるように、NBitcoinは、そのソースコード内をデバッグできるようにしてある。この機能が使えるようにするためには、Visual Studioのツール/オプション/デバッグで「ソースサーバーサポートを有効にする」をチェックする必要がある。  
![](../assets/visualstudio_enablesourceserversupport_jp.png)

これで、もしNBitcoinのコードにステップインをすると、ソースコードがGitHubから自動的に取得され、visual studioのデバッガーに表示される。

