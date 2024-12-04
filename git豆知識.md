# リモートmainブランチのものを、ローカルのfeatureブランチに反映させる方法

1. リモートリポジトリの最新情報を取得します
```
git fetch origin
```
2. featureブランチに切り替えます
```
git checkout feature
```
3. mainブランチをfeatureブランチに切り替えます
```
git merge origin/main   ※この段階で、featureブランチに切り替わっているので、featureブランチに最新のmainブランチの情報が反映される。
```

## コマンドまとめ

```
git fetch origin               # リモートの最新情報を取得
git checkout feature           # featureブランチに切り替え
git merge origin/main          # mainブランチをマージ
```