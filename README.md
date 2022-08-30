1. レポジトリ作成&git clone
githubでレポジトリを作成。
`git clone https://github.com/k-karen/test-app.git`
とかでCloneしてくる

2. vue create ~ build
クローンしたレポジトリ配下までcdしてから。
```
# レポジトリ名と同じ名前のアプリでいいなら、vue create . でOK。
vue create .
# オプションは適当でOKだと思います(babel,PWAをマニュアルで選択して私は行いました)
vi vue.config.js
# でレポジトリのファイルを参考に設定を作る。
yarn build
# git add -A & git push origin headとかで適当に今までの変更をgithubへpush
```

3. githubの設定
github上のSettingsからGitHub Pages の Source を `master branch /docs folder` にする。
https://k-karen.github.io/test-app/index.html
と反映できたことが確認できたかと思います。



# test-app

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn run serve
```

### Compiles and minifies for production
```
yarn run build
```

### Run your tests
```
yarn run test
```

### Lints and fixes files
```
yarn run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
