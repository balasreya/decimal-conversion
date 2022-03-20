# decimal-conversion
f#binary to decimal conversion
x <- scan()
c <- vector()
while(x>0) {
  r=x%%10
  c <- append(c,r)
  x=x%/%10
}
c
c <- rev(c)
c
k=0
n <- length(c)
for(i in n:1) {
  k=k+c[i]*(2^(n-i))
}
k
