# 職務経歴書

## 個人データ
- 氏名: 早坂 彪流 / HAYASAKA Takeru
- ID: `takemioIO`, `takehaya`
- https://profile.takemio.net/

## 職務要約
モバイルコアの自社開発・運用やゲーム機向けSDK開発など、ソフトウェアからインフラまで幅広い領域でシステム開発に従事してきました。C/Goを中心とした高性能ネットワーク処理やクラウド基盤の最適化により、大幅な性能改善やコスト削減を実現するとともに、OSSへの貢献も行ってきました。
加えて、社内勉強会の主催や若手育成、外部登壇や技術ブログ執筆を通じて知見を広く共有し、組織とコミュニティ双方の発展に貢献してきました。課題解決に向けた主体的な行動と技術力を両輪として、プロジェクト推進と人材育成に取り組んでおります。

## さくらインターネット株式会社 / BBSakura Networks株式会社(2022/10~現在)
- さくらインターネット株式会社から出向
- 契約: フルタイム
- 所属: モバイル開発チーム
- 職位: シニアソフトウェアエンジニア
### フルMVNO事業
- 説明: フルMVNO事業者として一からモバイルコア自作し、運用開発をしています
- プログラミング言語: C, Go, Python, Terraform, Ansible...etc
- その他キーワード: Google Cloud(Cloud Run, Spanner, Bigquery, Cloud monitoring ..etc), Github Actions, Linux, eBPF,　XDP, ConnectRPC, gRPC
- 業務内容
  - モバイルコア開発
  - 他のMVNOとのBGPを利用した相互接続オペレーション
  - モバイル環境のE2E監視システム
  - SRv6 MUPの研究開発
- 実績
  - トラヒック集計機能の年間コストを通常ワークロード時で3万倍削減に成功（CM->BQ移行によるリソース最適化の結果）
  - パケット転送機能を持つサービスのSCTPのカーネルパラメータチューニングなどを施し、200倍性能を改善した
  - パケット交換機のマルチコア化を実現し、モバイル接続を100Gbpsで裁くことができるようにしました。これは通常時の27倍の高速化になります。
    - またこの成果の一部はLinux Kernel, ethtoolへのUpstream化にも成功しました。これは粘り強く交渉した結果でもあります。
      - ethtool: Add GTP RSS hash options to ethtool.h
      - ice: Implement RSS settings for GTP using ethtool
        - https://www.spinics.net/lists/netdev/msg979517.html
  - 負荷試験ツールはベンダからの購入では4~5000万するライセンス費用がかかります。それの自作を行うことで、その費用を削減しモバイルコアで使われるNFVの性能測定を可能にしました。
    - これらは主体的に行われており、学生アルバイトの採用なども含めて企画立案し、実行しました。
    - これらはコアになるモジュールはOSSとして公開されています。
      - https://github.com/bbsakura/xk6-gtp
      - https://github.com/bbsakura/xk6-diameter
  - 倉庫事業者との交渉・調整を粘り強く行い、SIM発送機能を自作したことで工期を数ヶ月短縮し、更に1000万弱が見積もられてた改修コストを削減しました。
  - CI/CDやログ周りの整備に取り組み、Readiness ProbeとLiveness Probeの整理や利活用を行いサービスの安定性に貢献しました。
### 本務以外での活動実績
- 技術的にフィジビリティ確認の貢献
  - サービス展開の実現可能性のために簡易な仮想基盤自作やRAG自作を行いました。
  - それらのサービス開発のJDの記述も行いました。
- 外部への貢献
  - eBPF Meetup Japanの共同オーガナイザー
    - https://ebpf.connpass.com/
  - 技術広報チームとしての活動（アドベントカレンダーの主宰それを通じた外部への知見発信、ブログレビュー、スポンサー対応、パーカー作成など）
    - https://adventar.org/calendars/7980
    - https://adventar.org/calendars/8572
  - Google Cloud NextでのSpanner開発PMへの機能要望
