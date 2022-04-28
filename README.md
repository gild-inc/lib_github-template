## 概要

githubのISSUEやPRのテンプレートを提供します。  
全てのリポジトリでテンプレートのフォーマットを統一する為に、この手法はベストです。

## 設定方法

リポジトリルートの`composer.json`に以下追記します。

* composer.json
```json
{
    "scripts": {
        "post-autoload-dump": [
            ". vendor/gild/github-template/execution.sh"
        ]
    }
}
```

```shell
composer require --dev gild/github-template ^1.0
```

