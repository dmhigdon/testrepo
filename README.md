# testrepo
testrepo for MSDS 6306 Unit 5
This is the BLT submission for Unit 5. It will contain my data science profile and the Rmarkdown file from the previous week.


Rmarkdown file:
--- title: "Week 4 Lecture Assignment" author: "Daniel Higdon (MSDS 6306 - 404)" date: "1/24/2017" output: html_document: keep_md: true --- ```{r setup, include=FALSE} knitr::opts_chunk$set(echo = TRUE) ``` ## R Markdown - This my Week 4 Lecture Assignment Rmarkdown file Use summary() function on data set and interpret the results: ```{r stackloss summary} summary(stackloss) ``` The summary function provides the five number summary as well as the mean for four variables: * Air.Flow * Water.Temp * Acid.Conc. * stack.loss Use the "str" function on the data set and interpret the results: ```{r stackloss str} str(stackloss) ``` The str() function tells me that stackloss is a dataframe and has 21 observations of four variables. Additionally, all of the variables are numeric. ## Scatterplot of stack.loss vs. Air.Flow Note: I set echo=TRUE so that both the code chunk and the plot would be shown: ```{r stackloss plot, echo=TRUE} plot(stackloss$stack.loss, stackloss$Air.Flow, main="Stackloss Scatterplot", xlab="stack.loss",ylab="Air.Flow") ``` The stack.loss and Air.flow data are positively correlated. While there are some outliers, the correlation generally holds.
