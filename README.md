# オプティカルフローの基礎

`Pyramidal Lucas-kanade法` vs `Farneback法`
| 手法   | Lucas-Kanade (Pyramidal) | Farneback   |
| ---- | ------------------------ | ----------- |
| 基本   | 特徴点を追跡                   | 画像全体のフロー    |
| 出力   | Sparse (まばら)             | Dense (密)   |
| 計算量  | 軽い                       | 重い          |
| 精度   | 特徴点付近では高精度               | 全体的にそこそこ  |
| 典型用途 | トラッキング             | 動きの可視化 |

- 「点を追いかけたい」 → Lucas-Kanade
- 「全部のピクセルの動きを見たい」 → Farneback

## Pyramidal Lucas-kanade法のデモ
10個の特徴点に対してトラッキングした結果

https://github.com/user-attachments/assets/54503850-672a-4950-9792-15acd2230aac

## Farneback法のデモ
*ベクトルの向きによって色が変わる

https://github.com/user-attachments/assets/a21b351a-0dbb-4959-a044-97e115821861
