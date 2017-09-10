# gettxout メソッド

指定されたハッシュとインデックスに基づいて、対応するトランザクション出力情報（returned change）を返します。

## パラメータ説明

txid: トランザクションID

n: トランザクション内の出力(vout)のインデックス (ゼロベース)

## 例

リクエスト:

```json
{
   "jsonrpc": "2.0",
   "method": "gettxout",
   "params": ["f4250dab094c38d8265acc15c366dc508d2e14bf5699e12d9df26577ed74d657", 0],
   "id": 1
}
```

レスポンス:

```json
{
   "jsonrpc": "2.0",
   "id": 1,
   "result": {
     "N": 0,
     "Asset": "c56f33fc6ecfcd0c225c4ab356fee59390af8560be0e930faebe74a6daff7c9b",
     "Value": "2950",
     "Address": "AHCNSDkh2Xs66SzmyKGdoDKY752uyeXDrt"
   }
}
```