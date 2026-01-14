# Slot2 - スロットマシン

> ⚠️ **α版（アルファ版）** - このプラグインは現在開発中です。バグが存在する可能性があります。

GUIベースのスロットマシンゲームです。

---

## ⚠️ 前提プラグイン（必須）

**[EmeraldBank](https://github.com/henntekosennsi1-rgb/EmeraldBank)** が必要です！

### インストール手順

1. [EmeraldBank](https://github.com/henntekosennsi1-rgb/EmeraldBank/releases) をダウンロード
2. [Slot2](https://github.com/henntekosennsi1-rgb/Slot2/releases) をダウンロード
3. 両方の.jarファイルを `plugins` フォルダに配置
4. サーバーを再起動

---

## 機能

### 目押し機能
- リール回転中に停止ボタンをクリック
- 設定された「滑りコマ数」分だけ先に進んで停止
- `slip_frames: 0` で完全目押し

### 確変モード
- ダイヤ3つ揃いで確変突入
- 確変中は100回転（設定可能）
- ダイヤ出現率アップ

### シンボルと配当

| シンボル | 配当倍率 |
|---------|---------|
| ダイヤモンド | 10倍 |
| 金インゴット | 5倍 |
| 鉄インゴット | 3倍 |
| 石炭 | 0.5倍 |
| バリア | 0倍 |

---

## コマンド

| コマンド | 説明 | 権限 |
|---------|------|------|
| `/slot` | スロットGUIを開く | `slot2.use` |
| `/slot remote` | リモートアイテム取得 | `slot2.remote` |

---

## 設定
```yaml
reel:
  spin_speed: 2        # 回転速度
  slip_frames: 1       # 滑りコマ数

symbols:
  DIAMOND:
    normal_weight: 7
    kakuhen_weight: 15
    multiplier: 10.0

kakuhen:
  diamond_turns: 100   # 確変回転数
```

---

## 動作環境

- **[EmeraldBank](https://github.com/henntekosennsi1-rgb/EmeraldBank)（必須）**
- Spigot/Paper 1.21.x
- Java 17以上

## コミュニティ

**Discord:** https://discord.gg/zYY55dzhjd

## ライセンス

All Rights Reserved
