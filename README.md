有価証券報告書と四半期報告書を取得するプログラム

1.提出書類の一覧を取得するAPIを実行
　https://disclosure.edinet-fsa.go.jp/api/v1/documents.json?date=YYYY-MM-DD&type=2
　引数 YYYYMMDD 提出日を指定

2.有価証券報告書と四半期報告書が提出されている場合は次へ
　有価証券報告書　　　　ordinanceCode 010　from_code 030000
  有価証券報告書（訂正）ordinanceCode 010　from_code 030001
  四半期報告書　　　　　ordinanceCode 010　from_code 043000
  四半期報告書（訂正）　ordinanceCode 010　from_code 043001

3.報告書を取得するAPIを実行する
　https://disclosure.edinet-fsa.go.jp/api/v1/documents/XXXX?type=1
　