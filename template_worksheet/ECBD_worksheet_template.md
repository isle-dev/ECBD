# Evidence-Centered Benchmark Design: Worksheet Template
Evidence-Centered Benchmark Design (ECBD) is a framework that formalizes the benchmark design process. It requires first specifying the **intended use** of the benchmark (including specifying the objects of evaluation). The process is then broken down into five modules:
- **Capability module**: capabilities that the benchmark aims to measure.
- **Content module**: pool of test items that draw out responses from the objects.
- **Adaptation module**: adapting or instructing the objects to complete the tasks.
- **Assembly module**: selecting from the pool of test items to build the set used for evaluation.
- **Evidence module**: extracting and accumulating evidence about the capabilities of interest from responses produced by the objects. 

This worksheet provides guidance on how to create a new benchmark or analyze an existing benchmark following ECBD. It can be completed from different perspectives: as the creator of a new benchmark, as the custodian or the user of an existing benchmark, or as a third-party analyzing benchmarks, etc. Each module contains three questions:
- **Describe**: What design decisions did the benchmark creators make for this module?
- **Justify**: Why did the benchmark creators make these decisions? This involves forming a hypothesis that the decisions allow the module to accomplish its role in the process of gathering necessary capability evidence.
- **Support**: What validity evidence do the benchmark creators have to support the above hypothesis? In other words, what shows that the module indeed accomplishes its role?

This worksheet is not a checklist, and it is not required to answer each question perfectly. These questions are meant to encourage reflection and validation of benchmark design decisions, as well as to guide benchmark documentation.

## Benchmark Name and Reference(s)
The references are the source of information used to complete this worksheet. For example, a third-party analyzing an existing benchmark may choose to use the academic publication introducing said benchmark as their source of information. Other sources of information could be blog posts, official websites, or code repositories accompanying the benchmark. 
```
ANSWER HERE
```

## Who is filing the worksheet?
From what perspective is this worksheet completed? In other words, what is the relation between the person(s) completing this worksheet and the benchmark that is the focus of this worksheet? 

```
ANSWER HERE
```

## Intended Use
**Q1 - Who/What are the intended objects of evaluation?** Elaboration on the objects of evaluation (e.g., their assumed capabilities, demographic information for human objects of evaluation, etc.) helps us better understand whether the benchmark is suitable for all intended objects of evaluation.

```
ANSWER HERE
```

**Q2 - What is the intended use of the benchmark? Who are the intended users of the benchmark?** Benchmark results aim to provide insights about the objects of evaluation: how are users meant to use these insights? 

```
ANSWER HERE
```

## Capability Module
The capability module specifies the capabilities that the benchmark aims to evaluate. The term “capability” refers to a construct (e.g., quality criteria, skill, etc.) that the objects of evaluation are thought to exhibit or possess. Capabilities often cannot be directly observed or directly measured, thus requiring the benchmark to indirectly measure them by gathering necessary evidence about said capabilities. 

**Q3 - DESCRIBE: i) What are the capabilities of interest? ii) How is each one defined, and under what context is each one defined?**

```
ANSWER HERE
```

Additional recommended questions to consider so to further clarify and contextualize the definitions (in benchmark analysis: as presented by the benchmark):
- How does the definition used by the benchmark differ from other existing definitions of this capability?
    
```
ANSWER HERE
```
- How does this capability differ from other similarly defined capabilities?
```
ANSWER HERE
```

**Q4 - JUSTIFY: How are the capabilities of interest connected to the intended use of the benchmark (specified in Q2)? Are the capabilities theoretically attainable by the objects to be evaluated?** Explain the interest in measuring the capabilities in Q3 and question whether it may be impossible for the objects of evaluation to have said capabilities.

```
ANSWER HERE
```

**Q5 - SUPPORT: What validity evidence do the benchmark creators offer to support the choice and definition of capabilities of interest?**

```
ANSWER HERE
```

