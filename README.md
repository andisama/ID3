# Rule-based Algorithm ID3

Generate a Rule-Based Decision Tree with ID3 Algorithm.

As part of the Doctor of Computer Science Program assignments at Binus University.

Environment
============
- Operating System: Windows 11, 64 bits
- Programming Environment: Anaconda Navigator 2.4.0
- Programming Language: Python 3.9.12
- Python libraries: scikit-learn, pandas, matplotlib

Dataset
========
World Economic Forum, 2018, "Appendix B, Drivers of Production (continued), Table B8: Nascent Countries“, Readiness for the future of Production report 2018, page 52-53, https://www.weforum.org/reports/readiness-for-the-future-of-production-report-2018

The Process
===========
The Drivers of Production scores are converted into quartiles (Nascent Q1-Nascent Q4), creating four distributions within nascent countries (classes) with six components of the driver of production (features). Thus, ensuring a balanced number of samples per class.


The DecisionTreeClassifier algorithm within scikit-learn automatically drops the last 2 of 6 columns in the provided features.
criterion=‘entropy’ is set in the DecisionTreeClassifier function that indicates using the ID3 algorithm to calculate the homogeneity of the samples). Only the first 4 columns remain on the Trained DecisionTreeClassifier.

An additional 1 random new data is provided for the six features to test the trained model. The class is predicted to be Q3 for these new features.

