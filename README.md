# Fibonacci-number
# python
# Find the number of F[n] using Fibonacci numbers by entering n n을 입력해서 피보나치의 수를 이용해서 F[n]의 수 찾기
def solution(n):
    F= [0,1,1]
    for i in range(3,n+1):
        F.append((F[i-1]+F[i-2])%1234567)
    return F[-1]
a=solution(3)
print(a)
#result--> 2
