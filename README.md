## 概要

githubなどのホスティングサービスでISSUEやPRなどの利用可能なファイルテンプレートを提供します。  
全てのリポジトリでフォーマットを統一する為にこの手法は煩わしくありません。

## 設定方法

リポジトリルートの`composer.json`に以下を追記します。

* composer.json
```json
{
    "repositories":[
        {
            "type": "vcs",
            "url": "git@github.gild-inc:gild-inc/lib-hosting-required.git"
        }
    ],
    "require-dev": {
        "gild-lib/hosting-required": "*"
    },
    "scripts": {
        "post-autoload-dump": [
            ". vendor/gild-lib/hosting-required/execution.sh"
        ]
    }
}
```
