# Search-Query-SoK

This repository is the search log for the systematic literature review behind our SoK on zero-knowledge (ZK) blockchain interoperability protocols. It lists the database searches used for screening and the number of records each returned.

The academic search was run in two rounds, on 1 March 2026 and 30 September 2026. Screening and inclusion counts are reported in Section 4 of the SoK; the counts below are records identified before deduplication.

## Counts
| Database | Round 1 (1 Mar 2026) | Round 2 (30 Sep 2026) |
|---|---:|---:|
| ScienceDirect | 568 | 799 |
| Scopus | 172 | 188 |
| IEEE Xplore | 124 | 154 |
| ACM Digital Library | 221 | 277 |
| Web of Science | 207 | 263 |
| Google Scholar | 2,000 | 2,000 |
| **All sources, before deduplication** | **3,292** | **3,681** |

ScienceDirect totals comprise five query partitions per round; their individual counts are listed [below](#sciencedirect). Counts are records, not unique papers: duplicates within and across sources were removed during screening. Google Scholar's 2,000 records per round are the first 400 results in each of five publication-year intervals.

## The query

The same query was used everywhere, except in ScienceDirect (see below). It has two parts joined by `OR`:

- **Part A** (the first block) matches papers that use an interoperability term *and* a ZK term.
- **Part B** (the last block) matches phrases that already combine the two, such as "zk light client" or "ZK atomic swap".

```text
(
  ( "blockchain interoperability" OR "cross-chain" OR "cross chain" OR "cross-ledger" OR "cross ledger"
    OR interchain OR "inter-chain" OR "blockchain bridge" OR "cross-chain bridge" OR "cross-chain protocol"
    OR "interoperability protocol" OR "cross-chain communication" OR "cross-chain transaction"
    OR "cross-chain transfer" OR "chain relay" OR "blockchain relay" )
  AND
  ( "zero-knowledge" OR "zero knowledge" OR "zero-knowledge proof" OR "zero knowledge proof" OR ZKP
    OR NIZK OR "zk-SNARK" OR zkSNARK OR "zk-STARK" OR zkSTARK OR SNARK )
)
OR
( "ZK bridge" OR "zk bridge" OR "zero-knowledge bridge" OR "zero knowledge bridge" OR "ZKP bridge"
  OR "succinct light client" OR "zk light client" OR "ZK light client" OR "zero-knowledge light client"
  OR "cross-chain SNARK" OR "cross chain SNARK" OR "cross-chain proof" OR "cross chain proof"
  OR "validity bridge" OR "proof-carrying data" OR "proof carrying data" OR "chain relay SNARK"
  OR "cross-chain ZKP" OR "cross chain ZKP" OR "cross-chain zero-knowledge" OR "cross-chain zero knowledge"
  OR "zero-knowledge interoperability" OR "zero knowledge interoperability"
  OR "atomic swap zero knowledge" OR "zero-knowledge atomic swap" OR "ZK atomic swap" )
```

## Searches

The links below open each search with the query and filters that were used. Scopus, Web of Science and ScienceDirect need institutional access.


### ScienceDirect

ScienceDirect limits how many Boolean connectors one search may use, so the query was split into five partitions. Counts are shown as **Round 1 / Round 2**:

| Partition | Search | Counts |
|---|---|---:|
| 1 | [ScienceDirect search](<https://www.sciencedirect.com/search?qs=%28%0A++%22blockchain+interoperability%22%0A++OR+%22cross-chain%22%0A++OR+%22cross-ledger%22%0A++OR+interchain%0A%29%0AAND%0A%28%0A++%22zero-knowledge%22%0A++OR+ZKP%0A++OR+%22zk-SNARK%22%0A++OR+%22zk-STARK%22%0A%29>) | 272 / 413 |
| 2 | [ScienceDirect search](<https://www.sciencedirect.com/search?qs=%28+++%22blockchain+bridge%22+++OR+%22cross-chain+bridge%22+++OR+%22cross-chain+protocol%22+++OR+%22interoperability+protocol%22+%29+AND+%28+++%22zero-knowledge%22+++OR+ZKP+++OR+%22zk-SNARK%22+++OR+%22zk-STARK%22+%29>) | 131 / 159 |
| 3 | [ScienceDirect search](<https://www.sciencedirect.com/search?qs=%28%0A++%22cross-chain+communication%22%0A++OR+%22cross-chain+transaction%22%0A++OR+%22cross-chain+transfer%22%0A++OR+%22blockchain+relay%22%0A%29%0AAND%0A%28%0A++%22zero-knowledge%22%0A++OR+ZKP%0A++OR+%22zk-SNARK%22%0A++OR+%22zk-STARK%22%0A%29>) | 92 / 137 |
| 4 | [ScienceDirect search](<https://www.sciencedirect.com/search?qs=%22ZK+bridge%22%0AOR+%22zero-knowledge+bridge%22%0AOR+%22ZKP+bridge%22%0AOR+%22succinct+light+client%22%0AOR+%22zk+light+client%22%0AOR+%22zero-knowledge+light+client%22%0AOR+%22cross-chain+SNARK%22%0AOR+%22cross-chain+proof%22>) | 12 / 16 |
| 5 | [ScienceDirect search](<https://www.sciencedirect.com/search?qs=%22validity+bridge%22%0AOR+%22proof-carrying+data%22%0AOR+%22chain+relay+SNARK%22%0AOR+%22cross-chain+ZKP%22%0AOR+%22cross-chain+zero-knowledge%22%0AOR+%22zero-knowledge+interoperability%22%0AOR+%22atomic+swap+zero+knowledge%22%0AOR+%22zero-knowledge+atomic+swap%22>) | 61 / 74 |
| **Total** | | **568 / 799** |

The first partition used this shortened query:

```text
( "blockchain interoperability" OR "cross-chain" OR "cross-ledger" OR interchain )
AND ( "zero-knowledge" OR ZKP OR "zk-SNARK" OR "zk-STARK" )
```

Each partition's counts are included in the table above; together they match the ScienceDirect round totals in the methodology.

### Scopus

**Search:** [Scopus saved search](<https://www.scopus.com/pages/search/publications?searchId=4faf0973-296e-446e-b74d-5cf3268c94d0>)

Round 1: 172 records. Round 2: 188 records.

### IEEE Xplore

**Search:** [IEEE Xplore search](<https://ieeexplore.ieee.org/search/searchresult.jsp?queryText=((%22blockchain%20interoperability%22%20OR%20%22cross-chain%22%20OR%20%22cross%20chain%22%20OR%20%22cross-ledger%22%20OR%20%22cross%20ledger%22%20OR%20interchain%20OR%20%22inter-chain%22%20OR%20%22blockchain%20bridge%22%20OR%20%22cross-chain%20bridge%22%20OR%20%22cross-chain%20protocol%22%20OR%20%22interoperability%20protocol%22%20OR%20%22cross-chain%20communication%22%20OR%20%22cross-chain%20transaction%22%20OR%20%22cross-chain%20transfer%22%20OR%20%22chain%20relay%22%20OR%20%22blockchain%20relay%22)%20AND%20(%22zero-knowledge%22%20OR%20%22zero%20knowledge%22%20OR%20%22zero-knowledge%20proof%22%20OR%20%22zero%20knowledge%20proof%22%20OR%20ZKP%20OR%20NIZK%20OR%20%22zk-SNARK%22%20OR%20zkSNARK%20OR%20%22zk-STARK%22%20OR%20zkSTARK%20OR%20SNARK))%20OR%20(%22ZK%20bridge%22%20OR%20%22zk%20bridge%22%20OR%20%22zero-knowledge%20bridge%22%20OR%20%22zero%20knowledge%20bridge%22%20OR%20%22ZKP%20bridge%22%20OR%20%22succinct%20light%20client%22%20OR%20%22zk%20light%20client%22%20OR%20%22ZK%20light%20client%22%20OR%20%22zero-knowledge%20light%20client%22%20OR%20%22cross-chain%20SNARK%22%20OR%20%22cross%20chain%20SNARK%22%20OR%20%22cross-chain%20proof%22%20OR%20%22cross%20chain%20proof%22%20OR%20%22validity%20bridge%22%20OR%20%22proof-carrying%20data%22%20OR%20%22proof%20carrying%20data%22%20OR%20%22chain%20relay%20SNARK%22%20OR%20%22cross-chain%20ZKP%22%20OR%20%22cross%20chain%20ZKP%22%20OR%20%22cross-chain%20zero-knowledge%22%20OR%20%22cross-chain%20zero%20knowledge%22%20OR%20%22zero-knowledge%20interoperability%22%20OR%20%22zero%20knowledge%20interoperability%22%20OR%20%22atomic%20swap%20zero%20knowledge%22%20OR%20%22zero-knowledge%20atomic%20swap%22%20OR%20%22ZK%20atomic%20swap%22)&highlight=true&returnType=SEARCH&pageNumber=1&returnFacets=ALL>)

The full query. Round 1: 124 records. Round 2: 154 records.

### ACM Digital Library

**Search:** [ACM Digital Library search](<https://dl.acm.org/action/doSearch?AllField=%28%28%22blockchain%20interoperability%22%20OR%20%22cross-chain%22%20OR%20%22cross%20chain%22%20OR%20%22cross-ledger%22%20OR%20%22cross%20ledger%22%20OR%20interchain%20OR%20%22inter-chain%22%20OR%20%22blockchain%20bridge%22%20OR%20%22cross-chain%20bridge%22%20OR%20%22cross-chain%20protocol%22%20OR%20%22interoperability%20protocol%22%20OR%20%22cross-chain%20communication%22%20OR%20%22cross-chain%20transaction%22%20OR%20%22cross-chain%20transfer%22%20OR%20%22chain%20relay%22%20OR%20%22blockchain%20relay%22%29%20AND%20%28%22zero-knowledge%22%20OR%20%22zero%20knowledge%22%20OR%20%22zero-knowledge%20proof%22%20OR%20%22zero%20knowledge%20proof%22%20OR%20ZKP%20OR%20NIZK%20OR%20%22zk-SNARK%22%20OR%20zkSNARK%20OR%20%22zk-STARK%22%20OR%20zkSTARK%20OR%20SNARK%29%29%20OR%20%28%22ZK%20bridge%22%20OR%20%22zk%20bridge%22%20OR%20%22zero-knowledge%20bridge%22%20OR%20%22zero%20knowledge%20bridge%22%20OR%20%22ZKP%20bridge%22%20OR%20%22succinct%20light%20client%22%20OR%20%22zk%20light%20client%22%20OR%20%22ZK%20light%20client%22%20OR%20%22zero-knowledge%20light%20client%22%20OR%20%22cross-chain%20SNARK%22%20OR%20%22cross%20chain%20SNARK%22%20OR%20%22cross-chain%20proof%22%20OR%20%22cross%20chain%20proof%22%20OR%20%22validity%20bridge%22%20OR%20%22proof-carrying%20data%22%20OR%20%22proof%20carrying%20data%22%20OR%20%22chain%20relay%20SNARK%22%20OR%20%22cross-chain%20ZKP%22%20OR%20%22cross%20chain%20ZKP%22%20OR%20%22cross-chain%20zero-knowledge%22%20OR%20%22cross-chain%20zero%20knowledge%22%20OR%20%22zero-knowledge%20interoperability%22%20OR%20%22zero%20knowledge%20interoperability%22%20OR%20%22atomic%20swap%20zero%20knowledge%22%20OR%20%22zero-knowledge%20atomic%20swap%22%20OR%20%22ZK%20atomic%20swap%22%29>)

The full query, searched in all fields. Round 1: 221 records. Round 2: 277 records.

### Web of Science

**Search:** [Web of Science saved search](<https://www.webofscience.com/wos/alldb/summary/941b46ae-11d2-49c6-9e0c-bebe21b30f77-01cbf6ec5a/relevance/1>)

Round 1: 207 records. Round 2: 263 records.

### Google Scholar

The same query was run separately over five publication-year intervals: 2020–2021, 2022–2023, 2024, 2025, and 2026. In each interval, the first 400 results in relevance order were screened, for 2,000 inspected records per round. The second round considered only records not already considered in the first round. Google Scholar estimated about 168,000 results for the unrestricted query, but it displays at most 1,000 results per query, so the interval searches were used to screen a bounded, relevance-ranked sample. This follows Haddaway et al.'s recommendation to focus on highly ranked Scholar results when using it as a supplementary source for evidence reviews ([PLOS ONE, 2015](https://doi.org/10.1371/journal.pone.0138237)).

**Search:** [Google Scholar search](<https://scholar.google.com/scholar?q=%28%28%22blockchain+interoperability%22+OR+%22cross-chain%22+OR+%22cross+chain%22+OR+%22cross-ledger%22+OR+%22cross+ledger%22+OR+interchain+OR+%22inter-chain%22+OR+%22blockchain+bridge%22+OR+%22cross-chain+bridge%22+OR+%22cross-chain+protocol%22+OR+%22interoperability+protocol%22+OR+%22cross-chain+communication%22+OR+%22cross-chain+transaction%22+OR+%22cross-chain+transfer%22+OR+%22chain+relay%22+OR+%22blockchain+relay%22%29+AND+%28%22zero-knowledge%22+OR+%22zero+knowledge%22+OR+%22zero-knowledge+proof%22+OR+%22zero+knowledge+proof%22+OR+ZKP+OR+NIZK+OR+%22zk-SNARK%22+OR+zkSNARK+OR+%22zk-STARK%22+OR+zkSTARK+OR+SNARK%29%29+OR+%28%22ZK+bridge%22+OR+%22zk+bridge%22+OR+%22zero-knowledge+bridge%22+OR+%22zero+knowledge+bridge%22+OR+%22ZKP+bridge%22+OR+%22succinct+light+client%22+OR+%22zk+light+client%22+OR+%22ZK+light+client%22+OR+%22zero-knowledge+light+client%22+OR+%22cross-chain+SNARK%22+OR+%22cross+chain+SNARK%22+OR+%22cross-chain+proof%22+OR+%22cross+chain+proof%22+OR+%22validity+bridge%22+OR+%22proof-carrying+data%22+OR+%22proof+carrying+data%22+OR+%22chain+relay+SNARK%22+OR+%22cross-chain+ZKP%22+OR+%22cross+chain+ZKP%22+OR+%22cross-chain+zero-knowledge%22+OR+%22cross-chain+zero+knowledge%22+OR+%22zero-knowledge+interoperability%22+OR+%22zero+knowledge+interoperability%22+OR+%22atomic+swap+zero+knowledge%22+OR+%22zero-knowledge+atomic+swap%22+OR+%22ZK+atomic+swap%22%29>) (repeat with each year interval)

## Deployed systems

Deployed systems were identified through two complementary searches. Predefined Google web searches returned 43 candidate approaches. An AI search agent (Claude Opus 5.0, run on 15 August 2026) was prompted with:

> List me blockchain interoperability protocols / solutions that utilize zero knowledge proofs and are in production (All you can find)

The follow-up prompt asked: 

> Find more blockchain interoperability protocols / solutions that utilize zero knowledge proofs and are in production.

 It was repeated until the agent returned only invalid or duplicate results. 
 
 The agent identified 70 candidates, including all 43 found through web search, so the combined set contained 70 distinct candidates. Two authors manually assessed each; 41 were excluded and 29 deployed systems were included in the corpus.

The predefined Google search queries were:

1. Which blockchain interoperability protocols use zero-knowledge proofs and are currently deployed in production?
2. What zero-knowledge blockchain bridges are currently operational on mainnet?
3. Which production-ready cross-chain communication protocols utilize zero-knowledge proofs?
4. What blockchain interoperability solutions use zk-SNARKs or zk-STARKs and have active mainnet deployments?
5. Which trustless cross-chain bridges use zero-knowledge proofs to verify transactions between blockchains?
6. What zero-knowledge light client protocols are currently deployed for blockchain interoperability?
7. Which blockchain bridges use zero-knowledge proofs for cross-chain state verification in production?
8. What decentralized cross-chain messaging protocols use zero-knowledge proofs and are currently operational?
9. Which zero-knowledge interoperability projects have launched their mainnet networks or production services?
10. What blockchain interoperability protocols use zero-knowledge proofs for secure cross-chain asset transfers?
11. Which production blockchain bridges use succinct zero-knowledge proofs instead of trusted intermediaries?
12. What privacy-preserving cross-chain interoperability protocols use zero-knowledge proofs and are deployed on mainnet?
13. Which zero-knowledge rollup interoperability solutions enable communication between different blockchain networks in production?
14. What commercially available or open-source blockchain interoperability platforms use zero-knowledge proofs in their deployed infrastructure?
15. Which blockchain interoperability protocols launched between 2024 and 2026 use zero-knowledge proofs and are currently operational?
