# GAS（JS）のTIPS

## 謎のカンマを消す
GoogleFormの内容を受けとって出力する時に以下のような謎のカンマが入る時がある
```
送信内容,,, 送信内容
```
そんな時は
```
// formのパラメータがe, Formの項目名がtext
e.namedValues[text].filter(Boolean)} 
```