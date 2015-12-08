### About

Low-memory Multinomial Logistic Regression with Support for Text Classification

Maxent is an R package with tools for low-memory multinomial logistic regression,
also known as maximum entropy. The focus of this maximum entropy classifier is to
minimize memory consumption on very large datasets, particularly sparse document-term
matrices represented by the tm package. The classifier is based on an efficient C++
implementation written by Dr. Yoshimasa Tsuruoka.

### Installation

Maxent requires R 2.13+, which can be downloaded at http://www.r-project.org/.
To build and install sentiment, run the following commands while in the root folder:
```
R CMD REMOVE maxent
R CMD BUILD maxent
R CMD INSTALL maxent_X.X.X.tar.gz
```
(where the X's should be replaced with the version number -- e.g. 1.3.2)

### Source code

To modify the R code, go to the maxent folder, and modify files within the R directory.
After making changes, ensure the package passes R CHECK using the following command:
```
R CMD CHECK maxent
```
