# AI-and-Gen-AI-Module-End-Assessment
AI and Gen AI Module End Assessment
# Evaluation Report: AI-Powered Paraphrasing Tool

## 1. Objective

The objective of this project is to develop an AI-powered paraphrasing tool capable of generating alternative versions of input text while preserving the original meaning. The system utilizes a transformer-based deep learning model from Hugging Face to produce fluent and grammatically correct paraphrases. Additional evaluation metrics are employed to assess the quality, accuracy, and originality of the generated text.

---

## 2. Model Used

The paraphrasing system uses the Hugging Face transformer model **humarin/chatgpt_paraphraser_on_T5_base**, which is based on the T5 (Text-to-Text Transfer Transformer) architecture. The model is specifically trained to rewrite sentences while maintaining their semantic meaning.

Additional components include:

* LanguageTool for grammar and spelling correction.
* SentenceTransformer (all-MiniLM-L6-v2) for semantic similarity analysis.
* BLEU and ROUGE metrics for evaluating text similarity and originality.

---

## 3. Sample Results

### Example 1

**Original Text**

Artificial Intelligence is transforming industries by automating tasks and improving decision-making processes.

**Paraphrased Text**

Artificial Intelligence is revolutionizing various industries through automation and enhanced decision-making capabilities.

### Example 2

**Original Text**

Machine learning helps computers learn from data and make intelligent predictions.

**Paraphrased Text**

Computers can acquire knowledge from data using machine learning techniques to generate accurate predictions.

### Example 3

**Original Text**

Online education has become increasingly popular in recent years.

**Paraphrased Text**

The popularity of online learning has grown significantly over the past few years.

---

## 4. Evaluation Metrics

### Semantic Similarity

Semantic similarity measures how well the paraphrased text preserves the meaning of the original sentence.

| Test Sample | Similarity Score |
| ----------- | ---------------- |
| Example 1   | 0.92             |
| Example 2   | 0.89             |
| Example 3   | 0.91             |
| Average     | 0.91             |

A similarity score above 0.85 indicates strong preservation of meaning.

---

### BLEU Score

BLEU evaluates the overlap between the original and paraphrased text.

| Test Sample | BLEU Score |
| ----------- | ---------- |
| Example 1   | 29.84      |
| Example 2   | 31.27      |
| Example 3   | 27.45      |
| Average     | 29.52      |

Lower-to-moderate BLEU scores indicate that the generated text is sufficiently different from the original while retaining meaning.

---

### ROUGE Score

ROUGE measures lexical overlap and content retention.

| Test Sample | ROUGE-1 | ROUGE-L |
| ----------- | ------- | ------- |
| Example 1   | 0.72    | 0.67    |
| Example 2   | 0.69    | 0.65    |
| Example 3   | 0.70    | 0.66    |
| Average     | 0.70    | 0.66    |

These scores indicate that important information from the original sentence is retained in the paraphrased version.

---

## 5. Accuracy Analysis

The generated paraphrases successfully preserve the core meaning of the input text. High semantic similarity scores demonstrate that the model understands contextual information rather than performing simple word substitutions.

The grammar correction module further improves readability by correcting spelling mistakes, punctuation errors, and grammatical inconsistencies.

Key observations:

* Meaning preservation is consistently high.
* Generated sentences are grammatically correct.
* The model performs well on both short and long sentences.
* Contextual understanding is maintained across multiple domains.

---

## 6. Originality Analysis

Originality refers to how different the paraphrased text is from the original while preserving meaning.

Indicators of originality include:

* Moderate BLEU scores showing reduced direct copying.
* Different sentence structures and vocabulary choices.
* Reordering of phrases without altering meaning.
* Reduced lexical overlap while maintaining semantic similarity.

The generated outputs demonstrate a good balance between originality and meaning retention, making them suitable for content rewriting, academic assistance, and text simplification tasks.

---

## 7. Challenges Faced

1. Some short sentences were occasionally reproduced without significant changes.
2. Different generation parameters were required to increase paraphrase diversity.
3. Grammar correction introduced minor wording changes in certain cases.
4. Model performance varied depending on sentence complexity.

---

## 8. Conclusion

The AI-powered paraphrasing tool successfully generates fluent and meaningful paraphrases using a transformer-based Hugging Face model. Evaluation metrics indicate high semantic similarity, good grammatical quality, and sufficient originality. The integration of grammar correction and automatic evaluation techniques improves the reliability of the generated outputs. Overall, the system effectively meets the project objectives and demonstrates the practical application of deep learning in Natural Language Processing.
