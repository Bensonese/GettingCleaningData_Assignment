setwd("C:/UCI HAR Dataset")

test_who <- read.table("test/subject_test.txt")
test_values <- read.table("test/X_test.txt")
test_what <- read.table("test/y_test.txt")

train_who <- read.table("train/subject_train.txt")
train_values <- read.table("train/X_train.txt")
train_what <- read.table("train/y_train.txt")

test <- cbind(test_values, test_who, test_what)
train <- cbind(train_values, train_who, train_what)
all_data <- rbind(test, train)

list <- read.table("features.txt")
list <- list[,2]
index <- grep("(mean\\(\\))|std", list)
x <- all_data[,c(index, 562:563)]

x$V1.2 <- ifelse(x$V1.2 == 1, "Walking", 
          ifelse(x$V1.2 == 2, "Walk Upstairs",
          ifelse(x$V1.2 == 3, "Walking Downstairs",
          ifelse(x$V1.2 == 4, "Sitting",
          ifelse(x$V1.2 == 5, "Standing", "Laying")))))

list <- as.character(list)
variables <- sub("\\(\\)", "", list[index])
variables <- gsub("-", "_", variables)
variables <- sub("^t", "Time_", variables)
variables <- sub("^f", "Freq_", variables)
colnames(x) <- c(variables, "Subject", "Activity")

a <- x[,1:66]
b <- x[,67:68]
x <- cbind(b,a)

library(dplyr)
tidy <- x %>% group_by(Subject, Activity) %>% summarise_each(funs(mean))
write.table(tidy, file = "assignment_tidy_data.txt", row.names = FALSE)
