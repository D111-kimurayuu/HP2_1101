<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>お問い合わせフォーム</title>
</head>
    <style>
        .title1{
            color: brown;
            text-align: center;
        }
        .Form{
            max-width: 720px;
            background-color: antiquewhite;
            margin: 0 auto;
        }
        .Form-Item{
            display: flex;
            align-items: center;
            border-top: 1px solid #420142;
            font-weight: bold;
        }
        .Form-Item-Label{
            width: 100%;
            max-width: 248px;
        }
        .Form-Item-Input{
            background-color: #ffa07a;
        }
        .Form-Item-Label-Required{
            border: 2px solid orange;
            background-color: orange;
            padding: 4px;
            display: inline-block;
            border-radius: 10px;;
        }
        .Form-Item-Textarea{
            height: 200px;
            width: 400px;
            background-color: #ffa07a;
            border: 2px solid black;
        }
        .Form-Btn{
            display: block;
            margin: 0 auto;
        }

    </style>
<body>
    <h1 class="title1">お問い合わせフォームサンプル</h1>
    <form action="#" method="get">
        <div class="Form">
            <div class="Form-Item">
                <p class="Form-Item-Label"><span class="Form-Item-Label-Required">必須</span>氏名</p>
                <div class="box1"><input type="text" name="name" class="Form-Item-Input" placeholder="例） 電子太郎" required></div>
            </div>
            <div class="Form-Item">
                <p class="Form-Item-Label"><span
                     class="Form-Item-Label-Required Form-Btn-Free ">任意</span>電話番号</p>
                <input type="text" name="tel" class="Form-Item-Input" placeholder="例）000-0000-0000">
            </div>
            <div class="Form-Item">
                <p class="Form-Item-Label"><span class="Form-Item-Label-Required">必須</span>メールアドレス</p>
                <input type="email" name="mail" class="Form-Item-Input" placeholder="例）example@abc.com" required>
            </div>
            <div class="Form-Item">
                <p class="Form-Item-Label isMsg"><span class="Form-Item-Label-Required">必須</span>お問い合わせ内容</p>
                <textarea class="Form-Item-Textarea" name="inquiry" required></textarea>
            </div>
            <div class="Form-Item">
                <p class="Form-Item-Label"><span class="Form-Item-Label-Required Form-Btn-Free">任意</span>興味があるもの</p>   
                <input type="checkbox" id="HTML" name="interest" value="HTML">
                <label for="HTML">HTML</label> 
                <input type="checkbox" id="css" name="interest" value="css">
                <label for="css">css</label>
                <input type="checkbox" id="JavaScript" name="interest" value="JavaScript">
                <label for="JavaScript">JavaScript</label>   
            </div>
            <div class="Form-Item">
                <p class="Form-Item-Label"><span class="Form-Item-Label-Required">必須</span>お知らせメール</p>
                <label><input type="radio" name="ml" value="送信してもよい" checked required>送信してもよい</label>
                <label><input type="radio" name="ml" value="送信しない">送信しない</label>
            </div><input type="submit" class="Form-Btn" value="送信する">
        </div>
    </form>  
</body>
</html>
