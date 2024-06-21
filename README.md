# Tatsumi0000/texlive-ja-devcontainer-template

[korosuke613/texlive-ja-devcontainer-template](https://github.com/korosuke613/texlive-ja-devcontainer-template)をベースに一部カスタマイズをしたテンプレートです。変更点は以下の通りです。
- bibtexを使った参考文献管理
- mintedを使ったソースコード掲載
- devcontainerで使うベースイメージをUbuntu 24.04 LTSにアップデート
- compose specificationに対応
- docker imageをGitHub Container Registryで管理
  - docker imageのCI/CDでビルド


# texlive-ja-devcontainer-template

VS Code Remote Developmentの機能を用いて、LaTeX環境を容易に構築するサンプルコードです。

Dockerイメージは、[texlive-ja-devcontainer-template/texlive-ja](https://github.com/Tatsumi0000/texlive-ja-devcontainer-template/pkgs/container/texlive-ja-devcontainer-template%2Ftexlive-ja)を利用しています。

(**Dockerが必要です**)

## setup

1. `git clone https://github.com/Tatsumi0000/texlive-ja-devcontainer-template.git`
2. VS Codeで`texlive-ja-devcontainer-template`を開く。
3. 拡張機能[Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)を追加する。
4. 左下の`><`アイコンを押して、`Rebuild Container`を実行する。
5. 待つ。
6. ワークスペースが開いたら、terminalを開き、`latexmk sample.tex`を実行する。
7. 上手くコンパイルできたらsetup完了！

## build

```bash
latexmk sample.tex
```

`sample.pdf`という実行ファイルができているはず。
