# Artifacts
This repository contain the artifacts for the paper: *Demystifying Harmful Content in Ethereum Transactions*.

**Warning⚠️:** This repository contains *OFFENSIVE* and *EXPLICIT* content, please use it responsibly.

Specifically, this repository includes **harmful content classification criteria**.

- [`./criteria/readme.md`](criteria/readme.md): The detailed criteria for harmful content classification and example cases.
- [`./prompt/readme.md](./prompt/readme.md): Prompt templates for semantically meaningful content extraction.


## Introduction & Findings
Users can store arbitrary content on Ethereum through transactions, however, this freedom introduces the risk of embedding harmful content on blockchain. Due to the immutability and transparency of blockchain, once harmful content is recorded, it cannot be removed and is accessible to everyone, which could cause widespread and lasting negative impacts on the real world. 

We extracted 96,687 text segments, 9,931 files, and 1,198,889 URLs from 2,224,215,240 Ethereum transactions. Through sampling and the open card sorting approach, we randomly sampled 9,148 text segments and 9,528 URLs for examination, and reviewed all 9,931 files, providing a 95% confidence level and a 1% confidence interval.

We identified 638 cases of potentially harmful content, accounting for **3.2%** of all sampled content. These cases is classified into six categories: **Privacy Violation**, **Sexual Content**, **Discrimination**, **On-chain Crime**, **Personal Threat**, and **Child Maltreatment**.


