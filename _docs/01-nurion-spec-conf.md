---
title: "누리온 시스템 사양 및 구성"
permallink: "/docs/useage/nurion/spec-conf"
description: 기술지원 > 지침서 > 사용법 > 누리온 > 누리온 시스템 사양 및 구성 > 가. 개요
last_modified_at: 2020-06-25
---

# 가. 개요

KISTI 슈퍼컴퓨터 5호기 누리온(NURION)은 리눅스 기반의 초병렬 클러스터 시스템으로 이론최고성능(Rpeak) 25.7PFlops(4호기 Tachyon2의 약 70배)의 연산처리 성능을 갖고 있다.

&#x20;

누리온은 1소켓(CPU)당 성능이 3TFlops(4호기 Tachyon2 전체 성능의 약 1/100)인 매니코어 CPU(68개의 코어로 구성) 8,305개로 구성되어 수십만 코어를 동시에 활용할 수 있는 클러스터 방식의 초고성능 컴퓨팅 시스템이다. 그리고 고성능 인터커넥트(Interconnect), 대용량 스토리지, 버스트 버퍼(Burst Buffer)가 탑재되어 있다. 버스트 버퍼는 응용 프로그램에서 순간적으로 발생하는 대규모 I/O 요청을 원활히 처리 할 수 있다.

&#x20;

누리온은 이러한 대규모 계산 능력을 통해 국가 연구개발(R\&D)의 경쟁력 향상 기여에 목적을 두며, 기후 예측이나 신소재 개발 등 복잡한 문제나 신약개발, 항공 실험 등 실험적으로만 해결하기에는 위험하고 비용이 많이 소요되는 문제를 해결하는 데 기여하고자 한다. 누리온은 이러한 과학기술 문제를 해결하기 위해 기획 단계부터 다양한 분야의 난제를 발굴하는 노력을 병행하고 있다.

&#x20;

또한 누리온은 이러한 연구 개발들을 지원하기 위한 다양한 종류의 소프트웨어를 탑재하고 지속적으로 업그레이드 하고 있으며, 고성능 하드웨어와 유기적인 연동을 통해 최고의 생산성을 유지하기 위해 노력하고 있다. 아울러 최적ㆍ병렬화를 비롯한 다양한 사용자 지원과 거대 문제 및 난제 해결 등을 위한 대형 과제 발굴을 통해서 국가 과학기술 발전과 지능정보사회 구현의 핵심 인프라로서 역할을 수행하고자 한다.

![\[누리온 구성도\]](<../../../../.gitbook/assets/누리온 구성도.png>)

