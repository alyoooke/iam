---

copyright:

  years: 2017, 2018

lastupdated: "2017-11-16"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# 概説チュートリアル
{: #getstarted}

このチュートリアルの目的は、IBM Cloud ID Identity and Access Management (IAM) を稼働中にできるように支援することです。これは、ご使用のアカウントにユーザーを招待し、それらのユーザーに Cloud IAM アクセス権限を割り当てることによって行われます。

このチュートリアルは、IAM で管理されるリソースを対象としています。 アクセス管理のための Cloud IAM ポリシーの作成をサポートしていないサービスには、[Cloud Foundry アクセス権限](/docs/iam/cfaccess.html#cfaccess)を使用できます。


## ステップ 1: ユーザーを招待し、初期アクセス権限を割り当てる

1 人または複数のユーザーを招待し、招待時にユーザーの初期アクセス・ポリシーを設定することができます。 1 回の招待で複数のユーザーを招待する場合、各ユーザーに同じアクセス権限が割り当てられます。 「ユーザーの招待」ページの「アクセス権限」セクションには、割り当てを実行できるよう許可されているセクションのみが表示されます。

アカウント所有者は、「サービス」セクションで、招待するユーザーの Cloud IAM 役割を割り当てることができます。 リソース・グループ内のすべてのリソースへのアクセス権限、リソース・グループ内の特定のサービス用のすべてのリソースへのアクセス権限、アカウント内のすべての ID およびアクセス対応サービスへのアクセス権限、または、単一リソースへのアクセス権限を、招待で割り当てる初期ポリシーにおいて提供することができます。

1. **「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」**に移動して、**「ユーザー」**を選択します。
2. **「ユーザーの招待」**をクリックします。
3. 招待するユーザーの E メール・アドレスを指定します。
4. **「アクセス権限」**セクションで、**「サービス」**オプションを展開します。
5. **リソース**へのアクセス権限を割り当てるのか、**リソース・グループ**内のリソースへのアクセス権限を割り当てるのかを選択します。
6. 選択に応じて、プロンプトに従って、個別サービス・インスタンスへのアクセス権限、すべての ID およびアクセス対応サービスへのアクセス権限、リソース・グループ内のすべてのリソースへのアクセス権限、または、選択したリソース・グループ内の特定のサービスへのアクセス権限を指定します。 リソース・グループのオプションを選択した場合、そのリソース・グループにアクセスするための役割を選択することによって、リソースへのアクセス権限の表示、編集、または管理を行うことのできる権限をユーザーに提供することもできます。
7. 許可がある場合は、招待時に Cloud Foundry アクセス権限またはインフラストラクチャー・アクセス権限を割り当てることもできます。
8. **「ユーザーの招待」**をクリックします。

詳しくは、[ユーザーの招待とアクセス権限の割り当て](/docs/iam/iamuserinv.html#iamuserinv)を参照してください。

## ステップ 2: 既存ユーザーのアクセス権限の管理

ユーザーを招待して初期アクセス権限を割り当てた後で、アカウント内のすべてのユーザーのアクセス・レベルを目標通りにするために、追加のアクセス権限を割り当てたり、割り当て済みの初期アクセス権限を編集したりする必要が生じることがあります。

### 新規アクセス権限の割り当て

リソース・グループまたは単一リソースに対するアクセス権限をユーザーに割り当てることができます。

1. メニュー・バーで、**「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」**をクリックして、**「ユーザー」**を選択します。
2. アクセス権限を割り当てるユーザーの名前をクリックします。
3. **「アクセス権限の割り当て (Assign access)」**をクリックします。
4. 次のようにして、アクセス権限をどのように割り当てるのかを選択します。
    * グループ内のすべてのリソースへのアクセス権限を割り当てるか、グループ内の特定のサービス用のリソースのみへのアクセス権限を割り当てる場合は、**「リソース・グループ内のアクセス権限の割り当て (Assign access within a resource group)」**を選択します。 リソース・グループにアクセスするための役割を選択することによって、リソース・グループへのアクセス権限の表示、編集、または管理を行うことのできる権限をユーザーに提供することもできます。 指定されたリソースへのアクセス権限のみをユーザーに付与し、そのリソースが編成されているグループへのアクセス権限は付与しない場合は、**「アクセス権限なし」**を選択します。
    * アカウント全体のすべての ID およびアクセス対応リソースへのアクセス権限を割り当てるか、アカウント全体の特定サービスのすべてのリソースへのアクセス権限を割り当てるか、単一インスタンスへのアクセス権限を割り当てるか、または、特定のサービス・インスタンス内の単一リソースへのアクセス権限を割り当てる場合は、**「リソースへのアクセス権限の割り当て (Assign access to resources)」**を選択します。
5. アクセス有効範囲を定義する役割の組み合わせを選択します。 詳しくは、[Cloud IAM の役割](/docs/iam/users_roles.html#iamusermanrol)を参照してください。
6. **「割り当て」**をクリックします。


### 既存のアクセス権限の編集

ユーザーに割り当てられた役割を編集することによって、既存のアクセス権限を更新することができます。

1. メニュー・バーで、**「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」**をクリックして、**「ユーザー」**を選択します。
2. アクセス権限を編集する対象のユーザーの名前を選択します。
3. 編集するポリシーの行で、**「アクション」**メニューから**「ポリシーの編集」**をクリックします。
4. 割り当てられた役割を更新してポリシーを編集します。
5. **「保存」**をクリックします。

削除したいポリシーの**「アクション」**メニューから**「削除」**をクリックすることによって、ユーザーからアクセス権限を除去できます。

## 次のステップ

[Cloud IAM の機能](/docs/iam/index.html#features)リストで、Cloud IAM で他に何を行うことができるのかを検討してください。