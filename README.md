## 概要

githubのISSUEやPRのテンプレートを提供します。  
全てのリポジトリでテンプレートのフォーマットを統一する為に、この手法はベストです。

<details>
<summary>物好きなあなたへ...</summary>

本リポジトリは弊社で管理する複数リポジトリのPRテンプレートを統一するために作りました。

書式は弊社に馴染むものにしていますが、書式がどうあれ一元化されたい方はcomposerにrequireしても構いません。

そのためにpublicリポジトリに変更し、packagistにも登録しました。

所謂、書式はうちのを使ってもらうことになるけどそれでもいいなら相乗りOKだよ、ということです。

issueやPullRequestは立てられるようになっていますから、それぞれ提案していただくことは可能です。

ただしrejectとなる場合もあります。

</details>

## 設定方法

リポジトリルートの`composer.json`に以下を追記します。

* composer.json
```json
{
    "require-dev": {
        "gild/github-template": "^1.0"
    },
    "scripts": {
        "post-autoload-dump": [
            ". vendor/gild/github-template/execution.sh"
        ]
    }
}
```
