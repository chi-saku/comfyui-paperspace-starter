# ComfyUI Google Colab スターター

**🎨 教育用に最適化された画像生成AI環境**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/chi-saku/comfyui-google-colab-starter/blob/main/ComfyUI_for_Colab.ipynb)

**🚀 ワンクリックでComfyUIが起動する魔法のノートブック**

## ✨ 特徴

- **15秒起動**: セルを実行するだけで自動セットアップ
- **魔法のURL**: cloudflaredで外部アクセス可能なURLを自動生成
- **永続保存**: Google Driveに生成画像を自動保存
- **教育最適化**: 初心者でも迷わない詳細なガイド
- **安定動作**: メモリ最適化とエラーハンドリング完備

## 🚀 使い方

### Step 1: Colab起動
上記の「Open In Colab」バッジをクリック

### Step 2: GPU設定
1. 「ランタイム」→「ランタイムのタイプを変更」
2. 「ハードウェア アクセラレータ」を「T4 GPU」に設定
3. 「保存」をクリック

### Step 3: 実行
1. 「ランタイム」→「すべてのセルを実行」をクリック
2. 約10-15分待機（初回のみ）
3. `🎉 魔法のURL: https://xxxxx.trycloudflare.com` が表示されたらクリック
4. ComfyUIで画像生成開始！

## 📁 保存先

- **生成画像**: `/content/drive/MyDrive/ComfyUI/output/`
- **モデル**: `/content/drive/MyDrive/ComfyUI/models/checkpoints/`
- **ワークフロー**: Google Drive内で永続保存

## 🎓 教育現場での活用

### 講師の方へ
- **簡単配布**: このリンクを受講生に共有するだけ
- **統一環境**: 全員が同じ環境で学習可能
- **トラブル最小**: 詳細なエラーハンドリングで安定動作

### 学習者の方へ
- **即座開始**: 複雑なインストール作業は一切不要
- **安心学習**: Google Driveに作品が自動保存
- **段階学習**: 基本操作から高度な技術まで段階的に習得

## 🔧 トラブルシューティング

### よくある問題

**「魔法のURL」が表示されない場合**
```python
# セルを再実行してください
# または以下で状況確認
!ps aux | grep main.py
!netstat -tlnp | grep 8123
