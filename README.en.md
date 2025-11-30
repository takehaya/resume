# Resume

## Personal Data
* Name: Takeru Hayasaka
* ID: takemioIO, takehaya
* This document describes contributions made as a full-time professional. For information on internships or contests during student years, see the profile site below.
  * [https://profile.takemio.net/](https://profile.takemio.net/)

## Summary
I have worked across a wide range of system development, from in-house mobile core development and operation to SDK development for game consoles, covering software and infrastructure. I have achieved significant performance improvements and cost reductions by optimizing high-performance network processing and cloud platforms, mainly using C and Go, and I have contributed to OSS projects. I have also supported the growth of both my organization and the broader community by organizing internal study groups, mentoring junior engineers, giving talks, and writing technical blogs. I drive projects and talent development with a focus on proactive problem solving and technical expertise.

## Sakura Internet Inc. / BBSakura Networks Inc. (Oct 2022–Present)
* Seconded from Sakura Internet Inc.
* Full-time
* Mobile Development Team
* Senior Software Engineer
### Full MVNO Business
* Overview: Responsible for end-to-end development and operation of an in-house mobile core for a full MVNO business
* Languages: C, Go, Python, Terraform, Ansible
* Keywords: Google Cloud (Cloud Run, Spanner, BigQuery, Cloud Monitoring), GitHub Actions, Linux, eBPF, XDP, ConnectRPC, gRPC
* Responsibilities
  * Mobile core development
  * BGP-based interconnection operations with other MVNOs
  * End-to-end monitoring systems for mobile environments
  * R&D on SRv6 MUP
* Achievements
  * Reduced annual cost of traffic aggregation by a factor of about 30,000 under typical workloads by migrating from Cloud Monitoring to BigQuery
  * Improved performance of packet forwarding services by approximately 200 times through tuning SCTP-related kernel parameters
  * Implemented multicore support in the packet exchange system, expanding mobile connection throughput to 100 Gbps (about 27 times the previous level)
    * Upstreamed part of the work to the Linux kernel and ethtool after extensive coordination
      * ethtool: Add GTP RSS hash options to ethtool.h
      * ice: Implement RSS settings for GTP using ethtool
        * [https://www.spinics.net/lists/netdev/msg979517.html](https://www.spinics.net/lists/netdev/msg979517.html)
  * Avoided an estimated 40–50 million yen in license costs for commercial load-testing tools by developing an in-house alternative for NFV performance testing
    * Planned and executed independently, including hiring student assistants
    * Released core modules as OSS
      * [https://github.com/bbsakura/xk6-gtp](https://github.com/bbsakura/xk6-gtp)
      * [https://github.com/bbsakura/xk6-diameter](https://github.com/bbsakura/xk6-diameter)
  * Internalized SIM shipping operations through persistent negotiation with logistics vendors, shortening delivery timelines by several months and reducing an estimated cost of nearly 10 million yen
  * Improved service stability through CI/CD and logging infrastructure, including refinement and utilization of readiness and liveness probes
  * Achieved multi-vendor interoperability at IETF 116 for SRv6 MUP using Cisco, Furukawa, and Arrcus products with ExaBGP/GoBGP (including custom features)
    * Implemented MUP-BGP in ExaBGP and successfully upstreamed it

### Additional Activities

* Technical feasibility contributions
  * Built lightweight virtual platforms and RAG systems to evaluate service launch feasibility
  * Drafted job descriptions for future service development
* External contributions
  * Co-organizer of eBPF Meetup Japan
    * [https://ebpf.connpass.com/](https://ebpf.connpass.com/)
  * Member of the technical advocacy team (Advent Calendar management, external outreach, blog reviews, sponsor coordination, hoodie production)
    * [https://adventar.org/calendars/7980](https://adventar.org/calendars/7980)
    * [https://adventar.org/calendars/8572](https://adventar.org/calendars/8572)
  * Proposed feature requests to a Spanner product manager at Google Cloud Next
* Mentoring
  * Trained infrastructure development engineers through internal lab programs
  * Participated in ICTSC operations and fostered involvement of other members
  * Organized internal reading groups
    * Microkernel study group (11 sessions)
    * CPU study group (12 sessions)

## Nintendo Co., Ltd. (Apr 2021–Sep 2022)
* Full-time
* Platform Development Group
* Software Engineer

### Console Development
* Developed SDKs and designed and built infrastructure for game consoles
* Designed and developed configuration file distribution systems for more than 100 million consoles
  Keywords: C/C++, Go, AWS (Lambda, DynamoDB), Datadog, gRPC-Gateway, Terraform, Docker
* Worked on real-time communication features using WebRTC
  Keywords: C/C++, libwebrtc
* Conducted new-hire training, including lectures on capturing PCAP by performing MITM on console communications to understand internal sequences

## Public Entries

### Presentation Materials
* Go Conference: Multipath TCP in Go 1.24 Era
  [https://speakerdeck.com/takehaya/go-conference-2025-godeti-gan-surumultipath-tcp-go-1-dot-24-shi-dai-no-mptcp-listener-woli-jie-suru](https://speakerdeck.com/takehaya/go-conference-2025-godeti-gan-surumultipath-tcp-go-1-dot-24-shi-dai-no-mptcp-listener-woli-jie-suru)
* KubeCon + CloudNativeCon Japan Community Day 2025: Programmable Bandwidth Management with eBPF
  [https://speakerdeck.com/takehaya/programmable-bandwidth-management-with-ebpf](https://speakerdeck.com/takehaya/programmable-bandwidth-management-with-ebpf)
* KubeCon + CloudNativeCon Japan Community Day 2025: eBPF at Mobile Network Data Plane
  [https://speakerdeck.com/takehaya/ebpf-at-mobile-network-data-plane](https://speakerdeck.com/takehaya/ebpf-at-mobile-network-data-plane)
* CloudNative Days Winter 2024: eBPF Deep Dive
  [https://event.cloudnativedays.jp/cndw2024/talks/2398](https://event.cloudnativedays.jp/cndw2024/talks/2398)
* YAPC::Hakodate 2024: Starting eBPF with Perl
  [https://fortee.jp/yapc-hakodate-2024/proposal/2c24d2e4-f488-414f-ae3d-1df24180867b](https://fortee.jp/yapc-hakodate-2024/proposal/2c24d2e4-f488-414f-ae3d-1df24180867b)
* eBPF Meetup #1: Exploring XDP
  [https://speakerdeck.com/takehaya/exploring-xdp-fundamentals-and-real-world-implementations-in-mobile-network-data-plane](https://speakerdeck.com/takehaya/exploring-xdp-fundamentals-and-real-world-implementations-in-mobile-network-data-plane)
* Wakamonog13 LT: High-Performance BGP Router with VPP
  [https://speakerdeck.com/takehaya/wakamong13-lt-getstarted-with-vpp-high-performance-bgp-router](https://speakerdeck.com/takehaya/wakamong13-lt-getstarted-with-vpp-high-performance-bgp-router)
* JANOG53 LT: Load Measurement for NFV Using Custom k6 Extension
  [https://speakerdeck.com/takehaya/janog53-lt-introduction-to-load-measurement-method-for-nfv-using-self-made-k6-extension](https://speakerdeck.com/takehaya/janog53-lt-introduction-to-load-measurement-method-for-nfv-using-self-made-k6-extension)
* PyCon APAC 2023: Packet Processing Performance Evaluation and Improvement
  [https://2023-apac.pycon.jp/timetable?id=G3LDSG](https://2023-apac.pycon.jp/timetable?id=G3LDSG)
* ITRC Meeting 53: SRv6 MUP and Interoperability with OSS MUP-BGP
  [https://speakerdeck.com/takehaya/srv6-mobile-user-plane-mup-noshao-jie-tomup-bgpnoossshi-zhuang-niokeruxiang-hu-jie-sok-xing-nituite](https://speakerdeck.com/takehaya/srv6-mobile-user-plane-mup-noshao-jie-tomup-bgpnoossshi-zhuang-niokeruxiang-hu-jie-sok-xing-nituite)

### External Blog Posts
* [https://blog.bbsakura.net/posts/2024/12/24/145413](https://blog.bbsakura.net/posts/2024/12/24/145413)
* [https://blog.bbsakura.net/posts/2023/12/25/172803](https://blog.bbsakura.net/posts/2023/12/25/172803)
* [https://blog.bbsakura.net/posts/2023/04/13/175103](https://blog.bbsakura.net/posts/2023/04/13/175103)
* [https://blog.bbsakura.net/posts/add-srv6-mup-plugin-api-to-vpp/](https://blog.bbsakura.net/posts/add-srv6-mup-plugin-api-to-vpp/)
* [https://blog.bbsakura.net/posts/bbs-report-workenv/](https://blog.bbsakura.net/posts/bbs-report-workenv/)

### Papers
* Multipath Transport Protocol-based SRv6 BGP Egress Peer Engineering
  [https://www.ipsj.or.jp/dp/contents/publication/59/TR0503-03.html](https://www.ipsj.or.jp/dp/contents/publication/59/TR0503-03.html)

### Others
* ICTSC 2024 Problem Design and Explanation
  [https://blog.icttoracon.net/2024/12/14/ictsc2024pr/ngx/](https://blog.icttoracon.net/2024/12/14/ictsc2024pr/ngx/)
* JPNIC News & Views Column
  [https://www.nic.ad.jp/ja/mailmagazine/backnumber/2024/vol2090.html#column](https://www.nic.ad.jp/ja/mailmagazine/backnumber/2024/vol2090.html#column)
* ICTSC 2023 Problem Design
  [https://blog.icttoracon.net/2023/12/22/ictsc2023pr/dra/](https://blog.icttoracon.net/2023/12/22/ictsc2023pr/dra/)

### OSS Contributions
* VyOS
  * SSH Certificate Configuration
    * [https://vyos.dev/T6013](https://vyos.dev/T6013)
    * [https://github.com/vyos/vyos-1x/pull/4234](https://github.com/vyos/vyos-1x/pull/4234)
    * [https://github.com/vyos/vyos-1x/pull/4266](https://github.com/vyos/vyos-1x/pull/4266)
    * [https://github.com/vyos/vyos-documentation/pull/1578](https://github.com/vyos/vyos-documentation/pull/1578)
* VPP
  * [https://github.com/search?q=repo%3AFDio%2Fvpp+hayasaka&type=commits](https://github.com/search?q=repo%3AFDio%2Fvpp+hayasaka&type=commits)
    * SRv6 Mobile API functions
    * Source IPv6 per SRv6 Policy
    * Flow-hash support for GTP-U TEID
* ExaBGP
  * Added MUP-BGP
    * [https://github.com/Exa-Networks/exabgp/pulls?q=is%3Apr+author%3Atakehaya+is%3Aclosed+](https://github.com/Exa-Networks/exabgp/pulls?q=is%3Apr+author%3Atakehaya+is%3Aclosed+)
* Linux
  * ethtool: Add GTP RSS hash options
  * ice: Implement RSS settings for GTP
    * [https://www.spinics.net/lists/netdev/msg979517.html](https://www.spinics.net/lists/netdev/msg979517.html)
* Other
  * llama-index
    * [https://github.com/run-llama/llama_index/pull/13863](https://github.com/run-llama/llama_index/pull/13863)
    * [https://github.com/run-llama/llama_index/pull/13761](https://github.com/run-llama/llama_index/pull/13761)
  * fluvia (co-author)
    * [https://github.com/nttcom/fluvia](https://github.com/nttcom/fluvia)
  * co-author
    * [https://github.com/erkanzileli/co-author/pull/1](https://github.com/erkanzileli/co-author/pull/1)

## Education
* MSc (in progress): Japan Advanced Institute of Science and Technology, Advanced Science and Technology (Apr 2024–Present)
* BD: Tohoku Gakuin University, Faculty of Engineering, Department of Information Infrastructure Engineering (Apr 2017–Mar 2021)

## Certifications
* Registered Information Security Specialist (passed, registration pending): Jul 2025
* Network Specialist: Jun 2024
* Telecommunications Chief Engineer, General Category: Sep 2021
* Class 2 Electrician: Aug 2015

## Language Level
- Japanese: Native
- English: Beginner ~ Intermediate