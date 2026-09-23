# Pakistani-student-focused-study-on-social-media-s-effect-on-concentration-and-academic-performance.
# Social Media Usage & Emotional Well-Being Analysis
### Methodology groundwork for a Pakistani student-focused study

An end-to-end data science pipeline exploring the relationship between social
media usage patterns and emotional well-being, built as preparation for a
Pakistan-specific research project on how social media affects students'
concentration, patience, and academic performance.

## 🎯 Motivation
Social media's impact on students in Pakistan — particularly on focus, patience,
and deep-work ability — is an under-researched area locally. This project builds
and validates a complete analysis pipeline (cleaning → EDA → statistical testing
→ clustering → classification) on an available social media/emotion dataset,
as a methodology dry-run ahead of applying the same pipeline to primary data
collected from Pakistani students.

## 🎯 Research Questions
1. How does daily usage time vary across platforms and demographics?
2. Is higher daily usage time associated with a particular dominant emotion (e.g., anxiety, boredom)?
3. Do engagement behaviors (posting, likes/comments received, messaging) differ by platform?
4. Are there distinct "usage profiles" among users (via clustering) that map onto different emotional states?
5. Which variables correlate most strongly with usage time and emotional state?

## 🛠️ Methodology
- **Data Cleaning:** Fixed column-shifted/malformed rows, removed synthetic-data
  artifacts, validated categorical fields against known label sets
- **Automated EDA:** ydata-profiling, Skimpy, Missingno for distribution and
  missing-data analysis
- **Visualization:** Matplotlib, Seaborn, Plotly — distributions, boxplots,
  cross-tabs, correlation heatmaps
- **Statistical Testing:** Kruskal-Wallis test (usage time vs. emotion),
  Chi-square test (platform vs. emotion), with effect sizes (epsilon-squared,
  Cramér's V)
- **Clustering:** StandardScaler + PCA + KMeans (optimal k via silhouette score)
  to identify distinct user usage profiles
- **Classification:** Logistic Regression, Decision Tree, Random Forest, and
  Gradient Boosting compared on accuracy and macro-F1, validated against a
  dummy baseline and checked for overfitting across train/val/test splits

## 📊 Tech Stack
Python · Pandas · NumPy · Scikit-learn · Seaborn · Plotly · SciPy · Statsmodels ·
Pingouin · ydata-profiling · Missingno · Skimpy

## 📈 Key Findings
*(fill in with your actual output numbers)*
- Sample size, demographics, and platform distribution
- Usage time distribution and skew
- Statistical significance of usage–emotion and platform–emotion associations
- Number and characteristics of usage clusters identified
- Best-performing classification model and its test-set accuracy/F1

## ⚠️ Limitations
- This dataset is **not Pakistan-specific** and does not measure the
  cognitive/behavioral constructs (concentration, patience, deep work) central
  to the actual research aim — it served as a pipeline-validation exercise
- Dataset shows evidence of synthetic/AI generation — findings here are for
  methodology practice, not generalizable conclusions
- Cross-sectional, non-experimental data — no causal claims
- Dominant emotion label is self-reported/generated with no validated
  measurement instrument

## 🔜 Next Steps
- Apply this same pipeline to primary survey data collected from Pakistani
  students, measuring concentration, patience, and academic performance
  alongside social media usage

## 🚀 Setup
\`\`\`bash
pip install -r requirements.txt
\`\`\`
