# 職務経歴書

## 個人データ

* 氏名: 早坂 彪流 / HAYASAKA Takeru
* ID: `takemioIO`, `takehaya`
* 社会人(フルタイム)になってからの貢献を記述しています。学生時代のインターンやコンテストなどの貢献を確認したい場合は以下のプロフィールサイトを参照してください。
  * [https://profile.takemio.net/](https://profile.takemio.net/)

## 職務要約
モバイルコアの自社開発・運用やゲーム機向け SDK 開発など、ソフトウェアからインフラまで幅広くシステム開発に従事してきました。
特に C/Go を中心とした高性能なネットワーク処理やクラウド基盤の最適化により、大幅な性能向上とコスト削減を実現し、OSS への貢献も行っています。
また、社内勉強会の主催や若手育成、外部登壇・技術ブログ執筆を通じて知見を共有し、組織とコミュニティの発展に寄与してきました。課題解決に向けた主体的な行動力と技術力を軸に、プロジェクト推進と人材育成に取り組んでいます。

## さくらインターネット株式会社 / BBSakura Networks株式会社 (2022/10〜現在)
* さくらインターネット株式会社から出向
* 契約: フルタイム
* 所属: モバイル開発チーム
* 職位: シニアソフトウェアエンジニア

### フル MVNO 事業(2022/10〜現在)
* 説明: フル MVNO 事業者として、モバイルコアをゼロから自社開発し、運用・開発を担当
* プログラミング言語: C, Go, Python, Terraform, Ansible など
* その他キーワード: Google Cloud（Cloud Run, Spanner, BigQuery, Cloud Monitoring など）, GitHub Actions, Linux, eBPF, XDP, ConnectRPC, gRPC, FRR
* 業務内容
  * モバイルコア開発
  * 他 MVNO との BGP を用いた相互接続オペレーション
  * モバイル環境の E2E 監視システム
  * SRv6 MUP の研究開発
* 実績
  * トラフィック集計機能の年間コストを通常ワークロードで約 **3万分の1** に削減（Cloud Monitoring から BigQuery への移行によるリソース最適化）
  * パケット転送機能を持つサービスで、SCTP 関連のカーネルパラメータをチューニングし、性能を **約200倍** に向上
  * パケット交換機のマルチコア化を実装し、モバイル接続の処理能力を **100 Gbps** まで拡張（従来比 **約27倍**）
    * 成果の一部を Linux カーネル／ethtool に upstream（粘り強く交渉・調整）
      * ethtool: Add GTP RSS hash options to ethtool.h
      * ice: Implement RSS settings for GTP using ethtool
        * [https://www.spinics.net/lists/netdev/msg979517.html](https://www.spinics.net/lists/netdev/msg979517.html)
  * 市販の負荷試験ツールでは **4,000〜5,000万円** のライセンス費用が見込まれるところ、自作により費用を削減し、モバイルコアで用いる NFV の性能測定を実現
    * 主体的に企画・実行（学生アルバイトの採用を含む）
    * コアモジュールを OSS として公開
      * [https://github.com/bbsakura/xk6-gtp](https://github.com/bbsakura/xk6-gtp)
      * [https://github.com/bbsakura/xk6-diameter](https://github.com/bbsakura/xk6-diameter)
  * 倉庫事業者と粘り強く交渉・調整し、SIM 発送機能を内製化。工期を数か月短縮し、**約1,000万円弱** と見積もられていた改修コストを削減
  * CI/CD とログ基盤を整備。Readiness/Liveness Probe を整理・活用し、サービスの安定性を向上
  * SRv6 MUP の研究開発を通じ、IETF 116 において Cisco・古河・Arrcus の製品と、ExaBGP/GoBGP（自作機能を実装）との相互接続検証に成功
    * 具体的には ExaBGP に MUP-BGP を実装し、upstream化を成功

### 仮想基盤開発(2025/10〜現在)
* 説明: NaaS 事業者として、NFV向け仮想基盤をゼロから自社開発し、研究・開発リードを担当
* プログラミング言語: Go, Python, Terraform, Ansible など
* その他キーワード: Linux, OvS, etcd, libvirt, FRR, EVPN-VXLAN, ConnectRPC, Google Cloud, GitHub Actions
* 業務内容
  * NFVをターゲットにした仮想基盤の開発
  * 既存サービス網との相互接続
* 実績
  * 3~5名ほどのチームのリーダーとして人・技術両方の面からプロジェクトを牽引
    * 学生アルバイト等を含めると最大8名ほど
  * クラスタ間でのデータのやり取りなどを含めた設計・開発を実施

### 本務以外での活動実績
* 技術的フィジビリティ確認への貢献
  * サービス展開の実現可能性評価のため、簡易な仮想基盤や RAG を自作
  * それらのサービス開発に向けた求人票（JD）の作成も担当
* 外部への貢献
  * eBPF Meetup Japan 共同オーガナイザー
    * [https://ebpf.connpass.com/](https://ebpf.connpass.com/)
  * 技術広報チームとして活動（アドベントカレンダー主宰・外部発信、ブログレビュー、スポンサー対応、パーカー制作 など）
    * [https://adventar.org/calendars/7980](https://adventar.org/calendars/7980)
    * [https://adventar.org/calendars/8572](https://adventar.org/calendars/8572)
  * Google Cloud Next にて Spanner 開発 PM に機能要望を提案
* 育成
  * 開発チーム内でのメンタリングを通じた後進の育成
  * インフラ開発エンジニアの育成（社内ラボ制度の運用を通じた若手育成）
  * ICTSC（インフラトラブルシューティングコンテスト）の運営参加と、他メンバーの巻き込みを通じた育成
  * 社内輪読会の主催
    * MicroKernel 勉強会（全11回）
    * CPU 勉強会（全12回）

## 任天堂株式会社 (2021/04〜2022/09)
* 契約: フルタイム
* 所属: プラットフォーム開発グループ
* 職位: ソフトウェアエンジニア

### コンソール機開発
* ゲーム機向け SDK の開発およびインフラの設計・構築を担当
* 1億台超のゲーム機に対する設定ファイル配信機能の設計・開発
  keyword: C/C++, Go, AWS（Lambda, DynamoDB）, Datadog, gRPC-Gateway, Terraform, Docker
* WebRTC を用いたリアルタイムコミュニケーション機能
  keyword: C/C++, libwebrtc
* 新人研修を担当。コンソール機の通信を MITM して PCAP を取得し、内部シーケンスを理解する講義を実施
## 公開エントリ
### 登壇資料一覧
* [Go Conference: Goで体感するMultipath TCP ― Go 1.24 時代の MPTCP Listener を理解する](https://speakerdeck.com/takehaya/go-conference-2025-godeti-gan-surumultipath-tcp-go-1-dot-24-shi-dai-no-mptcp-listener-woli-jie-suru) ※CfP 採択 27/244（約9倍）
* [Japan Community Day at KubeCon + CloudNativeCon Japan 2025: Programmable Bandwidth Management with eBPF](https://speakerdeck.com/takehaya/programmable-bandwidth-management-with-ebpf)
* [Japan Community Day at KubeCon + CloudNativeCon Japan 2025: eBPF at Mobile Network Data Plane](https://speakerdeck.com/takehaya/ebpf-at-mobile-network-data-plane) ※招待講演
* [CloudNative Days Winter 2024: eBPF Deep Dive: Architecture and Safety Mechanisms](https://event.cloudnativedays.jp/cndw2024/talks/2398) ※CfP 採択 24/78（約3.25倍）
* [YAPC::Hakodate2024: Perlで始めるeBPF: 自作Loaderの作り方](https://fortee.jp/yapc-hakodate-2024/proposal/2c24d2e4-f488-414f-ae3d-1df24180867b) ※採択（約8.25倍）
* [eBPF Meetup #1: "Exploring XDP: Fundamentals and Real-World Implementations in Mobile Network Data Plane"](https://speakerdeck.com/takehaya/exploring-xdp-fundamentals-and-real-world-implementations-in-mobile-network-data-plane)
* [Wakamonog13 LT: VPPで始めるHigh Performance BGPルーター](https://speakerdeck.com/takehaya/wakamong13-lt-getstarted-with-vpp-high-performance-bgp-router)
* [JANOG53 LT: 自作 k6 Extension を利用した NFV への負荷計測手法の紹介](https://speakerdeck.com/takehaya/janog53-lt-introduction-to-load-measurement-method-for-nfv-using-self-made-k6-extension)
* [PyCon APAC 2023: 自作パケット処理系の性能測定と可視化&改善の PDCA を回して最強のパケット処理系の作り方を学ぼう](https://2023-apac.pycon.jp/timetable?id=G3LDSG) ※CfP 採択（約4.3倍）
* [シン・ITRC meeting 53: SRv6 Mobile User Plane (MUP) の紹介と MUP-BGP の OSS 実装における相互接続性](https://speakerdeck.com/takehaya/srv6-mobile-user-plane-mup-noshao-jie-tomup-bgpnoossshi-zhuang-niokeruxiang-hu-jie-sok-xing-nituite) ※招待講演

### 執筆した外部ブログ

* [eBPF/XDPでパケット処理をするときにやってるテスト方法の紹介 - BBSakura Networks Blog](https://blog.bbsakura.net/posts/2024/12/24/145413)
* [MPTCPのスケジューラーをeBPFで書けるようになった話 - BBSakura Networks Blog](https://blog.bbsakura.net/posts/2023/12/25/172803)
* [IETF 116 Hackathon に参加して SRv6 の開発をしてきました - BBSakura Networks Blog](https://blog.bbsakura.net/posts/2023/04/13/175103)
* [VPPにSRv6 MUP Plugin APIを追加している話 - BBSakura Networks Blog](https://blog.bbsakura.net/posts/add-srv6-mup-plugin-api-to-vpp/)
* [勝手にレポート！BBSakura の社員はどんな環境で仕事をしているのか？ - BBSakura Networks Blog](https://blog.bbsakura.net/posts/bbs-report-workenv/)

### 執筆に携わった論文
* [Multipath Transport Protocol を用いた SRv6 BGP Egress Peer Engineering による高品質・高信頼なコンテンツ配信](https://www.ipsj.or.jp/dp/contents/publication/59/TR0503-03.html)

### その他
* [ICTSC2025 二次予選 問題解説: The Handover of the Handover](https://blog.icttoracon.net/2025/12/27/ictsc2025pr2/mpt/): 学生向けコンテスト ICTSC の運営委員として、問題作成・解説を担当
* [ICTSC 2024 二次予選問題作問・解説 にゃーん](https://blog.icttoracon.net/2024/12/14/ictsc2024pr/ngx/): ICTSC の運営委員として、問題作成・解説を担当
* [JPNIC News & Views Column「もう一つのインターネット：モバイルローミングの世界」](https://www.nic.ad.jp/ja/mailmagazine/backnumber/2024/vol2090.html#column): 依頼を受けてコラムを執筆
* [ICTSC 2023 二次予選問題作問・解説 直径と半径](https://blog.icttoracon.net/2023/12/22/ictsc2023pr/dra/): ICTSC の運営委員として問題を作成

### OSS 貢献
* VyOS
  * SSH Certificate Configuration 機能
    * [https://vyos.dev/T6013](https://vyos.dev/T6013)
    * [https://github.com/vyos/vyos-1x/pull/4234](https://github.com/vyos/vyos-1x/pull/4234)
    * [https://github.com/vyos/vyos-1x/pull/4266](https://github.com/vyos/vyos-1x/pull/4266)
    * [https://github.com/vyos/vyos-documentation/pull/1578](https://github.com/vyos/vyos-documentation/pull/1578)
* VPP
  * [https://github.com/search?q=repo%3AFDio%2Fvpp+hayasaka&type=commits](https://github.com/search?q=repo%3AFDio%2Fvpp+hayasaka&type=commits)
    * srv6-mobile: Implement SRv6 Mobile API funcs（SRv6-MUP の API を定義）
    * sr: support define src ipv6 per encap policy（SRv6 Policy ごとの送信元アドレス切替に対応）
    * ip: support flow-hash gtpv1teid（GTP-U の TEID をハッシュに用いた ECMP を実現）
* ExaBGP
  * MUP-BGP を追加
    * [https://github.com/Exa-Networks/exabgp/pulls?q=is%3Apr+author%3Atakehaya+is%3Aclosed+](https://github.com/Exa-Networks/exabgp/pulls?q=is%3Apr+author%3Atakehaya+is%3Aclosed+)
* Linux
  * ethtool: Add GTP RSS hash options to ethtool.h
  * ice: Implement RSS settings for GTP using ethtool
    * [https://www.spinics.net/lists/netdev/msg979517.html](https://www.spinics.net/lists/netdev/msg979517.html)
* その他
  * llama-index
    * [https://github.com/run-llama/llama_index/pull/13863](https://github.com/run-llama/llama_index/pull/13863)
    * [https://github.com/run-llama/llama_index/pull/13761](https://github.com/run-llama/llama_index/pull/13761)
  * fluvia（NTT Comとのco-author に自分が含まれています）
    * [https://github.com/nttcom/fluvia](https://github.com/nttcom/fluvia)
  * co-author
    * [https://github.com/erkanzileli/co-author/pull/1](https://github.com/erkanzileli/co-author/pull/1)

## EDUCATION
* MSc(在学中): 北陸先端大学院大学 先端科学技術専攻（2024/04〜現在）
* BD: 東北学院大学 工学部 情報基盤工学科（2017/04〜2021/03）

## 資格
* 情報処理安全確保支援士（未登録）: 2025/07
* ネットワークスペシャリスト: 2024/06
* 工事担任者 総合種: 2021/09
* 第二種電気工事士: 2015/08
