# Web Create Skills for Antigravity

Antigravity（Google DeepMind Agentic IDE）向けのフルスタックWebアプリケーション開発支援スキル群です。

## 含まれるスキル

| スキル名 | 説明 | 配置パス |
| :--- | :--- | :--- |
| **`web-create`** | フルスタックWebアプリ開発の全体工程（ヒアリング・アーキテクチャ設計・サブエージェント統括・QA自動デバッグ・ドキュメント作成）を一貫してオーケストレーションする中核スキル。 | `skills/web-create/` |
| **`design-master`** | 参考WebサイトのURLや画像・コンセプトを解析し、「脱AI感」のプロフェッショナルなデザイン定義書（`docs/design-spec.md`）とデザイントークン（Tailwind/CSS変数）を作成するデザイン特化スキル。 | `skills/design-master/` |

---

## ディレクトリ構成

```text
.
├── README.md
└── skills/
    ├── web-create/
    │   └── SKILL.md
    └── design-master/
        └── SKILL.md
```

---

## インストール・導入方法

### 1. グローバルスキルとして利用する場合
PC全体のAntigravity環境で常時利用可能にするには、以下のディレクトリに配置してください。

- **Windows**: `C:\Users\<UserName>\.gemini\config\skills\`
- **macOS / Linux**: `~/.gemini/config/skills/`

```bash
# 例: skills ディレクトリの内容をグローバル設定にコピー
cp -r skills/* ~/.gemini/config/skills/
```

### 2. 特定プロジェクト（ワークスペース）限定で利用する場合
プロジェクトのルート直下の `.agents/skills/` に配置してください。

```text
your-project/
└── .agents/
    └── skills/
        ├── web-create/
        │   └── SKILL.md
        └── design-master/
            └── SKILL.md
```

---

## 使い方

Antigravity IDEのチャットで以下のように指示します：

```text
/web-create
モダンなカフェのオンライン予約・テイクアウト注文ができるWebアプリを作りたいです。
```

詳細は各スキルの `SKILL.md` をご参照ください。
