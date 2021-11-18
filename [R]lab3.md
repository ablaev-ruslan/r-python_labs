df <- read.csv(file="hw1_data.csv")
#1
colnames(df)
#2
read.csv(file="hw1_data.csv",nrows=6)
#3
nrow(df)
#4
tail(df,10)
#5
sum(is.na(df$Ozone))
#6
mean(df$Ozone, na.rm = TRUE)
#7
subset(df, Ozone > 31 & Temp > 90)
mean(subset(df, Ozone > 31 & Temp > 90)$Solar.R)
#8
mean(subset(df, Month == 6)$Temp)
#9
max(subset(df, Month == 5 & !is.na(Ozone))$Ozone)