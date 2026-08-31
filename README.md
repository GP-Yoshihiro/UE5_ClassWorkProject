# UE5 Class Work Project

## 概要

ゲームエンジンの授業で制作しているUnreal Engine 5（UE5）のゲームプロジェクトです。

授業内でゲーム制作を行い、GitHubを利用してプロジェクトのバージョン管理を行います。

---

## 開発環境

* **Game Engine**：Unreal Engine 5
* **Programming**：C++ / Blueprint
* **IDE**：Visual Studio
* **Version Control**：Git / GitHub
* **Git Client**：SourceTree
* **Large File Storage**：Git LFS

---

## 授業情報

**授業名**：ゲームエンジン

**授業日**：毎週火曜日

| 時限   | 時間            |
| ---- | ------------- |
| 1時間目 | 9:10 ～ 10:40  |
| 2時間目 | 10:50 ～ 12:20 |

1回の授業につき90分×2コマ、合計180分の制作時間があります。

---

## プロジェクト構成

```text
UE5_ClassWorkProject/
├─ .gitignore
├─ README.md
│
└─ UE5_ClassWrokProject/
   ├─ Config/
   ├─ Content/
   ├─ Source/
   ├─ Plugins/
   ├─ UE5_ClassWrokProject.uproject
   └─ その他UE5関連ファイル・フォルダ
```

`UE5_ClassWrokProject` フォルダ内にUnreal Engine 5のプロジェクト本体を配置しています。

---

## バージョン管理

本プロジェクトでは、GitHubを利用してバージョン管理を行います。

UE5のプロジェクトでは容量の大きいアセットやバイナリファイルを扱うため、必要に応じてGit LFSを使用します。

### 基本的な作業手順

```text
1. 最新の変更を取得
      ↓
2. 自分の担当箇所を編集
      ↓
3. UE5上で動作確認
      ↓
4. Commit
      ↓
5. GitHubへPush
```

### 作業前

他のメンバーの変更を取得してから作業を開始します。

```bash
git pull
```

### Commit

Commitメッセージは、変更内容が分かるように記述します。

例：

```text
Add player movement
Add enemy character
Fix player collision
Update player animation
Add battle system
Update UI
```

---

## 開発ルール

### 1. 作業前に最新状態を取得する

作業を開始する前に、リモートリポジトリの変更を取得します。

```bash
git pull
```

### 2. 他のメンバーの担当箇所を勝手に変更しない

他のメンバーが担当しているBlueprintやC++ファイルを変更する場合は、事前に確認します。

### 3. 動作確認してからCommit・Pushする

コンパイルエラーやゲームが正常に起動しない状態でCommit・Pushしないようにします。

### 4. Commit内容を分かりやすくする

1つのCommitに関係のない変更を大量に含めず、変更内容が分かる単位でCommitします。

### 5. Git LFSに注意する

UE5ではアセットなどのファイルサイズが大きくなるため、Git LFSで管理するファイルを確認してからPushします。

---

## ブランチ運用

基本的に`main`ブランチを安定した状態として管理し、機能ごとに作業ブランチを作成します。

```text
main
 ├─ feature/player
 ├─ feature/enemy
 ├─ feature/boss
 ├─ feature/ui
 └─ feature/system
```

### main

完成した機能を統合するためのメインブランチです。

### featureブランチ

各機能の開発に使用します。

例：

```text
feature/player
feature/enemy
feature/boss
feature/ui
feature/animation
```

---

## 開発メンバー

| 担当         | 内容                    |
| ---------- | --------------------- |
| Programmer | C++・Blueprint・ゲームシステム |
| Planner    | ゲーム企画・仕様              |
| Motion     | キャラクターアニメーション         |
| Modeler    | 3Dモデル・アセット            |

---

## 制作記録

授業ごとの制作内容を記録します。

| 日付         | 制作内容               |
| ---------- | ------------------ |
| 2026/09/01 | プロジェクト・GitHub環境の構築 |

##

---

## 使用ツール

* Unreal Engine 5
* Visual Studio
* Git
* GitHub
* SourceTree
* Git LFS

---

## License

本プロジェクトは授業内で制作している作品です。

無断での利用・転載・再配布を禁止します。
