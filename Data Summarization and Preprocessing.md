### Importing the dataset

```{r}
dataset = read.csv('bodyPerformance.csv')

View(dataset)
summary(dataset)
str(dataset)
```

################# Dealing with the missing values - Outliers

```{r}
is.na(dataset)

```

### to find the total null values in the dataset

```{r}
sum(is.na(dataset))
```

```{r}
print(dataset)
```

### Detect Outlier

```{r}
summary(dataset$age)
```

```{r}
summary(dataset$height_cm)
```

```{r}
summary(dataset$weight_kg)
```

```{r}
summary(dataset$body.fat_.)
```

```{r}
summary(dataset$diastolic)
```

```{r}
summary(dataset$systolic)
```

```{r}
summary(dataset$gripForce)
```

```{r}
summary(dataset$sit.and.bend.forward_cm)
```

```{r}
summary(dataset$sit.ups.counts)
```

```{r}
summary(dataset$broad.jump_cm)
```

### Boxplot:

#### Boxplot of age

```{r}
boxplot.stats(dataset$age)$out

out <- boxplot.stats(dataset$age)$out
out_ind <- which(dataset$age %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$age ,
        ylab= "age",
        main= "Boxplot of age")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))

```

#### Boxplot of height_cm

```{r}
boxplot.stats(dataset$height_cm)$out

out <- boxplot.stats(dataset$height_cm)$out
out_ind <- which(dataset$height_cm %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$height_cm ,
        ylab= "height_cm",
        main= "Boxplot of height_cm")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of weight_kg

```{r}
boxplot.stats(dataset$weight_kg)$out

out <- boxplot.stats(dataset$weight_kg)$out
out_ind <- which(dataset$weight_kg %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$weight_kg ,
        ylab= "weight_kg",
        main= "Boxplot of weight_kg")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of body.fat\_.

```{r}
boxplot.stats(dataset$body.fat_.)$out

out <- boxplot.stats(dataset$body.fat_.)$out
out_ind <- which(dataset$body.fat_. %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$weight_kg ,
        ylab= "body.fat_.",
        main= "Boxplot of body.fat_.")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of diastolic

```{r}
boxplot.stats(dataset$diastolic)$out

out <- boxplot.stats(dataset$diastolic)$out
out_ind <- which(dataset$diastolic %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$diastolic ,
        ylab= "diastolic",
        main= "Boxplot of diastolic")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of systolic

```{r}
boxplot.stats(dataset$systolic)$out

out <- boxplot.stats(dataset$systolic)$out
out_ind <- which(dataset$systolic %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$systolic ,
        ylab= "systolic",
        main= "Boxplot of systolic")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of gripForce

```{r}
boxplot.stats(dataset$gripForce)$out

out <- boxplot.stats(dataset$gripForce)$out
out_ind <- which(dataset$gripForce %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$gripForce ,
        ylab= "gripForce",
        main= "Boxplot of gripForce")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of sit.and.bend.forward_cm

```{r}
boxplot.stats(dataset$sit.and.bend.forward_cm)$out

out <- boxplot.stats(dataset$sit.and.bend.forward_cm)$out
out_ind <- which(dataset$sit.and.bend.forward_cm %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$sit.and.bend.forward_cm ,
        ylab= "sit.and.bend.forward_cm",
        main= "Boxplot of sit.and.bend.forward_cm")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of sit.ups.counts

```{r}
boxplot.stats(dataset$sit.ups.counts)$out

out <- boxplot.stats(dataset$sit.ups.counts)$out
out_ind <- which(dataset$sit.ups.counts %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$sit.ups.counts ,
        ylab= "sit.ups.counts",
        main= "Boxplot of sit.ups.counts")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```

#### boxplot of broad.jump_cm

```{r}
boxplot.stats(dataset$broad.jump_cm)$out

out <- boxplot.stats(dataset$broad.jump_cm)$out
out_ind <- which(dataset$broad.jump_cm %in% c(out))
out_ind

dataset[out_ind, ]

boxplot(dataset$broad.jump_cm ,
        ylab= "sit.ups.counts",
        main= "Boxplot of broad.jump_cm")
mtext(paste("Outliers: ", paste(out, collapse = ", ")))
```
