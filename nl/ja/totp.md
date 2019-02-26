---

copyright:

  years: 2018, 2019

lastupdated: "2019-01-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:tip: .tip}
{:note: .note}

# ユーザーに対するワンタイム・パスコード MFA の有効化
{: #totp}

適切な権限を持つ管理者は、{{site.data.keyword.Bluemix}} コンソールの「ユーザーの詳細」ページで、ログイン時にユーザーに対して時間ベースのワンタイム・パスコード (TOTP) を求めるプロンプトが出されるようにするオプションを有効にすることができます。 ID ベースの MFA とは違って、このタイプの多要素認証 (MFA) は設定が有効にされているアカウントでのみ必要になります。 詳しくは、『[多要素認証のタイプ](/docs/iam?topic=iam-types#types)』を参照してください。
{:shortdesc}

以下のアクセス権限を持っている場合、アカウント内の他のユーザーに対するこの設定を更新できます。

* ユーザー管理サービスに対するエディター以上の役割
* 当該ユーザーのクラシック・インフラストラクチャー階層内で上位にいて、かつ、「ユーザーの管理」クラシック・インフラストラクチャー許可を割り当てられている

ユーザーに TOTP MFA のプロンプトが出されるようにするログイン設定をオンにするには、以下の手順を実行します。

あるユーザーに対してこの MFA オプションをオンにするには、まず、そのユーザーが、プロファイルの「ログイン設定」ページで [TOTP をセットアップ](/docs/account?topic=account-MFA#MFA)する必要があります。
{: note}

1. メニュー・バーから、**「管理」** &gt; **「アクセス (IAM)」**をクリックして、**「ユーザー」**を選択します。
2. リストからユーザーを選択します。
3. **「ユーザーの詳細」**ページの**「ユーザー・ログインの管理」**セクションで、**「時間ベースのワンタイム・パスコード MFA」**オプションをオンに設定します。

「ユーザーの詳細」ページで「ユーザー管理ログイン」設定を有効にしてもらったユーザーは、自分自身でこの設定を管理できます。
{: tip}
