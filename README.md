# LINE アプリで簡単に作れる AI チャットボット！ ChatGPT 連携

- OpenAI の設定

  1. アカウント作成

     「[Create your account](https://platform.openai.com/signup)」画面にアクセスし、OpenAI のアカウントを作成  
     ![OpenAI 1](img/openai-01.png)

  1. ログイン

     「[Create your account](https://platform.openai.com/signup)」画面にアクセス後、「Log in」リンクをクリックし、ログイン画面を表示後、ログインを実施  
     ![OpenAI 2](img/openai-02.png)

  1. 「API Keys」画面に遷移

     右上の「Personal」をクリック後、「View API keys」をクリックし、「API kyes」画面に遷移  
     ![OpenAI 3](img/openai-03.png)

  1. 「Create new secret key」ダイアログを表示

     「+ Create new secret key」をクリックし、「Create new secret key」ダイアログを表示
     ![OpenAI 4](img/openai-04.png)

  1. secret key の発行

     「Name」に「hands-on」と入力し、「Create secret key」ボタンをクリック
     ![OpenAI 5](img/openai-05.png)

  1. 「secret key」をコピー

     「Create new secret key」ダイアログに表示された「コピー」ボタンをクリックし、「secret key」をコピーし、「Done」ボタンをクリック  
     ※コピーした secret key をテキストエディターにペーストしておいてください  
     ![OpenAI 6](img/openai-06.png)

- LINE Messaging API の設定

  1. LINE Business ID の作成

     以下のリンクにアクセスし、LINE Business ID のアカウントを作成してください  
     https://account.line.biz/login
     ![LINE 01](img/line-01-01.png)

  1. LINE Developers ID ログイン画面を開く

     以下のリンクの「LINE アカウントでログイン」ボタンをクリックし、ログイン画面を開く  
     https://account.line.biz/login?redirectUri=https%3A%2F%2Fdevelopers.line.biz%2Fconsole%2F  
     ![LINE 01](img/line-01-02.png)

  1. ログイン

     「LINE アカウントでログイン」をクリック後、「メールアドレス」「パスワード」を入力し、「ログイン」ボタンをクリック  
     ![LINE 02](img/line-02.png)  
     ※スマートフォンの LINE アプリ上で画面に表示された認証番号を入力する必要があります。

  1. 「新規プロバイダー作成」ダイアログを表示

     プロバイダーの「新規プロバイダー作成」ボタンをクリックし、新規プロバイダー作成ダイアログを開く  
     ![LINE 03](img/line-03.png)

  1. 新規プロバイダーを作成

     「プロバイダー名」に「hands-on」を入力し、「作成」ボタンをクリック  
     ![LINE 04](img/line-04.png)

  1. 新規チャネル作成画面を開く

     「Messaging API」をクリック
     ![LINE 05](img/line-05.png)

  1. 新規チャネルを作成

     必須項目を入力して「作成」ボタンをクリックし、確認ダイアログを表示し、「OK」ボタンをクリック  
     ※確認ダイアログが 2 回表示されますが、中身を読んだ上で「確認」ボタンをクリック  
     ![LINE 06](img/line-06.png)
     |入力項目|入力値|
     |----|----|
     |会社・事業者の所在国・地域|日本|
     |チャネル名|hands-on|
     |チャネル説明|ChatGPT hands-on|
     |大業種|飲食店・レストラン|
     |小業種|カフェ・喫茶店|
     |メールアドレス|（個人のメールアドレスを入力してください）|
     |LINE 公式アカウント利用規約 の内容に同意します|チェックボックス On|
     |LINE 公式アカウント API 利用規約 の内容に同意します|チェックボックス On|

  1. チャネル作成完了

     チャネルの作成が完了  
     ![LINE 07](img/line-07.png)

  1. 友達追加

     「Messaging API 設定」タブをクリックし、QR コードを表示し、スマホの LINE アプリで友達追加をしておいてください  
     ![LINE 08](img/line-08.png)

  1. 「応答設定」画面を開く

     「LINE 公式アカウント機能 > 応答メッセージ > 編集」リンクをクリックし、「応答設定」画面を開く  
     ![LINE 09](img/line-09.png)

  1. 「応答設定」

     応答設定を実施後、画面を閉じてください  
     ![LINE 10](img/line-10.png)
     |入力項目|入力値|
     |----|----|
     |チャット|Off|
     |あいさつメッセージ|Off|
     |Webhook|On|
     |応答メッセージ|Off|

  1. 「チャネルアクセストークン」の発行

     「LINE Developers」画面の「Messaging API 設定」タブを開き、「チャネルアクセストークン > 発行」ボタンをクリック  
     ![LINE 11](img/line-11.png)

  1. 「チャネルアクセストークン」のコピー

     発行された「チャネルアクセストークン」をコピーして、テキストに貼り付けておいてください  
     ![LINE 12](img/line-12.png)

- make の設定

  1. make アカウントの作成

     以下のリンクにアクセスし、make のアカウントを作成してください  
     https://www.make.com/en/register  
     ![make 01](img/make-01.png)

  1. make にログイン

     以下のリンクにアクセス後、「Email」「Password」を入力し、「Sign in」ボタンをクリック  
     https://www.make.com/en/login  
     ![make 02](img/make-02.png)

  1. scenario の作成

     「Create a new scenario」ボタンをクリックし、 「New scenario」画面を開く  
     ![make 03](img/make-03.png)

  1. LINE application の追加

     「+」ボタンクリック後、検索フォームに「LINE」を入力し、「LINE」を選択  
     ![make 04](img/make-04.png)

  1. 「Watch Events」 の追加

     「Watch Events」をクリック  
     ![make 05](img/make-05.png)

  1. 「Webhook」 の追加

     「Webhook」ダイアログの「Add」ボタンをクリック  
     ![make 06](img/make-06.png)

  1. 「Webhook」 の作成

     「Create a webhook」ダイアログの「Webhoook name」に「hands-on」と入力し、「Connection」の「Add」ボタンをクリック  
     ![make 07](img/make-07.png)

  1. 「connection」 の作成

     「Create a connection」ダイアログの「Connection name」に「hands-on」と入力し、「Channel Access Token」に【「チャンネルアクセストークン」のコピー】でコピーしたチャネルアクセストークンを貼り付けて「Save」ボタンをクリック  
     ![make 08](img/make-08.png)

  1. 「webhook」 の作成

     「Create a webhook」ダイアログで「Connection」に「hands-on」が設定されているのを確認し、「Save」ボタンをクリック  
     ![make 09](img/make-09.png)

  1. 「Webhook address」のコピー

     「LINE」ダイアログの「Copy address to clipboard」ボタンをクリックし、「address」をコピーし、テキストに貼り付けておいてください。貼り付けが終わったら「OK」ボタンをクリックして「LINE」ダイアログを閉じてください  
     ![make 10](img/make-10.png)

  1. 「make」を一時保存

     「Save」ボタンをクリックし、make を一時保存  
     ![make 11](img/make-11.png)

- LINE から make の連携設定

  1. Webhook 設定

     「LINE Developers」画面の「Messaging API 設定」タブの「Webhook 設定 > 編集」ボタンをクリック後、入力欄に【「Webhook address」のコピー】でコピーしたアドレスを貼り付けて「更新ボタン」をクリック  
     ![make-line 01](img/make-line-01.png)

  1. Webhook 検証

     「make」画面で「Run Once」ボタンクリック後、「LINE Developers」画面に戻り「Messaging API 設定」タブの「Webhook 設定 > 検証」ボタンをクリックし、「成功」ダイアログが表示されることを確認  
     「make」画面に戻り、LINE アイコンの右上に「1」が表示されることを確認  
     「LINE Developers」画面に戻り「Messaging API 設定」タブの「Webhook 設定 > webhook の利用」ボタンを On に変更  
     ![make-line 02](img/make-line-02.png)
     ![make-line 03](img/make-line-03.png)
     ![make-line 04](img/make-line-04.png)
     ![make-line 05](img/make-line-05.png)

  1. LINE よりメッセージ送信

     「make」画面で再度「Run Once」ボタンクリック後、【友達追加】で追加したチャットボットアカウントに LINE でメッセージを送信し、「make」画面で LINE アイコンの右上に「1」が表示されることを確認  
     ![make-line 06](img/make-line-06.png)

- make から openai の連携設定

  1. module 追加

     「make」画面で「LINE」アイコン横にカーソルを移し、表示された「+ Add another module」ボタンをクリック  
     ![make-openai 01](img/make-openai-01.png)

  1. HTTP モジュール選択

     検索フォームに「http」と入力し、「HTTP」モジュールを選択  
     ![make-openai 02](img/make-openai-02.png)

  1. Make a request モジュール選択

     ACTIONS より「Make a request」モジュールを選択  
     ![make-openai 03](img/make-openai-03.png)

  1. HTTP モジュールの設定（その 1）

     以下の値を入力  
     ![make-openai 04](img/make-openai-04.png)
     |入力項目|入力値|
     |----|----|
     |URL|https://api.openai.com/v1/chat/completions|
     |Method|POST|

  1. HTTP モジュールの設定（その 2）

     以下の値を入力  
     ![make-openai 05](img/make-openai-05.png)
     |入力項目|入力値|
     |----|----|
     |Headers > item1 > Name|Content-Type|
     |Headers > item1 > Value|application/json|
     |Headers > item2 > Name|Authorization|
     |Headers > item2 > Value|Bearer {OpenAI で発行した API キー}|

  1. HTTP モジュールの設定（その 3）

     以下の値を入力し、「OK」ボタンをクリック  
     ![make-openai 06](img/make-openai-06.png)
     |入力項目|入力値|
     |----|----|
     |Body type|Raw|
     |Content type|JSON (application/json)|
     |Request content|{"model": "gpt-3.5-turbo","messages" : [{"role": "system","content": "あなたは大阪府箕面市森町中にある喫茶店「森のひととき」の店長です。常に明るく元気に丁寧に返信してください。お店の営業時間は AM9:00〜PM18:00。休業日は水曜日。受信メッセージに `SHINMACHI` が含まれる場合は返信内容に「クーポンをお知らせします！12345」を文末または文頭に含めてください。"},{"role": "user","content": "{{1.events[].message.text}}"}]}|
     |Parse response|Yes|

  1. openai へのメッセージ送信検証

     「make」画面で「Run Once」ボタンクリック後、LINE からメッセージを送信し、「LINE」アイコン、「HTTP」アイコンの右上に「1」が表示されることを確認  
     ![make-openai 07](img/make-openai-07.png)

- make から LINE の連携設定

  1. module 追加

     「make」画面で「LINE」アイコン横にカーソルを移し、表示された「+ Add another module」ボタンをクリック  
     ![make-line 10](img/make-line-10.png)

  1. 「LINE > Send a Reply Message」の選択

     「LINE > Send a Reply Message」を選択  
     ![make-line 11](img/make-line-11.png)

  1. 「Send a Reply Message」の設定

     以下の値を入力し、「OK」ボタンをクリック  
     ![make-line 12](img/make-line-12.png)
     |入力項目|入力値|
     |----|----|
     |Connection|hands-on (hands-on)|
     |Reply Token|{{1.events[].replyToken}}|
     |Messages > item1 > Type|Text|
     |Messages > item1 > Text|{{2.data.choices[].message.content}}|

  1. openai アプリの送信検証

     「make」画面で「Run Once」ボタンクリック後、LINE からメッセージを送信し、応答が LINE で返ってくることを確認
