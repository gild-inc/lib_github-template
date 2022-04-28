## 概要

githubのISSUEやPRのテンプレートを提供します。  
全てのリポジトリでテンプレートのフォーマットを統一する為に、この手法はベストです。

## 導入要件

* なし

## 導入方法

`composer.json`に以下追記します。

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

