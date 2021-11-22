# Armstrong-Number
#Find out if a given number is an "Armstrong Number"
num = int(input('Enter a number:  '))

sum = 0

temp = num
while temp > 0:
  digit = temp % 10
  sum += digit ** 3
  temp //= 10
  

if num == sum:
  print(num,'is an Armstrong Number.')
elif num < 0:
  print(num,'is an invalid entry. Don\'t use non-numeric, float, or negative values!')
else:
  print(num,'is not an Armstrong Number.')
