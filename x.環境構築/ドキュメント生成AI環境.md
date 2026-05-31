# ドキュメント生成AI環境

---

## 目次

- [ドキュメント生成AI環境](#ドキュメント生成ai環境)
  - [目次](#目次)
  - [**VSCodeインストール・セットアップ**](#vscodeインストールセットアップ)
    - [１．VSCodeダウンロード](#１vscodeダウンロード)
      - [①　ダウンロードページを開く。](#ダウンロードページを開く)
      - [②　インストールファイルをダウンロードする。](#インストールファイルをダウンロードする)
    - [２．VS Codeインストール](#２vs-codeインストール)
      - [①　ダウンロードしたファイルを実行する。](#ダウンロードしたファイルを実行する)
      - [②　「同意する」を選択して次へをクリックする。](#同意するを選択して次へをクリックする)
      - [③　インストール先のフォルダを指定する。](#インストール先のフォルダを指定する)
      - [④　スタートメニューフォルダー名を指定する。](#スタートメニューフォルダー名を指定する)
      - [⑤　インストール時に追加する機能を選択する。](#インストール時に追加する機能を選択する)
      - [➅　インストール内容を確認して次へをクリックする。](#インストール内容を確認して次へをクリックする)
      - [➆　インストール中](#インストール中)
      - [➇　インストール完了](#インストール完了)
      - [➈　GitHubへの接続画面](#githubへの接続画面)
    - [２．VS Codeの日本語化](#２vs-codeの日本語化)
      - [①　拡張機能インストール画面を表示し、テキストボックスに「Japanese Language Pack」を入力する。](#拡張機能インストール画面を表示しテキストボックスにjapanese-language-packを入力する)
      - [②　右下「Change Language and Restart」をクリックし再起動する。](#右下change-language-and-restartをクリックし再起動する)
      - [③　日本語化が完了する。](#日本語化が完了する)
    - [３．Markdown関連インストール](#３markdown関連インストール)
      - [①　拡張機能インストール画面を表示し、テキストボックスに「markdown」を入力する。](#拡張機能インストール画面を表示しテキストボックスにmarkdownを入力する)
      - [② Markdown Preview Enhanced](#-markdown-preview-enhanced)
      - [③ Markdown All in One](#-markdown-all-in-one)
      - [④ Markdown Preview Mermaid Support](#-markdown-preview-mermaid-support)
      - [⑤ Markdown PDF](#-markdown-pdf)
    - [４．Cline（クライン）のインストール](#４clineクラインのインストール)
      - [①　拡張機能インストール画面を表示し、テキストボックスに「Cline」を入力する。](#拡張機能インストール画面を表示しテキストボックスにclineを入力する)
      - [②　Clineのインストールボタンをクリックする。](#clineのインストールボタンをクリックする)
        - [③　「ようこそ」画面はXで消去する。](#ようこそ画面はxで消去する)
    - [５．Gitのインストール](#５gitのインストール)
      - [①　拡張機能インストール画面を表示し、テキストボックスに「Git」を入力する。](#拡張機能インストール画面を表示しテキストボックスにgitを入力する)
      - [②　Git Graph](#git-graph)
      - [③　Git History](#git-history)
      - [④　GitLens - Git supercharged](#gitlens---git-supercharged)
  - [GoogleAIアカウントとAPIキーの取得](#googleaiアカウントとapiキーの取得)
    - [①　Google AI StudioのWebサイトにアクセスする。](#google-ai-studioのwebサイトにアクセスする)
    - [②　Google AI StudioのWebサイトにアクセスする。](#google-ai-studioのwebサイトにアクセスする-1)
    - [③　規約と説明](#規約と説明)
    - [③　APIキーの取得](#apiキーの取得)
  - [GitHubアカウント](#githubアカウント)
    - [①　GitHubのWebサイトにアクセスする。](#githubのwebサイトにアクセスする)
    - [②　サインアップの必要事項を入力する。](#サインアップの必要事項を入力する)
    - [③　GitHubにログインする。](#githubにログインする)
    - [④　GitHubにE-Emailアドレスを設定する。](#githubにe-emailアドレスを設定する)
  - [VSCodeとGoogle AIの連携設定](#vscodeとgoogle-aiの連携設定)
    - [①　CLINEの画面を表示する。](#clineの画面を表示する)
    - [②　「Bring my own API key」を選択してContinueをクリックする。](#bring-my-own-api-keyを選択してcontinueをクリックする)
    - [③　GoogleAPIを設定する。](#googleapiを設定する)
    - [⑤　設定完了](#設定完了)
  - [VSCodeとGitHubの連携設定](#vscodeとgithubの連携設定)
    - [１．Gitのインストール](#１gitのインストール)
    - [①　GitのWebサイトを表示する。](#gitのwebサイトを表示する)
    - [２．sshキーの取得と設定](#２sshキーの取得と設定)
      - [①　sshキーを取得する。](#sshキーを取得する)
      - [②　sshキーをGitHubに設定する。](#sshキーをgithubに設定する)
      - [③　ssh接続ができているか確認する。](#ssh接続ができているか確認する)
    - [３．リポジトリを開く](#３リポジトリを開く)
      - [①　ソース管理画面から「リポジトリをクローンする」をクリックする。](#ソース管理画面からリポジトリをクローンするをクリックする)
      - [②　VSCode上部の「GitHubから複製」をクリックする。](#vscode上部のgithubから複製をクリックする)
      - [③　GitHubのサインインを許可する。](#githubのサインインを許可する)
      - [④　リポジトリを選択する。](#リポジトリを選択する)
      - [⑤　リポジトリをダウンロードするフォルダを指定する。](#リポジトリをダウンロードするフォルダを指定する)
      - [➅　リポジトリを開く](#リポジトリを開く)

---

## **VSCodeインストール・セットアップ**

### <u>１．VSCodeダウンロード</u>

#### ①　ダウンロードページを開く。

[ダウンロードページ](https://code.visualstudio.com/)
![ダウンロード画面](./①VSCode/インストール/01.png)

#### ②　インストールファイルをダウンロードする。

![ダウンロード画面](./①VSCode/インストール/03.png)
![ダウンロード画面](./①VSCode/インストール/02.png)

### <u>２．VS Codeインストール</u>

#### ①　ダウンロードしたファイルを実行する。

#### ②　「同意する」を選択して次へをクリックする。
![ログイン画面](./①VSCode/インストール/04.png)

#### ③　インストール先のフォルダを指定する。
任意のフォルダを指定できるが、デフォルトで問題ない。
![ログイン画面](./①VSCode/インストール/05_1.png)
![ログイン画面](./①VSCode/インストール/05_2.png)

#### ④　スタートメニューフォルダー名を指定する。
デフォルトで問題ない。
![ログイン画面](./①VSCode/インストール/06.png)

#### ⑤　インストール時に追加する機能を選択する。
デフォルトで問題ない。
![ログイン画面](./①VSCode/インストール/07_1.png)
![ログイン画面](./①VSCode/インストール/07_2.png)

#### ➅　インストール内容を確認して次へをクリックする。
![ログイン画面](./①VSCode/インストール/08.png)

#### ➆　インストール中
![ログイン画面](./①VSCode/インストール/09.png)

![ログイン画面](./①VSCode/インストール/10.png)

![ログイン画面](./①VSCode/インストール/11.png)

#### ➇　インストール完了
![ログイン画面](./①VSCode/インストール/12.png)

#### ➈　GitHubへの接続画面
GitHubへの接続画面が表示された場合は、別途実施するので「X」で消去する。
![ログイン画面](./①VSCode/インストール/13.png)

---

### <u>２．VS Codeの日本語化</u>

#### ①　拡張機能インストール画面を表示し、テキストボックスに「Japanese Language Pack」を入力する。
![ログイン画面](./①VSCode/日本語化/03.png)

#### ②　右下「Change Language and Restart」をクリックし再起動する。
![ログイン画面](./①VSCode/日本語化/04.png)

#### ③　日本語化が完了する。
![ログイン画面](./①VSCode/日本語化/05.png)

---

### <u>３．Markdown関連インストール</u>

#### ①　拡張機能インストール画面を表示し、テキストボックスに「markdown」を入力する。
![ログイン画面](./①VSCode/Markdown/01.png)

#### ② Markdown Preview Enhanced
Markdown Preview Enhancedのインストールボタンをクリックしてインストールする。
Markdownの書式で記載したドキュメントのプレビュー機能を持つ。
![ログイン画面](./①VSCode/Markdown/02_1.png)
![ログイン画面](./①VSCode/Markdown/02_2.png)

#### ③ Markdown All in One
Markdown All in Oneのインストールボタンをクリックしてインストールする。
Markdownの書式で記載したドキュメントに、目次の自動生成、キーボードのショートカット、見出しのナンバリング等の機能を持つ。
![ログイン画面](./①VSCode/Markdown/03_1.png)
![ログイン画面](./①VSCode/Markdown/03_2.png)

#### ④ Markdown Preview Mermaid Support
Markdown Preview Mermaid Supportのインストールボタンをクリックしてインストールする。
Markdownの書式で記載したドキュメントのMermaid書式部分をプレビュー時に図として表示する機能を持つ。
![ログイン画面](./①VSCode/Markdown/04_1.png)
![ログイン画面](./①VSCode/Markdown/04_2.png)

#### ⑤ Markdown PDF
Markdown PDFのインストールボタンをクリックしてインストールする。
Markdownの書式で記載したドキュメントをPDFに変換する機能を持つ。
![ログイン画面](./①VSCode/Markdown/05_1.png)
![ログイン画面](./①VSCode/Markdown/05_2.png)

---

### <u>４．Cline（クライン）のインストール</u>

#### ①　拡張機能インストール画面を表示し、テキストボックスに「Cline」を入力する。
![ログイン画面](./①VSCode/Cline/03.png)

#### ②　Clineのインストールボタンをクリックする。
![ログイン画面](./①VSCode/Cline/04.png)
![ログイン画面](./①VSCode/Cline/05.png)

##### ③　「ようこそ」画面はXで消去する。
![ログイン画面](./①VSCode/Cline/06.png)

---

### <u>５．Gitのインストール</u>

#### ①　拡張機能インストール画面を表示し、テキストボックスに「Git」を入力する。
![ログイン画面](./①VSCode/Git/01.png)

#### ②　Git Graph
Git Graphのインストールボタンをクリックしてインストールする。
![ログイン画面](./①VSCode/Git/02.png)

#### ③　Git History
Git Graphのインストールボタンをクリックしてインストールする。
![ログイン画面](./①VSCode/Git/04.png)

#### ④　GitLens - Git supercharged
GitLens - Git superchargedのインストールボタンをクリックしてインストールする。
![ログイン画面](./①VSCode/Git/05.png)
![ログイン画面](./①VSCode/Git/06.png)

---

## GoogleAIアカウントとAPIキーの取得

### ①　Google AI StudioのWebサイトにアクセスする。
Webブラウザに「https://aistudio.google.com」を入力する。
Get started をクリックする。
![ログイン画面](./②GoogleAI/03.png)
### ②　Google AI StudioのWebサイトにアクセスする。
メールアドレス（Google GMail）を入力する。
本人確認を実施する。
![ログイン画面](./②GoogleAI/04.png)
![ログイン画面](./②GoogleAI/05.png)
![ログイン画面](./②GoogleAI/06.png)
![ログイン画面](./②GoogleAI/07.png)
![ログイン画面](./②GoogleAI/08.png)
![ログイン画面](./②GoogleAI/08_.png)
![ログイン画面](./②GoogleAI/09.png)
![ログイン画面](./②GoogleAI/10.png)
### ③　規約と説明
図のようにチェックして続行する。
![ログイン画面](./②GoogleAI/12.png)
Nextをクリック
![ログイン画面](./②GoogleAI/13.png)
Nextをクリック
![ログイン画面](./②GoogleAI/14.png)
Nextをクリック
![ログイン画面](./②GoogleAI/15.png)
### ③　APIキーの取得
「Get API Key」をクリックする。
![ログイン画面](./②GoogleAI/17.png)
「APIキーを作成」をクリックする。
![ログイン画面](./②GoogleAI/18.png)
キー名を入力する。（任意ですが合わせておく）
![ログイン画面](./②GoogleAI/20.png)
![ログイン画面](./②GoogleAI/25.png)
プロジェクト名を入力する。（任意ですが合わせておく）
![ログイン画面](./②GoogleAI/26.png)
![ログイン画面](./②GoogleAI/27.png)
![ログイン画面](./②GoogleAI/28.png)
![ログイン画面](./②GoogleAI/29.png)
「キーを作成」をクリックする。
![ログイン画面](./②GoogleAI/30.png)
![ログイン画面](./②GoogleAI/31.png)
![ログイン画面](./②GoogleAI/32.png)

---

## GitHubアカウント

<u>**アカウントは作成済のためこの手順は実施不要です。**</u>

### ①　GitHubのWebサイトにアクセスする。
Webブラウザに「https://github.co.jp」を入力する。
「サインアップ」をクリックする。
![ログイン画面](./③GitHub/01.png)

### ②　サインアップの必要事項を入力する。
Cチーム用にアカウントを作成する。
パスワードはVitalの共通パスワードとした。
![ログイン画面](./③GitHub/02.png)
![ログイン画面](./③GitHub/03.png)
必要事項を入力後「Create account」をクリックする。
![ログイン画面](./③GitHub/04.png)
![ログイン画面](./③GitHub/05.png)
登録したE-Mailにコードが届くので入力する。
![ログイン画面](./③GitHub/06.png)

### ③　GitHubにログインする。
![ログイン画面](./③GitHub/07.png)
![ログイン画面](./③GitHub/08.png)

### ④　GitHubにE-Emailアドレスを設定する。
右上のアイコンをクリックし、メニューから「Settings」を選択する。
![ログイン画面](./③GitHub/09.png)
左のメニューから「Emails」を選択する。
![ログイン画面](./③GitHub/10.png)
「Keep my email addresses private」をONに設定する。
これでGitHub用のEmailアドレスが使用できる。
![ログイン画面](./③GitHub/11.png)

---

## VSCodeとGoogle AIの連携設定

### ①　CLINEの画面を表示する。
![ログイン画面](./④VSCode_GoogleAI/01.png)
### ②　「Bring my own API key」を選択してContinueをクリックする。
![ログイン画面](./④VSCode_GoogleAI/02.png)
### ③　GoogleAPIを設定する。
![ログイン画面](./④VSCode_GoogleAI/03.png)
API Provider : Google Gemini
Gemini API Key : Google AI Studioで取得したAPIキーを入力する。
![ログイン画面](./④VSCode_GoogleAI/04.png)
### ⑤　設定完了
「X」で消去
![ログイン画面](./④VSCode_GoogleAI/05.png)
![ログイン画面](./④VSCode_GoogleAI/06.png)

---

## VSCodeとGitHubの連携設定

### １．Gitのインストール

### ①　GitのWebサイトを表示する。
「Install for Windows」をクリックする。
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/01.png)
「Git for windwos/x64 Setup.」をクリックする。
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/02.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/03.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/04.png)
ダウンロードしたファイルを実行する。
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/05.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/06.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/07.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/08.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/10.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/11.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/12.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/13.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/15.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/16.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/17.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/18.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/19.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/20.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/21.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/22.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/23.png)
![ログイン画面](./⑤VSCode_GitHub/Gitインストール/24.png)

### ２．sshキーの取得と設定

#### ①　sshキーを取得する。

git --version  
git config --global user.name VitalTeamC  
git config --global user.email GitHub用のEmailアドレスを入力する。  
ssh-keygen -t rsa  
clip < .ssh/id_rsa.pub　　　　　← Keyがクリップボードにコピーされる。  
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/01.png)
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/02.png)

#### ②　sshキーをGitHubに設定する。
「New SSH key」をクリックする。
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/03.png)

Title：　任意だが、利用者が特定できる名称とする。  
Key type：　変更なし  
Key：　クリップボードからCtrl + vでペーストする。  
入力後に「Add SSH Key」をクリックする。
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/04.png)
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/06.png)

パスワード（Vital標準）を入力してConfirmをクリックする。
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/07.png)

設定完了
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/08.png)

#### ③　ssh接続ができているか確認する。

ssh -T git@github.com
![ログイン画面](./⑤VSCode_GitHub/sshキー取得と登録/09.png)

### ３．リポジトリを開く

#### ①　ソース管理画面から「リポジトリをクローンする」をクリックする。
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/01.png)
#### ②　VSCode上部の「GitHubから複製」をクリックする。
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/02.png)
#### ③　GitHubのサインインを許可する。
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/03.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/04.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/05_1.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/05_2.png)
#### ④　リポジトリを選択する。
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/06.png)
#### ⑤　リポジトリをダウンロードするフォルダを指定する。
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/07_1.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/07_2.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/08.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/09.png)
#### ➅　リポジトリを開く
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/10.png)
![ログイン画面](./⑤VSCode_GitHub/リポジトリを開く/11.png)







