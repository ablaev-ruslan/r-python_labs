#1
add2 <- function(x,y){
return(x+y)
}
#2
above <- function(x,n){
return(x[x > n])
}
#3
my_ifelse<- function(x, exp, n){
  if (exp == '=='){
    return(x[x == n])
  }
  
  else if (exp == '>'){
    return(x[x > n])
  }
  
  else if (exp == '<'){
    return(x[x < n])
  }
  
  else if (exp == '>='){
    return(x[x >= n])
  }
  
  else if (exp == '<='){
    return(x[x <= n])
  }
  
  else{
    return(x)
  }
}

#4
columnmean <- function(x,removeNA=TRUE){
return(colMeans(x,na.rm=removeNA))
}