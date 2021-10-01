# GitHub CLI
- **参考 site**
> https://cli.github.com/

> https://cli.github.com/manual/

> https://zenn.dev/torahack/articles/d6b760fd11bf3a
### 1. install
    brew install gh
### 2. 確認
    # help, その他command
    gh
### 3. terminal と GitHub acount 同期
    # 1.
    gh auth login
    # 2.
    GitHub.com
    # 3.
    SSH
    # 4.
    Paste an authentication token
    # 4-1. 表示される password copy 後
    Enter
    # 5. browser で先程の password 入力
    Authoreize github
    完了！
## GitHub CLI command
### 1. Local Repository 作成 ※ project dir内で
    git init
### 2. IDE 開く
    code
### 3. README.md & .gitignore
    touch README.md
    touch .gitignore
### 4. add & commit
    git add.
    git commit -m 'Frst Commit'
### 5. gh CLI
    gh repo create
    # name ?
- *default は directory name がそのまま反映される*
### 6. description ?
    This is the repository for testing GitHub CLI
### 7. Visibility ?　( reop の種類 )
- *Public, Private, Internal*
### 8. 最終確認される
    Enter
### <center>これで remote repository 作成完了 !!</center>
### 9. branch 作成・切り替え・push
    # branch & 切り替え
    git checkout -b develop

    # push
    git push - u origin develop
### 10. GitHub browser 立ち上げ
    gh repo view --web
- しっかり出来ているか確認してみる
### pull Request
    # 1.
    gh pr create

    # 2. どこに pull requ するか聞かれる
    remote repo

    # 3. Title, Body, Submit
    入力 -> 送信
### pull Request 確認
    gh pr list
