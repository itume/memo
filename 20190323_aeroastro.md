# Rails meets Protocol Buffers - For Schema First Development

## Game開発にRailsなんで？

ランタイムにおいて許容可能なOHがあれば非常に開発効率が高いので
ほとんどのAPIは数十ミリ秒で返せるように作れるはず

## スキーマファースト開発とは

### スキーマ is なに？

データ構造を説明するための設計
Interface定義
OpenAPI/Yaml/GraphQL

スキーマ決めたら自動でコード/Doc/Mockが生成される世界が素敵

## ProtocolBuffer

HTTP通信のうち、bodyのコードをProtocolBufferを使っている
* JSON Schemaより読み書きしやすい
* メモリのfootprointが少ない
* バイナリ、数字について自然な表現ができる
* リファクタリングに強い
* serializetion/desirializationのコストが安い

ただし、curlでリクエスト手投げするとき辛いので対策が必要


