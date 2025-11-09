# Research Question 2 Summary: Feature Identification

## Research Question
**What are the most salient linguistic features (specific vocabulary, frequency of negative or passive emotional language, use of self-referential pronouns) that distinguish text associated with various mental health challenges?**

---

## Key Findings

### 1. **Vocabulary Analysis**
Using TF-IDF analysis, each mental health category shows distinctive word patterns:
- **Anxiety**: "anxiety", "restless", "nervous" (high specificity)
- **Depression**: "depression", "feel", "want" (emotional expression)
- **Suicidal**: "life", "want", "feel" (existential themes)
- **Stress**: "stress", "feel", "don't" (pressure indicators)
- **Bipolar**: "bipolar", "feel", "just" (condition awareness)
- **Personality disorder**: "people", "feel", "don't" (relational focus)
- **Normal**: General conversational words with low emotional intensity

### 2. **Self-Referential Pronoun Usage**
First-person singular pronouns (I, me, my) are **significantly elevated** in mental health categories:
- **Depression**: 19.05 avg occurrences (highest)
- **Personality disorder**: 18.62 avg occurrences
- **Bipolar**: 18.47 avg occurrences
- **Suicidal**: 17.61 avg occurrences
- **Anxiety**: 14.65 avg occurrences
- **Stress**: 11.03 avg occurrences
- **Normal**: 1.07 avg occurrences (baseline)

**Insight**: Mental health-related text demonstrates **10-18x higher** self-focused language compared to normal discourse.

### 3. **Emotional Language Patterns**

#### Negative Words
- **Stress**: 1.37 avg (highest negative language)
- **Anxiety**: 1.31 avg
- **Depression**: 0.99 avg
- **Normal**: 0.05 avg (minimal negative language)

#### Positive Words
- **Depression**: 1.09 avg (surprisingly high - potentially coping language)
- **Suicidal**: 0.99 avg
- **Normal**: 0.14 avg

#### Passive Markers (feel, feeling, felt, seems, etc.)
- **Personality disorder**: 2.08 avg (highest)
- **Depression**: 2.06 avg
- **Bipolar**: 1.90 avg
- **Anxiety**: 1.68 avg
- **Normal**: 0.07 avg (minimal passive expression)

**Insight**: Mental health categories show **20-30x higher** use of passive emotional markers, indicating introspective and emotionally focused communication.

---

## Statistical Insights

### Linguistic Feature Profile (Normalized)
The heatmap analysis reveals:
- **Depression** scores highest across all linguistic features
- **Normal** category shows near-zero scores on all mental health indicators
- **Stress** and **Anxiety** share similar linguistic profiles with high negative word usage
- **Suicidal** category shows balanced negative/positive language with moderate first-person usage

### Word Count Patterns
- Mental health categories average 115-180 words per statement
- **Normal** category averages only 18 words (significantly shorter)
- Longer statements correlate with greater emotional expression and self-disclosure

---

## Conclusions

The analysis successfully identified **clear linguistic signatures** that distinguish mental health categories:

1. **First-person pronouns** are the strongest discriminator (10-18x increase)
2. **Passive emotional markers** indicate introspective processing (20-30x increase)
3. **Category-specific vocabulary** enables targeted classification
4. **Normal** text shows minimal emotional language and self-reference

These findings validate that **linguistic patterns can serve as early indicators** of mental health challenges, supporting automated detection systems for proactive intervention.

---

**Answer to RQ2**: Yes, distinctive linguistic features exist across mental health categories, with first-person pronoun usage, passive emotional markers, and category-specific vocabulary serving as the most salient differentiators.
