### 2024/12/26 AWSサービスの写経
* AWS CAFおよび機械学習関連のサービスをノートに写経  
  手書きと音読でより覚えられるのでは。
#### 次の予定
* SAA対策動画の視聴  

### 2024/12/24 AWSサービスの勉強
* AWS ECS  
  * フルマネージドサービス
  * アプリケーションのデプロイ、スケーリング、管理を効率化
  * Amazon ECSの実行環境 → Amazon EC2 or AWS Fargateで実行
    サーバレスかそうでないか。
  * 構成要素
    * クラスタ  
    コンテナを実行するコンピューティングリソースの集まり。EC2インスタンスやFargateで構成可能。
    *  タスク定義  
    コンテナの設定を定義したJSONファイル。使用するイメージ、リソース、環境変数などを指定。
    * タスク  
    タスク定義に基づいて実行されるコンテナインスタンス。単一または複数のコンテナを含む。
    * サービス  
    タスクを指定数常に実行することを保証。負荷分散や高可用性を実現。
  * 定義はAWS Secrets Manager, AWS Systems Manager パラメータストアやIAMアクセス許可設定を適切に使い、機密情報は守る

### 2024/12/22 CLF対策
* 問題集回答 161-170  
  examtopicsの無料分終了。
#### 次の予定
* udemyか、参考書を探す

### 2024/12/21 CLF対策
* 問題集回答 131-160
#### 次の予定
* 問題集回答
  
### 2024/12/19 CLF対策
* 問題集回答 81-130
#### 次の予定
* 問題集回答　1月までは続ける予定。場合によっては、SAA

### 2024/12/17 CLF対策
* 問題集回答 1-80
* AWS CAFの確認
#### 次の予定
* 問題集回答 719問あり。中々やりごたえある

### 2024/12/16 CLF対策
* 問題集回答 
  No.51-100

* 気づき
  * AWS Trusted Advisorはもう一度確認
  * 正答率90%超えではあるがケアレスミスが1問あり。
  
* No.68 AWSイベントが会社のAWSリソースに影響を与える可能性がある場合、アラートを提供するAWSサービスは次のうちどれですか？
  AWS Personal Health Dashboard
  AWS service health Dashboard  
  AWS Trusted Advisor  
  AWS Infrastructure Event Management  
* No.78 オンプレミスサーバーにアプリケーションをデプロイすることができるサービスは次のうちどれですか。（2つ選択してください）  
  AWS Elastic Beanstalk
  AWS OpsWorks
  AWS CodeDeploy
  AWS Batch
  AWS X-Ray
* No.88 コンプライアンスレポートと証明書を取得するためには、どのAWSサービスを使用すればよいですか？  
  AWS Artifact
  AWS Lambda
  Amazon Inspector
  AWS Certificate Manager
* No.92 AWSのお客様が新しいAmazon RDSクラスターを起動するために使用できるのは次のうちどれですか？正しい組み合わせを選択してください。  
  AWS コンシェルジュ
  AWS CloudFormation
  Amazon S3
  Amazon EC2 Auto Scaling
  AWS Management Console
* No.96 AWSリソースの運用上の洞察を得て、それらのリソースを使用するアプリケーションに影響を与える可能性のある問題を迅速に特定するのに役立つAWSサービスはどれですか？  
  Amazon Inspector
  AWS Systems Manager
  AWS Trusted Advisor
  AWS Health Dashboard

#### 次の予定
* 問題集を解く
* 不得意なサービスの再確認

