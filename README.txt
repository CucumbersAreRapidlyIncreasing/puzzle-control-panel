謎解き用 システム制御盤
========================

使い方
1. outputs/index.html をSafariなどのブラウザで開きます。
2. レバーは1本だけONにできます。同じレバーを再度押すとOFFになります。
3. ボタンは押している間だけONです。黄と桃の2個を同時に押すと成功します。
4. ダイヤルはタップごとに1から6まで進みます。
5. A=2、B=3、C=4、D=1、E=5で復旧メッセージが表示されます。
6. 右上のリセットですべて初期状態に戻ります。

iPadでの利用（推奨）
1. index.html、manifest.webmanifest、sw.js、.nojekyll、iconsフォルダを
   GitHubリポジトリの直下へアップロードします。
2. Settings > Pagesで「Deploy from a branch」「main」「/(root)」を選択します。
3. 公開URLをiPadのSafariで開きます。
4. 共有 > ホーム画面に追加 > Web Appとして開くをオンにします。
5. 最初にオンラインで一度起動すると、以後はオフラインでも起動できます。

PWA用ファイル
- manifest.webmanifest: アプリ名、表示方法、アイコンを定義します。
- sw.js: 必要なファイルをiPadへキャッシュし、オフライン起動を可能にします。
- .nojekyll: GitHub Pagesでファイルをそのまま配信させます。
- icons: iPadホーム画面などに表示するアイコンです。

PCで確認する例
outputsフォルダで次を実行し、http://localhost:8000 を開きます。

  python -m http.server 8000

レバー、ボタン、ダイヤル、ラベル、三角マーカーはすべてHTML内のSVGです。