## Content Module
The content module specifies test items that the benchmark could require objects of evaluation to perform or to respond to. The test items should elicit evidence about some capability of interest, so that said capability evidence can be later extracted from the responses and aggregated to produce a measurement of said capability.

**Q6 - DESCRIBE: {i) Characterize the test items**. Most often, NLP evaluation relies on input data, so this step could involve describing the data that is available to the benchmark to use, how the data is obtained, etc. **ii)  Which capabilities of interest does each test item aim to capture?** Each item can aim to capture one or several capabilities amongst those listed in Q3.

```
ANSWER HERE
```

**Q7 - JUSTIFY: How does each test item elicit evidence about its target capabilities? Justify via the characteristics of the test items (Q6).**

```
ANSWER HERE
```

**Q8 - SUPPORT: What evidence do the benchmark creators offer to support content validity of the test items?** In other words, we question whether the test items captures capabilities of interest. Content validity is often based on analysis by external experts or benchmark users.

```
ANSWER HERE
```

## Adaptation Module
When evaluating humans, the benchmark might instruct them to perform a task by providing instructions, training exercises, demonstrations, etc. When evaluating models/systems, there are also myriad methods that i) modify the models/systems (e.g., fine-tuning), or ii) format or add onto the input (e.g., adding examples in few-shot prompting). These adaptation methods should be chosen carefully so as to not confound evaluation results.

**Q9 - DESCRIBE: Given an input, how are the objects of evaluation adapted or instructed to provide the output?**

```
ANSWER HERE
```

**Q10 - JUSTIFY: Elaborate on the suitability of the adaptation methods for all intended objects of evaluation.**

```
ANSWER HERE
```

**Q11 - SUPPORT: What validity evidence do benchmark designers offer that supports the choice of the adaptation methods?**

```
ANSWER HERE
```

## Assembly Module
Test items specified by the content module are what the benchmark could use. The assembly module concerns what items from that pool will actually be used by the benchmark for evaluation, and whether this set allows the benchmark to gather sufficient evidence.

**Q12 - DESCRIBE: How many test items are chosen to assemble the subset used for evaluation? What factors inform this selection?**

```
ANSWER HERE
```

**Q13 - JUSTIFY: How does the described assembly method ensure that the produced subset elicits sufficient evidence for all capabilities of interest?**

```
ANSWER HERE
```

**Q14 - SUPPORT: What validity evidence do the benchmark creators offer to support the choice of assembly methods?**

```
ANSWER HERE
```

## Evidence Module
### Evidence Extraction Component
In response to each presented test item, objects of evaluation produce observable behaviors (referred to as “responses”) which are captured by the benchmark. From these responses, the benchmark extracts evidence about capabilities of interest that said test item targets (referred to as ``salient evidence''). 

**Q15 - DESCRIBE: For each test item, i) What responses are captured and used for evidence extraction?** When evaluating humans, many types of responses can be captured: selection in multiple-choice questions, long-form answers, response time, etc. Similarly, the benchmark can use the generated text (decoded in a certain way), token probabilities, running time, etc. **ii) How is evidence extracted and represented?**

```
ANSWER HERE
```

**Q16 - JUSTIFY: How does the extracted evidence capture the capabilities of interest?**

```
ANSWER HERE
```

**Q17 - SUPPORT: What validity evidence do the benchmark creators offer to support the choice of evidence extraction method?**

```
ANSWER HERE
```

### Evidence Accumulation Component

**Q18 - DESCRIBE: How is the evidence accumulated to draw insights about the objects of evaluation in terms of capabilities of interest?**

```
ANSWER HERE
```

**Q19 - JUSTIFY: How does the method of accumulating evidence capture capabilities of interest?**

```
ANSWER HERE
```

**Q20 - SUPPORT: What validity evidence do the benchmark creators offer to support the choice of evidence accumulation method?**

```
ANSWER HERE
```