- 育成
  - インフラ開発エンジニアの育成活動
    - ラボ制度が社内にありその環境の運用を通じて、若手の育成に大きく貢献しました。
  - ICTSC（インフラトラブルシューティングコンテスト）の運営参加と他メンバーの巻き込みを通じた育成
  - 社内輪読会の主催
    - MicroKernel勉強会（全11回）
    - CPU勉強会（全12回）

## 任天堂株式会社(2021/04~2022/09)
- 契約: フルタイム
- 所属: プラットフォーム開発グループ
- 職位: ソフトウェアエンジニア
### コンソール機開発
- ゲーム機におけるSDK開発およびインフラの設計と構築に取り組んでいました
- 一億代を超えるゲーム機本体に対する設定ファイル配信機能の設計と開発: keyword: C/C++,Go,AWS{lambda, dynamodb}, datadog,gRPC-GW,terraform,docker
- WebRTCを利用したリアルタイムコミュニケーション機能: keyword: C/C++, libwebrtc
- 新人向けの研修担当: コンソール機が行う通信をMITMをしてDumpし、理解する講義などを行いました

## 公開エントリ
### 登壇資料一覧
- [Go Conference: Goで体感するMultipath TCP ― Go 1.24 時代の MPTCP Listener を理解する](https://speakerdeck.com/takehaya/go-conference-2025-godeti-gan-surumultipath-tcp-go-1-dot-24-shi-dai-no-mptcp-listener-woli-jie-suru)※CfP投稿は 244/27 = 約 9 倍の倍率
- [Japan Community Day at KubeCon + CloudNativeCon Japan 2025: Programmable Bandwidth Management with eBPF](https://speakerdeck.com/takehaya/programmable-bandwidth-management-with-ebpf)
- [Japan Community Day at KubeCon + CloudNativeCon Japan 2025: eBPF at Mobile Network Data Plane](https://speakerdeck.com/takehaya/ebpf-at-mobile-network-data-plane)招待された講演
- [CloudNative Days Winter 2024: eBPF Deep Dive: Architecture and Safety Mechanisms](https://event.cloudnativedays.jp/cndw2024/talks/2398)※CfP投稿は 78/24 = 3.25倍の倍率
- [YAPC::Hakodate2024: Perlで始めるeBPF: 自作Loaderの作り方](https://fortee.jp/yapc-hakodate-2024/proposal/2c24d2e4-f488-414f-ae3d-1df24180867b)※8.25倍の倍率。
- [eBPF Meetup #1: "Exploring XDP: Fundamentals and Real-World Implementations in Mobile Network Data Plane"](https://speakerdeck.com/takehaya/exploring-xdp-fundamentals-and-real-world-implementations-in-mobile-network-data-plane)
- [Wakamonog13 LT: VPPで始めるHigh Performance BGPルーター](https://speakerdeck.com/takehaya/wakamong13-lt-getstarted-with-vpp-high-performance-bgp-router)
- [JANOG53 LT / 自作k6 Extension利用した NFVへの負荷計測手法の紹介](https://speakerdeck.com/takehaya/janog53-lt-introduction-to-load-measurement-method-for-nfv-using-self-made-k6-extension)
- [PyCon APAC 2023: 自作パケット処理系の性能測定と可視化&改善のPDCAを回して最強のパケット処理系の作り方を学ぼう](https://2023-apac.pycon.jp/timetable?id=G3LDSG)※CfP投稿は約4.3倍
- [シン・ITRC meeting 53 / SRv6 Mobile User Plane(MUP) の紹介とMUP-BGPのOSS実装における相互接続性について](https://speakerdeck.com/takehaya/srv6-mobile-user-plane-mup-noshao-jie-tomup-bgpnoossshi-zhuang-niokeruxiang-hu-jie-sok-xing-nituite)
招待された公演

### 執筆した外部ブログ
- [eBPF/XDPでパケット処理をするときにやってるテスト方法の紹介 - BBSakura Networks Blog](https://blog.bbsakura.net/posts/2024/12/24/145413)
- [MPTCPのスケジューラーをeBPFで書けるようになった話 - BBSakura Networks Blog](https://blog.bbsakura.net/posts/2023/12/25/172803)
- [IETF 116 Hackathon に参加して SRv6 の開発をしてきました - BBSakura Networks Blog](https://blog.bbsakura.net/posts/2023/04/13/175103)
- [VPPにSRv6 MUP Plugin APIを追加している話 - BBSakura Networks Blog](https://blog.bbsakura.net/posts/add-srv6-mup-plugin-api-to-vpp/)
- [勝手にレポート！BBSakura の社員はどんな環境で仕事をしているのか？ - BBSakura Networks Blog](https://blog.bbsakura.net/posts/bbs-report-workenv/)

### 執筆に携わった論文
- [Multipath Transport Protocol を用いた SRv6 BGP Egress Peer Engineering による高品質・高信頼なコンテンツ配信](https://www.ipsj.or.jp/dp/contents/publication/59/TR0503-03.html)

### その他
- [ICTSC 2024 二次予選問題作問・解説 にゃーん](https://blog.icttoracon.net/2024/12/14/ictsc2024pr/ngx/): ICTSCという学生向けコンテストの運営委員として参加して問題を作問しました
- [JPNIC News & Views Column「もう一つのインターネット：モバイルローミングの世界」](https://www.nic.ad.jp/ja/mailmagazine/backnumber/2024/vol2090.html#column): JPNICから依頼を受けてコラムを書きました
- [ICTSC 2023 二次予選問題作問・解説 直径と半径](https://blog.icttoracon.net/2023/12/22/ictsc2023pr/dra/): ICTSCという学生向けコンテストの運営委員として参加して問題を作問しました

### OSS貢献
- vyos
  - SSH Certificate configuration という機能
    - https://vyos.dev/T6013
    - https://github.com/vyos/vyos-1x/pull/4234
    - https://github.com/vyos/vyos-1x/pull/4266
    - https://github.com/vyos/vyos-documentation/pull/1578
- vpp
  - https://github.com/search?q=repo%3AFDio%2Fvpp+hayasaka&type=commits
    - srv6-mobile: Implement SRv6 mobile API funcs
      - SRv6-MUPのAPIを定義した
    - sr: support define src ipv6 per encap policy
      - SRv6 policy毎にSrcアドレスを変更可能にする
    - ip: support flow-hash gtpv1teid
      - GTP-UのTEIDをベースにHashを取ってECMPできる
- exabgp
  - MUP-BGPの追加
    - https://github.com/Exa-Networks/exabgp/pulls?q=is%3Apr+author%3Atakehaya+is%3Aclosed+
- Linux
  - ethtool: Add GTP RSS hash options to ethtool.h
  - ice: Implement RSS settings for GTP using ethtool
      - https://www.spinics.net/lists/netdev/msg979517.html
- その他細々としたもの
  - llama-index
    - https://github.com/run-llama/llama_index/pull/13863
    - https://github.com/run-llama/llama_index/pull/13761
  - fulvia(NTTCom, co-autherに自分が含まれてるのがわかると思います)
    - https://github.com/nttcom/fluvia
  - co-auther
    - https://github.com/erkanzileli/co-author/pull/1


## EDUCATION
- MD: 北陸先端大学院大学 先端科学技術専攻: 2024/04-現在
- BD: 東北学院大学 工学部 情報基盤工学科: 2017/04 - 2021/03

## 資格
- 情報処理安全確保支援士(未登録): 2025/07
- ネットワークスペシャリスト: 2024/06
- 工事担任者総合種: 2021/09
- 電気工事士2種: 2015/08
