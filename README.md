# Assign2
1.fibonacci series
list=[ ]
n=int(input("enter the input n:"))
if n>=1:
    list.append(0)
    list.append(1)
for i in range(2,n):
    list.append(list[i-1]+list[i-2])
print(list)   

2.prime numbers till N

primelist=[]
n=int(input("enter n:"))
if n>=1:
    isprime=True
    for u in range(2,int(i**0.5)+1):
        if i%u == 0:
            isprime=false
            break
        if isprime:
            primelist.append(i)
    print(primelist)
else:
    print("input a number greater than 0")


3.Vowel and consonent count
def count_v_c(s):
    vowel='aeiou'
    consonant='bcdfghijklmnpqrstvwxyz'
    vc=0
    cc=0
    s=s.lower()
    for char in s:
        if char in vowel:
            vc+=1
        elif char in consonant:
            cc+=1
    return vc,cc
string =input("enter the string:")
vowels,consonants=count_v_c(string)
print(f"number of vowels:{vowels}")
print(f"number of consonants:{consonants}")     

4.Center-aligned Star triangle
n=int(input("enter the number of rows: "))
for i in range(1,n+1):
    space=n-i
    star=2*i-1
    print(" "*space +"*"*star)
    vvvv