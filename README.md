# Hi, I'm SEKO 👋

北海道出身、東京在住の Web Developer です。（CAL-tokyo 所属）

---

## 🏆 実績：Welp プロジェクト（CAL-welp Organization）

スキマバイト／人材マッチングサービス **Welp** の開発に、2025年4月から継続して参画しています。
スタッフ（ワーカー）向けアプリ・顧客（企業）向け Web・社内管理画面（WELMS）・バッチ・DB・インフラまで、サービス全体を横断して開発しています。

### 📊 数字で見る実績（2026年9月時点）

| 指標 | 値 |
| --- | --- |
| 作成した Pull Request | **199 件**（うちマージ **196 件**） |
| コントリビュートしたリポジトリ | **12 リポジトリ** |
| 参画期間 | 2025年4月 〜 現在 |

| リポジトリ | 領域 | PR 数 | 期間 |
| --- | --- | ---: | --- |
| Welp-cs-welms-Web | 社内管理画面（Laravel） | 55 | 2026/01 〜 |
| Welp-client-Web-Laravel | 顧客向け Web（Laravel 刷新版） | 37 | 2026/05 〜 |
| Welp-staff-Web-Laravel | スタッフ向け API / Web（Laravel 刷新版） | 37 | 2026/05 〜 |
| Welp-client-Web | 顧客向け Web（旧版） | 21 | 2026/01 〜 2026/03 |
| Welp-staff-Android-kotlin | スタッフ向け Android アプリ | 17 | 2025/04 〜 |
| Welp-staff-Web | スタッフ向け API（旧版） | 12 | 2026/02 〜 |
| Welp-staff-Flutter-Protype | スタッフ向けアプリ（Flutter 刷新版） | 6 | 2026/03 〜 |
| Welp-client-Android | 顧客向け Android アプリ | 5 | 2025/04 〜 |
| Welp-DB | データベース | 4 | 2026/05 〜 |
| Welp-client-iOS | 顧客向け iOS アプリ | 3 | 2025/04 |
| Welp-staff-iOS | スタッフ向け iOS アプリ | 1 | 2026/01 |
| Welp-Infra | インフラ（スケジュールトリガー等） | 1 | 2026/08 |

### 🛠 主な取り組み

#### 1. システム刷新（リプレイス）の推進
- 旧システムから **Laravel ベースの新アーキテクチャ** への刷新を、顧客 Web・スタッフ API・管理画面の 3 系統で推進
- **SQL Server のストアドプロシージャを Laravel Eloquent モデルへ移植**し、ビジネスロジックをアプリケーション層へ集約
- Laravel 13 / MySQL 移行を見据えた Eloquent モデル定義の整備、PHP 8.5 対応
- 刷新アプリと旧アプリの併存期間に向けた、リニューアル告知 WebView・複数パッケージ対応の KPI 集計などの移行支援

#### 2. 業務機能の開発
- **求人**：求人作成・編集、求人テンプレート、URL 限定公開／バッジ限定求人、自動公開、資格・待遇による絞り込み、地図表示
- **就業・勤怠**：QR 打刻（求人単位）、就業確定・勤怠承認、勤務評価、契約解除、無断欠勤・遅刻ペナルティ
- **請求・支払**：請求書ワーク・請求 No 採番、入金登録、締め猶予判定、源泉・給与計算、立替金計上、振込処理とエラー時ロールバック
- **コミュニケーション**：就業チャット、スカウト、プッシュ通知（リマインド・受信設定）、NG ワード検閲
- **会員登録・認証**：SMS／メール OTP 認証、eKYC、電話番号＋生年月日ログイン、得意先アカウントのロール・権限、代理ログイン
- **提携学校（専門学校）**：学生向け登録フォーム、学校別のアプリ DL 計測・動的 QR
- **KPI・分析**：ストアデータ取込、日次／月次集計、顧客別集計、バッジ指標の分布・閾値シミュレータ
- **操作履歴**：顧客・スタッフ・管理者の操作履歴記録と閲覧画面

#### 3. バッチ・自動化
- 確定処理の自動化バッチ（営業日判定対応）、就業確定リマインド、未読チャット通知などの定期バッチを実装
- 月次確定処理の原子化、部分成功時の結果表示、バッチの JWT 認証

#### 4. 品質・保守性の向上
- **Pest** による Unit / Feature テスト、**Pest 4 ブラウザテスト（E2E）** の導入と継続的な拡充
- **Larastan（静的解析）Level 6** 対応を中心とした広範囲リファクタリング、JavaScript 全般のリファクタリング
- SQL クエリの実行性能改善、コントローラーの責務分離、PHPDoc の全面刷新
- Laravel Boost / AI エージェント向けスキルの整備による開発生産性の向上

#### 5. セキュリティ・運用基盤
- 脆弱性診断の指摘事項に対する是正対応、セキュリティチェック対応
- ログのトレーサビリティ強化（機微情報マスク付きコンテキスト、CloudWatch での調査性向上）
- AWS（S3 / CloudFront による画像配信、WAF 誤検知対策）、Docker / Laravel Octane 環境の整備
- コンテナビルド時の脆弱性スキャン対策、環境ごとの設定切り替え

#### 6. モバイルアプリ
- Android（Kotlin）：SMS 本人認証、全国解放対応、在留資格者向け対応、Google Play 審査対応（ストレージ権限削除）、targetSdk 更新
- Flutter：マップ検索、就業レビュー画面、しごと予定チャット、経路表示
- iOS：表示修正・キャンセル対応

### 💻 技術スタック

| 分類 | 技術 |
| --- | --- |
| Backend | PHP 8.x, Laravel, Laravel Octane, Eloquent |
| Frontend | Blade, JavaScript, Tabler |
| Mobile | Kotlin (Android), Flutter, Swift (iOS) |
| Database | MySQL, Microsoft SQL Server |
| Testing / Quality | Pest（Browser Testing 含む）, Larastan |
| Infra | AWS (S3, CloudFront, CloudWatch, WAF), Docker |
| Tools | GitHub, Laravel Boost, Claude Code |
