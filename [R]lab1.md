#first
v <- rnorm(100)
v[10]
v[10:20]
v[20:(20+10)]
v[v>0]
#second
y <- data.frame(a = rnorm(100), b= 1:100, cc = sample(letters, 100, replace = TRUE))
tail(y, n=10)
y[10:20, 1:3]
y[10, "b"]
y[,"cc"]
#third
z<-c(1, 2, 3, NA, 4, NA, 5, NA)
z[!is.na(z)]
mean(z[!is.na(z)])
mean(z)


