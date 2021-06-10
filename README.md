## 概要

githubのISSUEやPRのテンプレートを提供します。  
全てのリポジトリでテンプレートのフォーマットを統一する為に、この手法はベストです。

## 設定方法

リポジトリルートの`composer.json`に以下を追記します。

* composer.json
```json
{
    "repositories":[
        {
            "type": "vcs",
            "url": "git@gild.github.com:gild-inc/lib_github-template.git"
        }
    ],
    "require-dev": {
        "gild-lib/github-template": "*"
    },
    "scripts": {
        "post-autoload-dump": [
            ". vendor/gild-lib/github-template/execution.sh"
        ]
    }
}
```