<table class="common-table-03 txt-ac" border="0" cellspacing="0" cellpadding="0"><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 20%;"></colgroup><colgroup><col style="width: 20%;"></colgroup>
<thead>
<tr>
<th style="width: 415px;" colspan="2">구분</th>
<th style="width: 124px;">KNL 계산노드</th>
<th style="width: 124px;">Cpu-only 노드</th>
</tr>
</thead>
<tbody>
<tr>
<td style="width: 415px;" colspan="2">제조사 및 모델</td>
<td style="width: 269px;" colspan="2">Cray CS500</td>
</tr>
<tr>
<td style="width: 415px;" colspan="2">노드수</td>
<td style="width: 124px;">8,305</td>
<td style="width: 124px;">132</td>
</tr>
<tr>
<td style="width: 415px;" colspan="2">성능최고성능(Rpeak)</td>
<td style="width: 124px;">25.3 PFlops</td>
<td style="width: 124px;">0.4 PFlops</td>
</tr>
<tr>
<td style="width: 197px;" rowspan="5">프로세서</td>
<td style="width: 197px;">모델</td>
<td style="width: 124px;">Intel Xeon Phi 7250(KNL)</td>
<td style="width: 124px;">Intel Xeon 6148 (Skylake)</td>
</tr>
<tr>
<td style="width: 197px;">CPU당 이론성능</td>
<td style="width: 124px;">3.0464 TFLOPS</td>
<td style="width: 124px;">1.536 TFLOPS</td>
</tr>
<tr>
<td style="width: 197px;">CPU당 코어수</td>
<td style="width: 124px;">68</td>
<td style="width: 124px;">20</td>
</tr>
<tr>
<td style="width: 197px;">노드당 CPU수</td>
<td style="width: 124px;">1</td>
<td style="width: 124px;">2</td>
</tr>
<tr>
<td style="width: 197px;">On-package Memory</td>
<td style="width: 124px;">16GB, 490GB/s</td>
<td style="width: 124px;">-</td>
</tr>
<tr>
<td style="width: 197px;" rowspan="5">메인메모리</td>
<td style="width: 197px;">모델</td>
<td style="width: 124px;">16GB DDR4-2400</td>
<td style="width: 124px;">16GB DDR4-2666</td>
</tr>
<tr>
<td style="width: 197px;">구성</td>
<td style="width: 124px;">16GB x6, 6Ch per CPU</td>
<td style="width: 124px;">16GB x12, 6Ch per CPU</td>
</tr>
<tr>
<td style="width: 197px;">노드 당 메모리(GB)</td>
<td style="width: 124px;">96GB</td>
<td style="width: 124px;">192GB</td>
</tr>
<tr>
<td style="width: 197px;">CPU당 대역폭</td>
<td style="width: 124px;">115.2GB/s</td>
<td style="width: 124px;">128GB/s</td>
</tr>
<tr>
<td style="width: 197px;">전체크기</td>
<td style="width: 124px;">778.6TB</td>
<td style="width: 124px;">24.8TB</td>
</tr>
<tr>
<td style="width: 197px;" rowspan="4">고성능 인터커넥트</td>
<td style="width: 197px;">토폴로지</td>
<td style="width: 269px;" colspan="2">Fat Tree</td>
</tr>
<tr>
<td style="width: 197px;">Blocking Ratio</td>
<td style="width: 269px;" colspan="2">50% Blocking</td>
</tr>
<tr>
<td style="width: 197px;">Switches 구성</td>
<td style="width: 269px;" colspan="2">278x 48-port OPA edge switches<br>8x 768-port OPA core switches</td>
</tr>
<tr>
<td style="width: 197px;">포트 당 대역폭</td>
<td style="width: 269px;" colspan="2">100Gbps</td>
</tr>
<tr>
<td style="width: 197px;" rowspan="4">고성능 파일시스템(Burst Buffer)</td>
<td style="width: 197px;">서버수</td>
<td style="width: 269px;" colspan="2">DDN IME240 Server 48ea</td>
</tr>
<tr>
<td style="width: 197px;">서버 당 디스크</td>
<td style="width: 269px;" colspan="2">16x 1.2TB NVMe SSD, 2x 0.45TB NVMe SSD</td>
</tr>
<tr>
<td style="width: 197px;">전체 가용 용량</td>
<td style="width: 269px;" colspan="2">0.8PB</td>
</tr>
<tr>
<td style="width: 197px;">대역폭</td>
<td style="width: 269px;" colspan="2">20GB/sec per server, 0.8TB/s total</td>
</tr>
<tr>
<td style="width: 197px;" rowspan="4">병렬파일시스템</td>
<td style="width: 197px;">파일시스템</td>
<td style="width: 124px;" colspan="2">Lustre 2.7.21.3</td>
</tr>
<tr>
<td style="width: 197px;">전체 가용 용량</td>
<td style="width: 269px;" colspan="2">/scratch: 21PB, /home: 0.76PB, /apps: 0.5PB</td>
</tr>
<tr>
<td style="width: 197px;">대역폭</td>
<td style="width: 269px;" colspan="2">0.3TB/s</td>
</tr>
<tr>
<td style="width: 197px;">RAID 구성</td>
<td style="width: 269px;" colspan="2">RAID6(8D+2P)</td>
</tr>
</tbody>
</table>

![\[누리온 시스템 사양 및 구성\]](<../../../../.gitbook/assets/누리온 시스템 사양 및 구성.png>)

# 나. 계산노드

누리온 시스템의 계산노드는 총 8,437개로 매니코어 기반의 Intel Xeon Phi 7250프로세서가 장착된 8,305개 계산노드와 Intel Xeon Gold 6148 프로세서가 장착된 132개 계산노드로 구성되어 있다.

&#x20;

#### KNL(매니코어) 노드

KNL 노드에 장착된 Intel Xeon Phi 7250 프로세서(코드명 Knights Landing)는 1.4GHz 기본 주파수에 68개 코어(hyperthreading off)로 동작한다. L2 캐시 메모리는 34MB이며, 온패키지 메모리인 MCDRAM (Multi-Channel DRAM)은 16GB(대역폭 490GB/s)이다. 노드 당 메모리는 96GB로 16GB DDR4-2400 메모리가 6채널로 구성되어 있다. 2U크기의 인클로저(enclosure)에는 4개의 계산노드가 장착되며, 42U 표준랙에 72개의 계산노드로 구성되어 있다.

![\[KNL 기반 계산노드 블록 다이어그램\]](<../../../../.gitbook/assets/KNL 기반 계산노드 블록 다이어그램.png>)

![\[KNL 기반 계산노드\]](<../../../../.gitbook/assets/KNL 기반 계산노드.png>)

#### SKL(CPU-only) 노드

SKL(CPU-only) 노드에는 2개의 Intexl Xeon Gold 6148 프로세서(코드명 Skylake)가 장착되어 있다. 기본 주파수는 2.4GHz이며 20개의 CPU 코어(hyperthreading off)로 구성된다. L3 캐시 메모리는 27.5MB이며, 각 CPU당 메모리는 96GB(노드 당 192GB)로 16GB DDR4-2666 메모리가 6채널로 구성되어 있다. 2U크기의 인클로저(enclosure)에는 4개의 계산노드가 장착되어 있다.

![\[SKL 기반 CPU-only 노드 블록 다이어그램\]](<../../../../.gitbook/assets/SKL 기반 CPU-only 노드 블록 다이어그램.png>)

![\[SKL 기반 CPU-only 노드\]](<../../../../.gitbook/assets/SKL 기반 CPU-only 노드.png>)

