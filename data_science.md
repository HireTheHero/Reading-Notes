# Data Science
## [Nijman et al., 2021](https://pubmed.ncbi.nlm.nih.gov/34798287/)
### Takeaways
- In clinical diagnosis / prognosis prediction model studies, nulls are majorly treated as follows;
    - Insufficient information in literature
    - Methodologies
        - CCA (complete-case-analysis): Remove all samples which have nulls in any of the variables
            - Lessen # of samples
        - Single (mostly mean) imputation
        - Missing value indicator
            - Affect clinician's decision-making, which affects predictive power of the model
                - "They say missing value is important, so let's fill it"
            - Reasoning behind missing must be monitored
- Should be treated with;
    - Proper way of disclosure
    - Consideration of available approaches, such as;
        - Multiple imputation (using Rubin's rule)
        - Methodologies which can directly deal with null, such as ;
            - trees with surrogate splits, which use another variable for splitting samples with null values
            - sparsity-aware splitting, pattern-mixture model

### Questions & Comments
- Other than clinical settings, approaces to nulls should be carefully designed when it could be potentially a bias
    - e.g. Questions in questionnaire which is sensitive for answerer
- Also important if the model details will be given to "those who generate the data"
- What happens if likelihood in multiple imputation is not high "enough"?

### Notes
- [refernce 21 for pattern submodel](https://academic.oup.com/biostatistics/article/21/2/236/5092384)

## [Alayrac et al., 2022](https://www.deepmind.com/blog/tackling-multiple-tasks-with-a-single-visual-language-model)
### Where am I?
- 2.1
### Takeaways
#### Related Works
- Hoffmann et al. (2022)
    - shows # of tokens scale with model size, which explains large-model-better trend
    - Flamingo (80B) is built upon Chinchilla (70B)
- Multiple lines of works have been done on Multimodal BERT-like models but Flamingo is different in that fine-tuning is not needed
- Contrastive dual encoder is strong in small samples but applicable type of tasks is limited, and Flamingo can learn from even smaller samples (significant improvement with 4 samples)
- Autoregressive generative multimodal model is most similar to this work
    - Usage of frozen language model, mapping between vision encoder, cross-attention layers across language model layers
    - Still differentiated in its capability in small data and its flexibility
- In this work, multimodal task-agnostic web scraped data is used for pretraining
- Few-shot learning including "in-context" learning (e.g. in sequence #1 learn basic math, in #2 learn typo and correct spelling, ...) is studied and recently applied to multimodal learning, and this work is first application for video learning
### Questions & Comments
### Notes


## template
### Where am I?
### Takeaways
### Questions & Comments
### Notes