### 2024/12/15 CLF対策
#### AWS認定クラウドプラクティショナー（CLF-C01）対策トレーニング Cloud Practitioner(https://www.youtube.com/watch?v=ELVAXUVFZaM&ab_channel=Maruchintechch)
  * Networking & Content Delivery  
    * Amazon Route53  
      DNSサービス, ELBを使わずLBっぽい動きが出来る
    * Elastic Load Balancing  
      負荷分散, DNS切り替えなくEC2インスタンス切り替え可能, ALB, NLB, GLBが存在
  * Database
    RDB, NoSQL(Key-Value, 列指向, ドキュメント指向, グラフ指向)
    * Amazon RDS  
      リレーショナル型データベース
    * Amazon Aurora  
      MySQL, PosgreSQLとの互換かつ高性能
    * Amazon Redshift  
      データシェアハウス向け
    * Amazon DynamoDB  
      Key-Value型
    * Amazon ElasticCache  
      インメモリ型DB, RDBとApp間にキャッシュとして配置するなど
  * Application Integration  
      モノリシック, マイクロサービス
    * Amazon Simple Queue Service(SQS)  
      フルマネージドなメッセージキューサービス
    * Amazon Simple Notification Service(SNS)  
      メッセージ通知サービス,EmailやSMSなど
    * Amazon EventBridge  
      イベントデータを他クラウドやアプリケーションと連携
    * AWS Step Functions  
      ワークフローを構成し実行プロセスを構築管理自動化
  * Analytics
    * Amazon Kinesis Data Streams, Data Firehose, Data Analytics, Video Streams  
      ストリーミングデータを扱う,
    * Amazon Athena  
      標準SQLによりS3内のデータを分析
    * Amazon QuickSight  
      BIツール, AWSだけでなく3rd Partyツールのデータソースもサポート
  * Developer Tools
    * AWS CodeCommit  
      Gitのレポジトリと連携, 通知やDiffも可能
    * AWS CodeBuild  
      ビルド,テスト環境をフルマネージドで提供
    * AWS CodeDeploy
      本番環境へデプロイするサービス, デプロイするアプリはS3やGithubを指定

  * Pricing Calculator  
    見積もりツール
  * AWS Trusted Advisor  
    AWSアーキテクチャを分析し、ベストプラクティスの推奨事項を提供
  * AWS Partner Network
    コンサルトとテクノロジー
  * AWS Marketplace
    3rd partyのSWやServiceを検索, 比較, 購入
    
  * 学習リソース AWS公式
    * AWS Well-Architected(https://aws.amazon.com/jp/architecture/well-architected/)
    * Amazon WerServieブログ(https://aws.amazon.com/jp/blogs/news/)
    * AWS ホワイトペーパー(https://aws.amazon.com/jp/whitepapers/)
    * ナレッジセンター(https://repost.aws/ja/knowledge-center)
    * AWS Skill Builder(https://aws.amazon.com/jp/training/digital/)
    * コミニケション・イベント(https://aws.amazon.com/jp/events/aws-event-resource/)  
      * AWS JAWS-UG
      * AWS Summit
      * AWS re:Invent
      * AWS Black Belt Online Seminar
       
  * 学習リソース 非公式<sub>英語圏が圧倒的に情報が多い</sub>
    * Stephane Maarek | AWS Certified Cloud Practitioner,Solutions Architect,Developer(https://www.udemy.com/user/stephane-maarek/)
    * Jon Bonso AWS Certified Cloud Practitioner, Developer, Solutions Architect(https://www.udemy.com/user/jonjonbonso/)
      
    * A Cloud Guru(https://www.pluralsight.com/cloud-guru)
    * Digital Cloud Traing(https://digitalcloud.training/)
      
    * Stack Overflow(https://stackoverflow.com/collectives/aws)
    * Breifmenow(http://www.briefmenow.org/amazon/)
    * Exam Topics(https://www.examtopics.com/exams/amazon/)
  
* 問題集回答  
  No.1-50

#### 次の予定
* 問題集を解く

### 2024/12/14 CLF対策
#### AWS認定クラウドプラクティショナー（CLF-C01）対策トレーニング Cloud Practitioner(https://www.youtube.com/watch?v=ELVAXUVFZaM&ab_channel=Maruchintechch)
* クラウドの特徴
  * 可用性, スケーラビリティ, コスト最適化, 
  * AWSはデファクトスタンダードになってる
  * クラウドの分類(IaaS, PaaS, SaaS,)
  * 責任共有モデル  
    セキュリティの責任範囲, クラウド側はあくまで土台まで, 土台の上で構築するアプリやらシステムやらはユーザ側が作った部分
  * クラウドは3種類, パブリッククラウド, ハイブリッドクラウド, プライベートクラウド
  * AWS 構築ツール  
    コンソール, CLI, SDK
* 各サービスの説明
  * Management, Monitoring& Governance
    * AWS Organizations  
      複数のアカウントを階層構造で管理, SCPの一括管理, 請求の一括管理, 他サービスとの連携
    * Amazon CloudWatch (logs, Events, Alarms, Logs Insights, Dashboards)  
      統合的な運用監視サービス
    * AWS CloudTrail  
      いつ,だれ,なにをしたか記録 証跡を集める。90日までは無料保管, 長期保管はS3などのストレージサービス併用
    * AWS Config  
      AWSリソースの構成変更をログとして残す, 他Configルールを策定し、準拠されているか確認出来る
    * AWS License Manager  
      MS,SAP,Oracle,IBMなどのソフトウェアライセンスを一元管理
    * AWS Systems Manager  
      ハイブリッド環境向けの管理, オンプレとクラウドを一元管理
    * AWS Health  
      パフォーマンスの変更や障害などの情報をタイムリーに提供
    * AWS CloudFormation  
      IaC, AWSのリソースをJOSNやYAMLで記述して、テンプレート化して実行
    * AWS Budgets  
      予算のしきい値を超える, 超えそうな時アラートを発報
    * AWS Cost Explorer  
      各リソースのコストや使用状況を確認
    * タグ付け  
      リソースを識別するためのメタデータ, 部署名とか色々
  * Security, Identity&Compliance
    * AWS IAM  
      ユーザやグループに対し,サービスやリソースへの認証と認可を管理する
    * AWS STS(Security Token Service)  
      AWSのリソースのアクセスをコントロール, 一時的なセキュリティ認証情報として使用する
    * AWS KMS(Key Management Service)  
      暗号化キーの作成と制御を行うマネジメントサービス
    * AWS Certificate Manager  
      証明書の発行およびキーの作成保存更新を行う サイトシールは別途必要
    * Amazon Cognito  
      Webアプリケーションのサインアップ, サインアップ機能のアクセスを制御
    * AWS Secrets Manager  
      シークレット情報のライフサイクルを一元管理, DB認証情報やパスワードなど
    * Amazon Macie  
      S3に保存されたデータから機密データを検出, KMSによって暗号化
    * Amazon GuardDuty  
      ストレージやログサービスを分析し脅威となるデータを抽出, ランサムや悪意のあるアクセスなど
    * Amazon Detective  
      各種サービスのログデータを自動的に収集, 機械学習統計的分析を用いて詳細な調査を行う
    * AWS WAF  
      WebApplicationFirewall, CloudFrontやApplicationLoadBalancerなどのリクエストに対応
    * AWS Network Firewall  
      VPC向けのステートフルなファイアウォール
    * AWS Shield  
      DDoS攻撃からAWSリソースを保護するサービス
    * AWS Firewall Manager  
      複数アカウントでAWS WAF,AWS Shield Advanced, VPCセキュリティグループ, AWS Network Firewall, Amazon Route53 DNS Firewall, 3rd Party製Firewallの一元管理
  * Storage  
    オブジェクトストレージ, ブロックストレージ, ファイルストレージの3種
    * S3  
      最も汎用的なオブジェクトストレージサービス, データの性質によりストレージのクラスを選択可能(耐久性,可用性)
    * S3 Glacier  
      アクセス頻度の低いデータ保存用, 保存は安いが取り出しは高い
    * AWS Storage Gateway  
      AWS上のストレージをオンプレ環境に対してシームレスに接続するサービス
    * Amazon EFS  
      複数のインスタンスにマウント可能, 
    * Amazon EBS  
      ブロックストレージでクラスを選択可能, 単一のインスタンスにマウント
    * Amazon FSx 
      フルマネージドなファイルストレージサービス
    * AWS Backup  
      バックアップの一元化, 自動化
    * AWS Snow Family  
      物理ストレージを使い大きなデータを転送, 1週間~10日間程度かかる
  * Compute
    * Amazon EC2  
      仮想サーバ
    * Amazon EC2 Auto Scaling  
      必要に応じインスタンスを増やして,負荷分散を行う ロードバランサーを通す
    * AWS Auto Scaling
      複数のサービスにまたがる複数のリソースをスケーリング, DynamoDBやAuroraなど
    * Amazon ECS    
      Dockerを利用
    * Amazon EKS  
      Kubernetesを利用
    * AWS Lambda  
      サーバレスでコードを実行できるフルマネージドサービス
    * AWS Batch  
      数十万規模のバッチ処理を実行するためのサービス
    * Amazon Lightsail  
      EC2より低価格で規格化された仮想サーバ, 月額固定
    * Amazon Elastic Beanstalk  
      インフラやスケーリングを自動で構築するサービス, configファイルでカスタマイズ
    * Amazon WorkSpaces  
      VDI(仮想デスクトップサービス)
    * AWS Compute Optimizer  
      EC2,EBS,Lambdaの使用状況を分析し、リソースサイズが適切かどうか確認をする
  * Networking & Content Delivery  
    * AWS VPC  
      AWS上の仮想アドレス空間, Subnetの中に実際のAWSリソースを配置
    * VPC Flow Logs  
      ENIのIPトラフィック情報をキャプチャ
    * VPC Peering  
      VPC間をプライベートで接続
    * Gateway
      * Internet Gateway  
        VPCとインターネットとの通信を可能にするVPCコンポーネント, VPC1つに1つのみ
      * NAT Gateway  
        プライベートIPをグローバルIPに変換
      * VGW(Virtual Gateway)  
        VPCとVPNやDirectConnectを接続, AWSとオンプレを接続する際に使用
      * Customer Gateway  
        オンプレミス側のVPNエンドポイント
    * Virtual Private Network  
      AWS Client VPNを使用して、AWSリソースに安全にアクセス
    * AWS Direct Connect  
      専用線サービス, 単一アカウントの専用線接続かホスト接続
    * Amazon CloudFront  
      クライアントとコンテンツの間に設置, キャッシュを用い低レイテンシでコンテンツを配信
    * AWS Global Accelerator  
      クライアントとコンテツの間に設置, キャッシュはない, エッジロケーションを使用することでパフォーマンスを向上
    * Amazon Route53
    * Elastic Load Balancing

#### 次の予定
* Database, Application Integration, Analytics, Developer Tools   1時間位？
* 出来れば問題集

### 2024/12/13 AWS Well-Architected Frameworkとは
#### AWS Well-Architected Framework ホワイトペーパー(https://docs.aws.amazon.com/ja_jp/wellarchitected/latest/framework/welcome.html)
* オペレーショナル・エクセレンス
 * ベストプラクティス
    * 4つのベストプラクティス領域  
      * 組織
         * 優先順位の設定  
           ビジネス全体で共有される目標を定義し、優先順位を設定
         * 顧客ニーズの評価  
           社内外の顧客ニーズを評価し、重要な領域を決定
         * リスク評価  
           ビジネスに対する脅威を評価し、リスク管理を行う
         * 継続的な改善  
           優先順位を定期的に見直し、ニーズの変化に応じて更新
      * 準備
      	* ワークロードの理解
       * 観測性の確立  
         ワークロードの内部状態（メトリクス, ログ, イベント, トレースなど）を情報を取得出来る設定
       * キーパフォーマンスインジケータの特定  
         監視活動とビジネス目標の整合性を確保
       * 頻繁で小規模かつ可逆的な変更
       * 運用手順の頻繁な改善  
         ワークロードの変更に伴い、運用手順も進化させ、定期的なレビューと改善
       * 失敗の予測
         
      * 運用
      * 進化

#### 次の予定


### 2024/12/12 AWS Well-Architected Frameworkとは  
#### AWS Well-Architected Framework tool
* Self-check用のツール。  
  AWSアカウント必須のため、後回し  
  aws free tierの時間が勿体ないのでまだしない

#### 【AWS Black Belt Online Seminar】AWS Well-Architected Framework(動画)

* レビューは初期に  
  初期であれば取り返しがつくし、より良い方法が見つかるかもしれない。  
  進んでからレビューすると手戻りが発生する可能性も考慮しなければならなくなる    
* 定期的なレビューとKAIZEN  
  頻度は年一の棚卸しとかがやりやすいと思う  
  AWSで新しいサービスが出来てよりベストプラクティスが進んでいたり、情勢が変化してセキュリティのやり方が変わっている可能性もある。  
  セキュリティや問題点の顕在化と把握が重要。把握した上でやらない理由があるならよい。  
  ワールドワイドでKAIZENとよぶらしい。。。2018年頃のはなし？  
* レビューの進め方
  レビュー参加者の最初の認識合わせ  
 *監査ではなく、話し合いの場である*  
  誰も責めない  
 *関係者が対話に集まる*  
  実装しているチームが、実は全体は理解していなかったとかあり得る  
  担当箇所以外は見え難い...  
 *継続的なレビュー*  
  常に世の中変化しているので、継続的に行うのがベスト  
  AWSの新サービスの追加、マネージド型が出てきたり  
  コストの最適化、割と新しいインスタンスタイプは性能上がって安価になる場合もある
 

#### AWS Well-Architected Framework ホワイトペーパー  
* 一般的な設計の原則
  * 容量ニーズの推測不要
  * 本稼働スケールでシステムをテストする
  * アーキテクチャの実験を念頭に置いた自動化
  * 発展するアーキテクチャを検討
  * ゲームデーを利用して改善
* オペレーショナル・エクセレンス  
  企業が業務を効率的かつ効果的に運営し、競争優位性を確立するための取り組み  
  * 設計原則
    * ビジネスの成果に基づいたチームを編成。ビジネス目標を達成するために、効率化をする
    * 可観測性の実装。
    * 安全な自動化
    * 頻繁で小規模かつ可逆的な変更
    * 運用手順の頻繁な改善
    * 失敗を予測する
  * ベストプラクティス

#### 次の予定
* AWS Well-Architected Frameworkホワイトペーパーを満足するところまで確認

### 2024/12/11 クラウドの初歩の初歩から
#### はじめてのアマゾン ウェブ サービス（動画）

-AWSの歴史から  
-クラウドのいいところ  
--迅速な調達、柔軟な変更、最適化されたコスト  
-セキュリティ優先。けれど、責任共有モデルはよく理解しましょう。

#### AWS ご利用開始時に最低限おさえておきたい10のこと（動画&PDF）
 
-ベストプラクティス(AWS Well-Architected Framework(W-A)の理解。  
過去実績から出したチェックリストと理解
あくまで指針なので、従わないこともある。リスクの把握と顕在化が大事

#### AWS 設計のベストプラクティスで最低限知っておくべき 10 のこと（動画&PDF）
 
-基本的な考え方はオンプレと重複する部分もあるが、自由  
--動的なリソースの変更,使い捨ての環境,サーバレスの活用,潤沢な冗長性確保の手段,全レイヤでのセキュリティ確保と考慮すべきポイントは多い

#### 次の予定
 
-AWS Well-Architected Framework toolとは  
