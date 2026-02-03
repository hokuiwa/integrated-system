# 📤 GitHubへのプッシュ手順

## ステップ1: ファイルを配置

1. クローンしたフォルダ（integrated-system）を開く
2. 以下のファイルをコピー：
   - index.html
   - README.md

## ステップ2: GAS URLを設定

index.htmlを開いて、以下の行を修正：

```javascript
const GAS_API_URL = 'https://script.google.com/macros/s/あなたのURL/exec';
```

↓

```javascript
const GAS_API_URL = 'https://script.google.com/macros/s/実際のURL/exec';
```

保存する。

## ステップ3: GitHub Desktopでプッシュ

### GitHub Desktop使用の場合：

1. GitHub Desktopを開く
2. 左側に変更されたファイルが表示される
3. 左下の「Summary」に「初期バージョン」と入力
4. 「Commit to main」をクリック
5. 「Push origin」をクリック

### コマンドライン使用の場合：

```bash
# フォルダに移動
cd integrated-system

# ファイルを追加
git add .

# コミット
git commit -m "feat: 顧客管理・コンテナ管理の初期バージョン"

# プッシュ
git push origin main
```

## ステップ4: GitHub Pagesで公開

1. GitHubのリポジトリページを開く
2. Settings → Pages
3. Source: main branch
4. Save

5分後：
```
https://あなたのユーザー名.github.io/integrated-system/
```

でアクセスできる！

## 完了！🎉

これで顧客管理システムが公開されたよ！
