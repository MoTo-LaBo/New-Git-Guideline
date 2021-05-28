# New-Git_Guideline
- Git Complete Guide の新規追加・修正・改訂
- Git Complete Guide に新たに追記したい情報をまとめました
- submodule として Git Complete Guide に紐づいています
#### Git Complete Guide clone 時は、こちらの file/direcotory 情報は clone されないので注意
- 下記のcommand で clone すれば、New Git Guideline のfile / direcotory 情報も一緒に clone されます
## Git Complete Gide cole時には submodule を初期化＆更新を実行して下さい
    git clone --recurse-submodules <url>
## submodule が更新された場合
- **親 project の submodule directory は常に最新の commit をさすわけではない**
- あくまでも別々の repositories なので subumodule の中で個別に pull して情報を更新しないといけない
### 全ての submodule でコマンドを実行 ※ 基本は下記のコマンドを使用する
    git submodule forcach '<command>'
- git subumodule foreach `git pull origin main`コマンドを実行する事によって、各 subumodule で git pull origin main が実行される
