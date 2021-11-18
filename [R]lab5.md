#1
mat<-matrix(rnorm(50),nrow=10)
#2
apply(mat,2,max)
#3
apply(mat,2,mean)
#4
apply(mat,1,min)
#5
apply(mat,2,sort)
#6
my_func<- function(x){return(x[x>0])}
apply(mat,2, my_func)
#7
my_ifelse<- function(x){
  if (length(x[x>2])==0){
    return(FALSE)
  }
  else{
    return(TRUE)
  }
}

apply(mat,2, my_ifelse)

#8
list1<-list(observationA=c(1:5, 7:3),observationB=matrix(1:6, nrow=2))
lapply(list1,sum)
#9
lapply(list1,min)
lapply(list1,max)
lapply(list1,range)

sapply(list1,min)
sapply(list1,max)
sapply(list1,range)

#10
tapply(InsectSprays$count, InsectSprays$spray, mean)