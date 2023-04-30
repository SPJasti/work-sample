Here is detailed instructions on how to open, import a dataset, perform basic pre-processing, exploring, save and export to a CSV file in R-Studio:

**Step 1: Open R-Studio**
Open R-Studio on your computer. It should be installed on your system, and you can find it in the Start menu or on your desktop.

**Step 2: Load the required packages**
For basic pre-processing and exploring of datasets, you need to load the following packages:

```r
library(readr)
library(dplyr)
```

**Step 3: Set your working directory**
Your working directory is the folder where your R project and data are stored. You can use the `setwd()` function to set your working directory. For example, if your data file is stored in the "Data" folder on your desktop, you can set your working directory as follows:
```r
setwd("~/Desktop/Data")
```

**Step 4: Import the dataset**
To import a dataset in R-Studio, use the `read_csv()` function from the readr package. For example, if your data file is named "data.csv", you can import it as follows:
```r
data <- read_csv("data.csv")
```

**Step 5: Pre-process the dataset**
Now that you have imported your dataset, you can start pre-processing it. For example, you may want to remove any missing values or duplicates from your dataset. Here's an example of how you can remove missing values:
```r
data <- na.omit(data)
```
And here's an example of how you can remove duplicates:
```r
data <- distinct(data)
```

**Step 6: Explore the dataset**
To explore your dataset, you can use the `summary()` function. This will give you a summary of each variable in your dataset, including the mean, median, minimum, and maximum values, as well as the number of missing values.
```r
summary(data)
```
You can also use the `head()` function to view the first few rows of your dataset:
```r
head(data)
```

**Step 7: Save the pre-processed dataset**
To save the pre-processed dataset, use the `write_csv()` function from the readr package. For example, if you want to save your pre-processed dataset as "processed_data.csv", you can use the following code:
```r
write_csv(data, "processed_data.csv")
```

**Step 8: Export the pre-processed dataset**
To export the pre-processed dataset as a CSV file, you can use the `write.csv()` function. For example, if you want to export your pre-processed dataset as "processed_data.csv", you can use the following code:
```r
write.csv(data, "processed_data.csv", row.names = FALSE)
```

You have now learned how to open, import a dataset, perform basic pre-processing, explore, save and export to a CSV file in R-Studio. 
You have now gained new skills and you can be more useful to Navitas.
