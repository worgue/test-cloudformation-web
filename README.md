# test cloudformation django
djagnoアプリケーションを動かすcloudformationのサンプルです
簡単に使うには不足分が多いためtestです。
TODOが終わったら名前を変えて、アップし直します。


## TODO

- NATの追加
- EC2とfargate taskをprivate subnetへ配置するオプションの追加
- djangoとnginxのタスク定義分割
- segurity groupの整理
-- 何に使うかではなく役割によって名称を設定
-- そうでない場合、必要な時に必要なsecurity groupを追加
- fargate containerに対する任意のenv設定を検討
- fargate containerに対する任意のsecretからのenv設定を検討
- DATABASE_URLとDJANGO_ENV_PATHを上記secretsからの設定に移行
- RDSのマスターパスワードローテション
- readonly containerを選択可能にする
- cookiecutter化してcloudformationのParameterや要素を事前に減らしたり、テンプレートの依存関係を解決
- gunicornコマンドのproject_nameをcookiecutterで埋めるか、空白時は設定しない
