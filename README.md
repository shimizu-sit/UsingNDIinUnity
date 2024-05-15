# UsingNDIinUnity
 Transmission Project Using NDI in Unity

## 目的
本学のMetaverse Labで映像を投影するためには，映像出力用PCへNDIを使って映像を送信する必要があります．
投影したい映像は大体がUnityで作られます．
なので，UnityからNDI経由で映像を送信する手順を学ぶためにこのプロジェクトを作成しました．

## 開発環境
- MacBook Air M2 MacOS Sonoma 14.4.1
- Unity 2022.3.23
- [NDI plugin for Unity](https://github.com/keijiro/KlakNDI)
- NDI Tools 6.0.1.0

## メモ
KlakNDIはフレーム画像の寸法が16x8の倍数である必要があります．16x9が一般的なので計算をする必要があります．そのために幅を16:9基準に揃えた場合の高さを表にまとめておきます．

|  幅  | 高さ |   近いサイズ名称   |
| ---- | ---- | ------------------ |
| 1920 | 960  | Full HD            |
| 2560 | 1280 | Wide Quad HD(WQHD) |
| 3840 | 1920 | 4K/UHD             |
| 7680 | 3840 | 8K/SHV             |

## 参考サイト
- [NDI plugin for Unity](https://github.com/keijiro/KlakNDI)
- [KlakNDIのセットアップ 2.0.3 #Unity - Qiita](https://qiita.com/mu5dvlp/items/9fafe65df012c6d0835d)