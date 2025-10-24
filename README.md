# 【Git研修】GitHub Desktopで学ぶバージョン管理 🚀

## 目的
- チーム開発で必須のGit/GitHubの最低限の動作をマスターする（CloneからPR作成まで）
- [【🆕必須】Git＆GitHubインプット](https://www.notion.so/Git-GitHub-249a2eba3296801ea3bdc2b1677ada94?pvs=21) で学んだ内容をアウトプットする

## 準備
1. [GitHub Desktop](https://desktop.github.com/)をインストール
2. TOKIUMのGitHubアカウントでログイン

## ワーク：キャラクターのプロンプトを作成

### Step 1: リポジトリをクローン
1. GitHub Desktopを開く
2. File > Clone Repository... を選択
3. URLタブで以下を入力：
   ```
   https://github.com/TOKIUM/git-training-for-ai-agent-interns.git
   ```
4. Local Pathを選択してClone

### Step 2: ブランチ作成
1. Current Branchが`main`であることを確認
2. New Branchボタンをクリック
3. ブランチ名を入力（例：`yamada/cat-character`）
4. Create Branch

### Step 3: プロンプト編集
1. `Show in Finder`でフォルダを開く
2. `Prompt-template.txt`をエディタで開く
3. キャラクター設定を編集
4. [Gemini](https://gemini.google.com/)で「Gemを作成」
5. プロンプトを貼り付けてテスト
6. 必要に応じて修正を繰り返す

### Step 4: コミット
1. GitHub DesktopのChangesタブで変更を確認
2. Summaryに変更内容を入力（例：「猫キャラクターの口調を追加」）
3. Commit to [ブランチ名]をクリック

### Step 5: プッシュ
1. Publish branchまたはPush originボタンをクリック

### Step 6: プルリクエスト作成
1. Create Pull Requestボタンをクリック
2. ブラウザでPR作成画面が開く
3. Create Pull Requestをクリック

### Step 7: マージ
1. GitHubの「Pull requests」タブをクリック
2. 他の参加者のPRを選択
3. `Merge pull request`をクリック
4. `Confirm merge`をクリック

### Step 8: 最新変更を取り込み
1. GitHub Desktopに戻る
2. `Fetch origin`または`Pull origin`をクリック

## 重要な習慣

| 操作 | 習慣 |
|------|------|
| **作業開始時** | 必ず`main`ブランチを最新にする |
| **ブランチ作成** | `main`から新しいブランチを作成 |
| **コミット** | こまめにコミット、1つの変更に1つのコミット |
| **プッシュ** | 作業の区切りでプッシュ |
| **PR作成前** | コンフリクトがないか確認 |
| **マージ** | レビュー承認後にマージ |

## コミットメッセージの例
```
feat: 猫キャラクターの口調を追加
fix: プロンプトの誤字を修正
docs: READMEの手順を更新
```

## 用語集

| 用語 | 説明 |
|------|------|
| **クローン** | リポジトリをPCにコピー |
| **ブランチ** | 自分専用の作業スペース |
| **コミット** | 変更内容を記録 |
| **プッシュ** | 変更をGitHubに送信 |
| **プルリクエスト** | レビュー依頼 |
| **マージ** | 変更を統合 |
| **プル** | 最新変更を取得 |

## 困ったとき
- **コミット取り消し**: Historyタブでコミットを右クリック → Revert Changes in Commit
- **分からない時**: 研修担当者に相談

---

**研修担当者**: TOKIUM開発部  
**対象**: AIエージェントインターン生  
**所要時間**: 約60-90分