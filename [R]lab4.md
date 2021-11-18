setwd("C:/Users/RUSLAN~1/Desktop/")
source("C:/Users/RUSLAN~1/Desktop/pmean.R")
#1
pmean("specdata", "sulfate", 001:10)
pmean("specdata", "sulfate", 55)
pmean("specdata", "nitrate")

#2
complete("specdata", 1)
complete("specdata", c(2, 4, 8, 10, 12))
complete("specdata", 50:60)

#3
cr <- corr("specdata", 150)
head(cr)
summary(cr)

cr <- corr("specdata", 400)
head(cr)
summary(cr)

cr <- corr("specdata", 5000)
head(cr)
summary(cr)
length(cr)