# 다. 인터커넥트 네트워크

노드 간 계산 네트워크 및 파일 I/O 통신을 위한 인터커넥트 네트워크로 인텔 OPA(Omni-Path Architecture)를 사용하고 있다. 100Gbps OPA를 사용하여 Fat-Tree 구조로 계산노드 간 50% blocking, 스토리지 간 non-blocking 네트워크로 구성 하였다. 계산노드와 스토리지는 277개의 48포트 OPA Edge 스위치에 연결되며 모든 Edge 스위치는 8대의 768포트 OPA Director 스위치에 연결 하였다.

![\[인터커넥트 네트워크 구성도\]](<../../../../.gitbook/assets/인터커넥트 네트워크 구성도.png>)

# 라. 스토리지

#### 병렬파일시스템 및 버스트버퍼 구성

Nurion은 IO 처리 및 데이터 보관을 위해 병렬파일시스템과 버스트버퍼(Bust Buffer)를 제공한다. 병렬파일시스템을 위해 스크래치(/scratch 21PB), 홈(/home01, 760TB), 어플리케이션(/app, 507TB) 세 개의 Lustre 파일시스템을 제공하고 있다.

&#x20;

각 파일시스템은 SFA7700X 스토리지 기반의 메타데이터 서버(MDS)와, ES14KX 스토리지 기반의 오브젝트 스토리지 서버(OSS)로 구성된다. 버스트버퍼는 계산 노드와 병렬파일시스템 사이에서 동작하는 NVMe 기반의 IO 캐시로 약 844TB의 용량을 제공한다. Lustre 파일시스템은 계산노드, 로그인노드, 아카이빙 서버(Data Mover)에 마운트되어 IO 서비스를 제공한다.

![\[병렬파일시스템 및 버스트버퍼 전체 랙 구성\]](<../../../../.gitbook/assets/병렬파일시스템 및 버스트버퍼 전체 랙 구성.png>)

![\[PFS 서버 구성\]](<../../../../.gitbook/assets/PFS 서버 구성.png>)

#### 버스트버퍼

\- 개요

버스트버퍼(Burst Buffer, 이하 BB)는 계산노드와 스토리지 (/scratch) 사이의 I/O 가속화를 위한 캐시 레이어로 병렬파일시스템의 small I/O 또는 random I/O에 대한 낮은 성능 보완 및 병렬 IO의 성능 극대화를 위해 5호기에 새로이 도입되었다. I/O 의존성이 높은 사용자 어플리케이션의 성능 향상을 목표로 하고 있으며, KNL 노드를 사용하는 모든 큐에 대해 지원하고 있다.

![\[Burst Buffer 역할\]](<../../../../.gitbook/assets/Burst Buffer 역할.png>) ![\[Burst Buffer 서버 구성\]](<../../../../.gitbook/assets/Burst Buffer 서버 구성.png>)

\- 시스템 구성

BB 구성을 위해 DDN사의 IME240 솔루션이 적용되었으며, 위 \[Burst Buffer 서버 구성] 그림은 BB의 상세 구성을 나타낸다.

<table class="common-table-03 txt-ac" border="0" cellspacing="0" cellpadding="0"><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 70%;"></colgroup>
<tbody>
<tr>
<th>시스템</th>
<td style="text-align: center;">DDN IME240, Infinite Memory Engine Appliance</td>
</tr>
<tr>
<th>소프트웨어 버전</th>
<td style="text-align: center;">CentOS 7.4, IME 1.3</td>
</tr>
<tr>
<th>최대 IO 성능</th>
<td style="text-align: center;">20 GB/s</td>
</tr>
<tr>
<th>네트워크 인터페이스</th>
<td style="text-align: center;">2 x OPA</td>
</tr>
<tr>
<th>SSD 타입</th>
<td style="text-align: center;">1.2TB, NVMe 드라이브</td>
</tr>
<tr>
<th>SDD 수량</th>
<td style="text-align: center;">16ea(1.2TB NVMe) + 1ea(450GB SSD)</td>
</tr>
<tr>
<th>용량(RAW)</th>
<td style="text-align: center;">19.2TB</td>
</tr>
</tbody>
</table>

![\[IME 단일노드 구성\]](<../../../../.gitbook/assets/IME 단일노드 구성.png>)

<table class="common-table-03 txt-ac" border="0" cellspacing="0" cellpadding="0"><colgroup><col style="width: 30%;"></colgroup><colgroup><col style="width: 70%;"></colgroup>
<tbody>
<tr>
<th>총 시스템 수</th>
<td>IME240 x 48대</td>
</tr>
<tr>
<th>총 용량(RAW)</th>
<td>979.2 TB</td>
</tr>
<tr>
<th>총 용량(패리티 적용 시)</th>
<td>816 TB (EC*, 10+2)</td>
</tr>
<tr>
<th>최대 IO 성능</th>
<td>800 GB/s</td>
</tr>
</tbody>
</table>

![\[버스트버퍼 전체 구성\]](<../../../../.gitbook/assets/버스트버퍼 전체 구성.png>)

\*EC : Erasure Coding (설정은 변경될 수 있음)