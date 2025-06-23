# Arm HPC User Group Workshop @ ISC25

The 2025 Arm HPC User Group (AHUG) Workshop is held in conjunction with [**ISC High Performance 2025**](https://www.isc-hpc.com/) in Hamburg, Germany. 

**Date & Time**: June 13rd, 2025 @ 9:00am - 1:00pm <br>
**Location**: Hall X5 - 1st floor, Congress Center Hamburg (CCH), Germany

[**Join the AHUG Slack channel!**](https://join.slack.com/t/a-hug/shared_invite/zt-25r69qm2u-hhEkbN7terYpw7K3W2k6Eg)

## Timetable and Agenda 

<table>
<colgroup>
<col width="10%" />
<col width="10%" />
<col width="50%" />
<col width="30%" />
</colgroup>
<thead>
<tr class="header">
<th>Time</th>
<th>Duration</th>
<th>Title</th>
<th>Speaker</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">09:00-09:05</td>
<td markdown="span">5m</td>
<td markdown="span">**Welcome & Plenary address**</td>
<td markdown="span">Filippo Spiga (NVIDIA / AHUG)</td>
</tr>
<tr>
<td markdown="span">09:05-09:45</td>
<td markdown="span">40m</td>
<td markdown="span"><font size="-1">Invited Talk</font><br>
**Fugaku-LLM: A Large Language Model Trained on the Supercomputer Fugaku** <a href="slides/ISC25_AHUG_Fujitsu">PDF</a></td>
<td markdown="span">Koichi Shirahata (Fujitsu)</td>
</tr>
<tr>
<td markdown="span">09:45-10:10</td>
<td markdown="span">25m</td>
<td markdown="span">**An Overview of the Maturity of SYCL Implementations and Backends for AArch64**</td>
<td markdown="span">Etienne Renault (SiPearl)</td>
</tr>
<tr>
<td markdown="span">10:10-10:35</td>
<td markdown="span">25m</td>
<td markdown="span">**Early results from Isambard 3, one of the first NVIDIA Grace CPU-based systems**</td>
<td markdown="span">Tom Green (Univ. Bristol, BriCS), Simon McIntosh-Smith (Univ. Bristol, BriCS)</td>
</tr>
<tr>
<td markdown="span">10:35-11:00</td>
<td markdown="span">25m</td>
<td markdown="span">**Porting and tuning GROMACS on Arm SVE**</td>
<td markdown="span">Gilles Gouaillardet (RIST)</td>
</tr>
<tr>
<td markdown="span">11:00-11:30</td>
<td markdown="span">30m</td>
<td colspan="3" markdown="span">Coffee break</td>
</tr>
<tr>
<td markdown="span">11:30-11:55</td>
<td markdown="span">25m</td>
<td markdown="span">**MareNostrum5's Graceful landing**</td>
<td markdown="span">Majesa Trimmel (BSC), Fabio Banchelli (BSC)</td>
</tr>
<tr>
<td markdown="span">11:55-12:20</td>
<td markdown="span">25m</td>
<td markdown="span">**Advancing the ARM Ecosystem for European Scientific Flagship Codes**</td>
<td markdown="span">Erwan Raffin (EVIDEN)</td>
</tr>
<tr>
<td markdown="span">12:20-12:45</td>
<td markdown="span">25m</td>
<td markdown="span">**Exploring compiler behavior on an industrial application (OpenRadioss) on modern arm processors**</td>
<td markdown="span">Hugo Bolloré (UVSQ)</td>
</tr>
<tr>
<td markdown="span">12:45-13:00</td>
<td markdown="span">15m</td>
<td markdown="span">**Closing Remarks**</td>
<td markdown="span">Conrad Hillairet (Arm Ltd), Filippo Spiga (NVIDIA / AHUG)</td>
</tr>
</tbody>
</table>

## Abstracts

### (Invited Talk) Fugaku-LLM: A Large Language Model Trained on the Supercomputer Fugaku
**Speaker**: Koichi Shirahata (Fujitsu)<br>
_While not initially designed for large-scale deep learning models like Large Language Models (LLMs), Japan's flagship supercomputer, Fugaku, provided a unique opportunity. This work details the optimization of deep learning frameworks for distributed parallel execution on Fugaku, creating a high-performance computing environment for LLM training. A novel LLM was trained from scratch using a large dataset primarily focused on Japanese text._

### An Overview of the Maturity of SYCL Implementations and Backends for AArch64
**Speaker**: Etienne Renault (SiPearl)<br>
_Modern HPC systems are heterogeneous at both processing units level and memory level. This heterogeneity can be leveraged using SYCL which is a programming model that allow to abstract  devices where some part of the computation is offloaded. With increasing performance, ARM cores are today a suitable option for offloading. This talk will focus on the AArch64 SYCL ecosystem and its implementations, each supporting a variety of backends. In this context application developers need to carefully consider each combination of [framework x backend x device] in order to take the most out of their code. This talk focuses on performance of  two SYCL implementations (DPC++ and AdaptiveCpp) for AArch64 and evaluate them against HeCBench. The aim is to help the developer to quickly pick the correct backend according to his/her needs. A peak on our latest advances to strengthen the SYCL ecosystem will be presented : among other integration of NUMA awareness and Outer-Loop Vectorization._

### Early results from Isambard 3, one of the first NVIDIA Grace CPU-based systems
**Speaker**: Tom Green, Prof. Simon McIntosh-Smith (University of Bristol, BriCS)<br>
_The University of Bristol has been running production Arm-based HPC services since commissioning the Isambard 1 supercomputer back in 2018. This first system was based on Marvell ThunderX2 Arm-based CPUs, and the follow-on, Isambard 2, continued the theme, adding Fujitsu A64fx processors. Isambard 3 has recently gone into production, delivering one of the first substantial NVIDIA Grace-Grace CPU systems. Isambard 3's nodes each deliver 144 fast Arm Neoverse v2 cores and around 1 TB/s of memory bandwidth. The system is delivered by HPE, and exploits their Slingshot 11 200 Gbps network to connect the 384 nodes in the system, for a total of 55,296 cores. In this talk we will present early results from real users running a wide range of scientific applications on the system, as well as summarising useful lessons learned so far._

### Porting and tuning GROMACS on Arm SVE
**Speaker**: Gilles Gouaillardet (RIST)<br>
_This short talk will explain how SVE support was added to GROMACS, the challenges that were met and how they were overcome, and describe the optimizations that were implemented in order to improve performances on A64fx._


### MareNostrum5's Graceful landing
**Speaker**: Fabio Banchelli, Majesa Trimmel (BSC)<br>
_In this talk, we introduce the Next Generation General Purpose Partition of MareNostrum 5, deployed at the Barcelona Supercomputing Center. It comprises 400 nodes based on the NVIDIA Grace CPU Superchip. Our goal is to share our experience working on a full-scale Grace-based system. We present results from simple synthetic micro-benchmarks to production-ready scientific codes. Micro-benchmarks allow us to evaluate specific hardware features, while HPC applications allow us to conduct experiments across multiple nodes and analyze the system's scalability. We also leverage the power monitoring infrastructure deployed at BSC, which has been extended to support the power telemetry tools provided by the Grace CPU. Lastly, we share some insights on the system software, such as the multiple compiler toolchains and math libraries to choose from._

### Advancing the ARM Ecosystem for European Scientific Flagship Codes
**Speaker**: Erwan Raffin (EVIDEN)<br>
_The EMOPASS project aims at improving the Arm ecosystem for HPC. This includes the analysis of flagship HPC codes on Arm latest HPC processors using leading-edge profiling tool, MAQAO. This tool is being used to study, among key scientific applications, flagship codes from several European CoEs, leading to feedback and further improvements to the applications, compilers and to MAQAO itself. We will present several studies made in the context of the project, where these CoEs applications and kernels were used to evaluate compilers and micro-architecture capabilities. Moreover, We will look at the positive feedback loop this helped create for end-users of Arm CPUs. This includes new features in MAQAO such as thread binding and activity, and improvements to LLVM such as improved vectorization and Fortran support in the new flang front-end._

### Exploring compiler behavior on an industrial application (OpenRadioss) on modern arm processors
**Speaker**: Hugo Bolloré (University of Versailles Saint-Quentin -UVSQ)<br>
_On modern processors, compiler task is very difficult (dealing with large Instruction Level Parallelism and various vector lengths/instruction sets available) and often compilers generate suboptimal code. In this presentation, we will demonstrate how MAQAO (www.maqao.org) can be used to explore and detect compiler mistakes or suboptimal decisions. Such an exploration will rely on MAQAO advanced binary analysis features combined with simplified performance models (Code Quality Analysis). This work will be carried out with two compilers ACFL and GFortran using different compiler flags on OpenRadioss, a well known crash & impact open-source code. Target hardware will be AWS Graviton3 and AWS Graviton4 processors. A large effort will be devoted to perform comparative analysis between different compilers, compiler options and hardware._