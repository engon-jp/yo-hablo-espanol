# 音声ファイルの置き場所

このフォルダに、各フレーズの音声ファイルを置きます。

- **配置済み（2026-06-28）**：`phrase_01.mp3`〜`phrase_48.mp3` を配置済み。
- 生成時のパラメータ・手順（ElevenLabs設定・分割方法・再現手順）は [音声生成メモ.md](音声生成メモ.md) を参照。

## 命名規則（必須）
- ファイル名は `phrase_01.mp3` 〜 `phrase_48.mp3`（2桁ゼロ埋め）。
- 番号は仕様書／アプリ内マスターデータの問題番号（id 1〜48）と一致させること。
  - 例：id 1「Yo hablo español.」→ `phrase_01.mp3`
  - 例：id 36「Ellas escriben un mensaje.」→ `phrase_36.mp3`
- 形式は `.mp3` を推奨（ほぼ全ブラウザ・スマホで再生可）。

## 動作
- アプリは回答後に再生ボタンが有効になり、`assets/audio/phrase_XX.mp3` を再生します。
- **ファイルがまだ無い場合**は、端末内蔵の音声合成（Web Speech API・スペイン語 `es-ES`）で自動的に代替読み上げします。
- mp3 を置けば自動的にそちらが優先されます（コード変更不要）。

## 注意
- ブラウザのキャッシュにより、差し替え後すぐ反映されないことがあります。スーパーリロード（Mac: ⌘+Shift+R）で更新してください。
- ファイル名の番号がずれると別フレーズの音声が鳴るので、対応表（下記）で確認を。

## 対応表（id → 正解文）
| id | 音声ファイル | スペイン語文 |
|----|------------|-------------|
| 01 | phrase_01.mp3 | Yo hablo español. |
| 02 | phrase_02.mp3 | ¿Tú hablas inglés? |
| 03 | phrase_03.mp3 | Nosotros no hablamos japonés. |
| 04 | phrase_04.mp3 | Ellos hablan chino. |
| 05 | phrase_05.mp3 | Él no come un tomate. |
| 06 | phrase_06.mp3 | Ella come un huevo. |
| 07 | phrase_07.mp3 | Nosotras comemos una naranja. |
| 08 | phrase_08.mp3 | Ellas no comen una manzana. |
| 09 | phrase_09.mp3 | Usted vive en Tokio. |
| 10 | phrase_10.mp3 | Él no vive en Madrid. |
| 11 | phrase_11.mp3 | ¿Ustedes viven en Barcelona? |
| 12 | phrase_12.mp3 | Vosotras vivís en Buenos Aires. |
| 13 | phrase_13.mp3 | Yo no estudio chino. |
| 14 | phrase_14.mp3 | Tú estudias español. |
| 15 | phrase_15.mp3 | Nosotros estudiamos inglés. |
| 16 | phrase_16.mp3 | Ustedes no estudian japonés. |
| 17 | phrase_17.mp3 | Ella bebe agua. |
| 18 | phrase_18.mp3 | ¿Tú bebes vino? |
| 19 | phrase_19.mp3 | Vosotros no bebéis cerveza. |
| 20 | phrase_20.mp3 | Ellos beben leche. |
| 21 | phrase_21.mp3 | Usted no abre la boca. |
| 22 | phrase_22.mp3 | Yo abro el paquete. |
| 23 | phrase_23.mp3 | Nosotros abrimos la ventana. |
| 24 | phrase_24.mp3 | Ellas no abren la puerta. |
| 25 | phrase_25.mp3 | Yo compro un coche. |
| 26 | phrase_26.mp3 | Tú no compras una flor. |
| 27 | phrase_27.mp3 | ¿Ustedes compran un regalo? |
| 28 | phrase_28.mp3 | Vosotras compráis una bicicleta. |
| 29 | phrase_29.mp3 | Él no lee un libro. |
| 30 | phrase_30.mp3 | Ella lee un periódico. |
| 31 | phrase_31.mp3 | Ustedes leen una revista. |
| 32 | phrase_32.mp3 | Ellos no leen una novela. |
| 33 | phrase_33.mp3 | Ella escribe una carta. |
| 34 | phrase_34.mp3 | Usted no escribe un correo. |
| 35 | phrase_35.mp3 | ¿Vosotros escribís una postal? |
| 36 | phrase_36.mp3 | Ellas escriben un mensaje. |
| 37 | phrase_37.mp3 | Él habla español. |
| 38 | phrase_38.mp3 | Nosotros no hablamos inglés. |
| 39 | phrase_39.mp3 | Yo no como una manzana. |
| 40 | phrase_40.mp3 | Vosotros coméis un huevo. |
| 41 | phrase_41.mp3 | Tú vives en Madrid. |
| 42 | phrase_42.mp3 | Ellos no viven en Tokio. |
| 43 | phrase_43.mp3 | Él no bebe cerveza. |
| 44 | phrase_44.mp3 | Nosotras bebemos agua. |
| 45 | phrase_45.mp3 | Ella abre el paquete. |
| 46 | phrase_46.mp3 | Vosotras no abrís la puerta. |
| 47 | phrase_47.mp3 | ¿Usted compra un regalo? |
| 48 | phrase_48.mp3 | Ellas no escriben una carta. |
