# 02_AIとは

## 序章

AIとはArtificial Intelligence / 人工知能。
AI利用の幹となるのがLLM。
LLMとは大規模言語モデル。これがAIの脳・エンジンとなる。

---

## 第1章：LLM（基盤モデル）

世の中のLLM種類（2026/10/05時点想定、リンクは現在の公式URL）

| No | 国 | 作成会社 | モデル形態 | LLMシリーズ | 代表的なモデル名 | 公式リンク・情報元 | リンク・内容の妥当性評価 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | USA | OpenAI | クローズド | GPT | GPT-5 / GPT-4o / o1 | [OpenAI API](https://openai.com/api/) | 【妥当】公式のAPI・モデル一覧ページ。モデルの系譜と一致。 |
| 2 | USA | Anthropic | クローズド | Claude | Claude 3.5 Sonnet 等 | [Anthropic Claude](https://www.anthropic.com/claude) | 【妥当】Claude製品ページ。現行の主力モデル情報と一致。 |
| 3 | USA | Google | クローズド | Gemini | Gemini 1.5 Pro 等 | [Google DeepMind Gemini](https://deepmind.google/technologies/gemini/) | 【妥当】DeepMind社の公式ページ。移行事実と合致。 |
| 4 | USA | Meta | オープン | Llama | Llama 3.1 / 3.2 等 | [Meta Llama](https://llama.meta.com/) | 【妥当】Meta公式。オープンソースLLMの覇権としての実態と合致。 |
| 5 | USA | Microsoft | オープン | Phi | Phi-3 / 3.5 等 | [Microsoft Phi-3](https://azure.microsoft.com/ja-jp/blog/introducing-phi-3-redefining-whats-possible-with-slms/) | 【妥当】Microsoft公式。SLM（小規模言語モデル）の定義と一致。 |
| 6 | USA | xAI | オープン/API | Grok | Grok-2 / Grok-2 mini | [xAI](https://x.ai/) | 【妥当】イーロン・マスク氏設立。Xデータ活用モデルとして一致。 |
| 7 | USA | IBM | オープン | Granite | Granite 3.0 | [IBM Granite](https://www.ibm.com/granite) | 【妥当】IBM公式。企業向け透明性の高いオープンモデルと一致。 |
| 8 | USA | Amazon | クローズド | Titan | Amazon Titan | [Amazon Bedrock](https://aws.amazon.com/jp/bedrock/titan/) | 【妥当】AWS公式。Bedrock上で提供される自社開発モデルと一致。 |
| 9 | France | Mistral AI | オープン/API | Mistral | Mistral Large / Mixtral | [Mistral AI](https://mistral.ai/) | 【妥当】欧州発の公式。オープン/商用APIのハイブリッド実態と一致。 |
| 10 | Canada | Cohere | クローズド | Command | Command R+ | [Cohere](https://cohere.com/) | 【妥当】Cohere公式。B2B向け・RAG特化モデルとして一致。 |
| 11 | Israel | AI21 Labs | オープン/API | Jamba | Jamba 1.5 | [AI21 Labs](https://www.ai21.com/) | 【妥当】ハイブリッドアーキテクチャモデルとして世界的注目。妥当。 |
| 12 | China | Moonshot AI | クローズド | Kimi | Kimi (Moonshot) | [Moonshot AI](https://www.moonshot.cn/) | 【妥当】中国の有力AI企業。超長文処理に強い事実と一致。 |
| 13 | China | Alibaba | オープン | Qwen | Qwen 2.5 等 | [Qwen (GitHub)](https://github.com/QwenLM/Qwen) | 【妥当】アリババ開発。世界最高峰のオープンモデルとして事実と合致。 |
| 14 | China | DeepSeek | オープン | DeepSeek | DeepSeek-V2 / Coder | [DeepSeek](https://www.deepseek.com/) | 【妥当】中国の有力OSS。GPT-4級の評価を得ている事実と合致。 |
| 15 | China | Baidu | クローズド | ERNIE | ERNIE 4.0 (文心一言) | [Baidu ERNIE](https://yiyan.baidu.com/) | 【妥当】百度の主力モデル。中国国内エンタープライズ市場を牽引。 |
| 16 | China | Zhipu AI | オープン/API | GLM | GLM-4 | [Zhipu AI](https://www.zhipuai.cn/) | 【妥当】清華大学発。中国トップクラスの汎用モデルと一致。 |
| 17 | China | 01.AI | オープン | Yi | Yi-Large | [01.AI](https://01.ai/) | 【妥当】李開復氏設立。グローバルで高性能なオープンモデル。 |
| 18 | Japan | NTT | 一部オープン | tsuzumi | tsuzumi | [NTT tsuzumi](https://www.rd.ntt/research/LLM_tsuzumi.html) | 【妥当】NTT公式。軽量・日本語特化のコンセプトと一致。 |
| 19 | Japan | NEC | クローズド | cotomi | cotomi | [NEC cotomi](https://jpn.nec.com/cotomi/) | 【妥当】NEC公式。業種特化型としての実態と一致。 |
| 20 | Japan | Sakana AI | オープン | EvoLLM | EvoLLM / EvoVLM 等 | [Sakana AI](https://sakana.ai/) | 【妥当】日本発。進化的モデルマージという独自手法の開発実態と一致。 |
| 21 | Japan | SoftBank | オープン | Sarashina | Sarashina | [SoftBank](https://www.softbank.jp/corp/news/press/sbkk/2023/20231031_01/) | 【妥当】国内最大規模の計算基盤を用いた開発事実と一致。 |
| 22 | Japan | PFN | オープン | PLaMo | PLaMo-13B 等 | [Preferred Networks](https://www.preferred.jp/ja/news/pr20230928/) | 【妥当】日本のAIユニコーンPFNが独自開発するモデルと一致。 |

---

## 第2章：AIエージェント・アプリケーション

LLMを利用してエージェント（タスク実行できる機構＝手足・ハーネス）を作る。

### 1. 汎用チャット・対話型AI

（ユーザーが直接プロンプトを入力し、汎用的な回答や推論を得るチャットUI/ボット）

| No | 国 | 提供会社 | エージェント(UI)名 | バックエンドLLM | メリット・特徴 | 公式リンク | リンク・内容の妥当性評価 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | USA | OpenAI | ChatGPT | GPT系 | 世界標準のAIチャット。Web検索、画像生成、データ分析を統合。 | [ChatGPT](https://chatgpt.com/) | 【妥当】生成AIブームの火付け役。事実と完全一致。 |
| 2 | USA | Anthropic | Claude (Web UI) | Claude系 | 非常に自然な文章生成と、Artifacts（コードや図のプレビュー機能）が強力。 | [Claude](https://claude.ai/) | 【妥当】公式チャットUI。Artifacts機能の事実と合致。 |
| 3 | USA | Google | Gemini (Web UI) | Gemini系 | Google Workspace連携が強力で、リアルタイムな情報検索に優れる。 | [Gemini](https://gemini.google.com/) | 【妥当】旧Bard。Googleの公式チャットAIとして事実と一致。 |
| 4 | USA | Microsoft | Microsoft Copilot | GPT系 | 無料でGPT-4クラスが利用でき、Web検索(Bing)と強く統合されている。 | [Copilot](https://copilot.microsoft.com/) | 【妥当】旧Bing Chat。Web検索連動チャットとして事実と一致。 |
| 5 | France | Mistral AI | Le Chat | Mistral系 | 欧州発のチャットUI。プライバシーに配慮しつつ高速なレスポンス。 | [Le Chat](https://chat.mistral.ai/) | 【妥当】Mistralの公式チャットサービスとしての実態と一致。 |
| 6 | China | Moonshot AI | Kimi Chat | Kimi | 200万文字以上の超長文コンテキストを処理でき、中国国内で爆発的普及。 | [Kimi](https://kimi.moonshot.cn/) | 【妥当】長文特化のチャットAIアプリとして中国シェア上位の事実と合致。 |
| 7 | Japan | Sakana AI | Fugu | Sakana AI製モデル | 浮世絵テイストの和風UI。Sakana AIの画像言語モデル等の性能を試せるデモUI。 | [Sakana Fugu](https://fugu.sakana.ai/) | 【妥当】Sakana AIが公開している公式デモチャットUIの事実と一致。 |
| 8 | USA | Hugging Face | HuggingChat | 複数のOSSモデル | LlamaやQwenなど、最新のオープンソースモデルを無料で切り替えて試せる。 | [HuggingChat](https://huggingface.co/chat/) | 【妥当】OSSコミュニティ最大のチャットポータルとして事実と一致。 |

### 2. 資料作成・ナレッジ・検索エージェント

（特定データの要約、スライド生成、情報検索に特化したエージェント）

| No | 国 | 提供会社 | エージェント名 | 利用LLM | メリット・特徴 | 公式リンク | リンク・内容の妥当性評価 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | USA | Google | NotebookLM | Gemini | 大量のPDF等から高精度な要約や音声(Podcast風)生成が可能。 | [NotebookLM](https://notebooklm.google/) | 【妥当】Google公式ツール。RAGを活用したAIとして一致。 |
| 2 | USA | Microsoft | Copilot for M365 | GPT-4系 | Office製品(Word, Excel, PPT)とシームレスに連携。 | [Microsoft Copilot](https://www.microsoft.com/ja-jp/microsoft-365/enterprise/copilot-for-microsoft-365) | 【妥当】公式製品ページ。Office統合の実態と一致。 |
| 3 | USA | Notion Labs | Notion AI | Claude/GPT等 | ドキュメント管理ツール内で直接文章の推敲や生成が完結する。 | [Notion AI](https://www.notion.so/ja-jp/product/ai) | 【妥当】Notion公式。ワークスペース統合型AIとしての機能と一致。 |
| 4 | USA | Perplexity | Perplexity AI | 複数モデル | 「AI検索エンジン」の覇権。Web上の最新情報を検索・統合して回答。 | [Perplexity](https://www.perplexity.ai/) | 【妥当】情報収集エージェントとして世界トップシェア。事実と一致。 |
| 5 | USA | Gamma | Gamma | 独自/複数 | テキストを入力するだけでプレゼンスライドを数秒で自動生成・デザイン。 | [Gamma](https://gamma.app/) | 【妥当】資料作成特化のAIエージェントとして急速に普及。事実と一致。 |

### 3. コーディング・開発支援エージェント

（コードの自動生成、デバッグ、環境構築を自律的・半自律的に行うエージェント）

| No | 国 | 提供会社 | エージェント名 | 利用LLM | メリット・特徴 | 公式リンク | リンク・内容の妥当性評価 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | USA | Anysphere | Cursor | Claude, GPT等 | プロジェクト全体のコード文脈を自動把握。自律的修正(Composer)に強い。 | [Cursor](https://www.cursor.com/) | 【妥当】公式サイト。AIファーストエディタとしての機能と一致。 |
| 2 | USA | GitHub | GitHub Copilot | GPT系 | 各種エディタの拡張機能として動作し、普及率が世界一。 | [GitHub Copilot](https://github.com/features/copilot) | 【妥当】業界標準のコーディング支援ツールとしての実態と一致。 |
| 3 | USA | Cognition | Devin | 独自(非公開) | 「世界初のAIソフトウェアエンジニア」。要件から自律的にコーディング・テストを実行。 | [Cognition Devin](https://www.cognition.ai/blog/introducing-devin) | 【妥当】自律型AIエージェントの代表格。技術トレンドと完全に一致。 |
| 4 | USA | Amazon | Q Developer | 独自モデル | AWS環境の構築やコード生成に特化。(旧CodeWhisperer) | [Amazon Q](https://aws.amazon.com/jp/q/developer/) | 【妥当】AWS公式。インフラ開発特化のエージェントとして事実と一致。 |
| 5 | USA | Zed Industries | Zed | 複数モデル | Rust製で極めて軽量・高速なエディタ。AI機能がネイティブ統合。 | [Zed](https://zed.dev/) | 【妥当】Zed公式サイト。高速性とAI機能の内包というコンセプトと一致。 |
| 6 | - | オープンソース | Cline (旧Claude Dev) | 任意のAPI | VS Code内で動き、ターミナル操作やファイル作成を自律的に行う。 | [GitHub - Cline](https://github.com/cline/cline) | 【妥当】公式リポジトリ。自律型エージェントとしての動作仕様と一致。 |
| 7 | - | オープンソース | Aider | 任意のAPI | ターミナル上で動くAIペアプログラマ。Git連携し自動でコミットを作成。 | [Aider](https://aider.chat/) | 【妥当】OSSのCUIコーディングエージェントとして事実と合致。 |
