## 概要

githubのISSUEやPRのテンプレートを提供します。  
全てのリポジトリでテンプレートのフォーマットを統一する為に、この手法はベストです。

## 設定方法

リポジトリルートの`composer.json`に以下を追記します。

* composer.json
```json
{
    "require-dev": {
        "gild-lib/github-template": "^1.0"
    },
    "scripts": {
        "post-autoload-dump": [
            ". vendor/gild-lib/github-template/execution.sh"
        ]
    }
}
```
