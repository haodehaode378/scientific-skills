---
name: paper-summary
description: Summarize academic papers from arXiv links or PDF files and extract key research information such as research problem, methodology, contributions, results, and limitations.
---

# paper-summary

paper-summary is a research assistant skill designed to help researchers quickly understand academic papers.

Instead of reading the entire paper, this skill extracts the most important information and presents it in a structured summary format. It is particularly useful during literature review and early-stage research when researchers need to evaluate many papers efficiently.

## Motivation

Researchers often need to read a large number of academic papers in order to stay up to date with the latest developments in their field.

However, reading every paper in detail is time-consuming. In most cases, researchers only need to quickly determine:

- what problem the paper is addressing
- what method or approach it proposes
- what contributions it makes
- whether the results are significant
- whether the work is relevant to their research

This skill accelerates the literature review process by automatically extracting and organizing the most important information from academic papers.

## Supported Inputs

This skill supports the following input formats:

- arXiv paper links  
- arXiv IDs  
- local PDF files  

Examples:

```
summary paper https://arxiv.org/pdf/2304.13712
```

```
summary paper arxiv:2304.13712
```

```
summary paper ./paper.pdf
```

## Query Workflow

1. Detect the input source (arXiv link, arXiv ID, or local PDF file).
2. Retrieve the paper content.
3. Identify important sections of the paper.
4. Extract key research information.
5. Generate a structured summary.

## Output Structure

The generated summary should contain the following sections:

### Title

The title of the academic paper.

### Research Problem

A short explanation of the research question or problem the paper aims to solve.

### Methodology

A description of the method, model, or approach used in the research.

### Key Contributions

The main innovations or contributions proposed by the authors.

### Experimental Results

Important experimental findings or evaluation results reported in the paper.

### Limitations

Known weaknesses, assumptions, or limitations of the proposed method.

### Future Work

Possible research directions mentioned by the authors or implied by the work.

## Example Output

Title:  
Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond

Research Problem:  
The paper studies how large language models such as ChatGPT can be applied in real-world scenarios and reviews the current ecosystem of LLM-based applications.

Methodology:  
The authors conduct a systematic survey of recent research on large language models, analyzing their architectures, training strategies, and practical applications.

Key Contributions:  
1. Overview of the large language model research ecosystem  
2. Analysis of practical applications of ChatGPT  
3. Comparison of different LLM architectures and capabilities  

Experimental Results:  
The survey reports strong performance of LLMs across various NLP tasks such as question answering, text generation, summarization, and code generation.

Limitations:  
High computational cost, potential hallucination issues, and concerns related to reliability and alignment.

Future Work:  
Improving model alignment, reducing computational cost, and developing more reliable large language model systems.