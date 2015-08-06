# codingbat

## Warmup-1

### sleep_in
weekday が false または vacation が 

```
def sleep_in( weekday, vacation):
  return ( not weekday or vacation)
```

### monkey_trouble
description

```
def monkey_trouble(a_smile, b_smile):
  #return a_smile == b_smile
  return not( a_smile ^ b_smile)
```
### sum_double
description

```
def sum_double(a, b):
  return a+b if not( a == b) else (a+b) * 2
```
### diff21
description

```
def diff21(n):
  if n < 21:
    return abs( 21 - n)
  else:
    return abs( 21 - n) * 2
```
### parrot_trouble
description

```
def parrot_trouble(talking, hour):
  if talking and (hour < 7 or hour > 20):
    return True
  else:
    return False
```
### makes10
description

```
def makes10(a, b):
  return a == 10 or b == 10 or a + b == 10
```
### near_hundred
description

```
def near_hundred(n):
  if abs( 100 - n) <= 10 or abs( 200 - n) <= 10:
    return True
  return False
```
### pos_neg
description

```
def pos_neg(a, b, negative):
  if ( not(negative) and not( (a < 0) == (b < 0))) or ( negative and a < 0 and b < 0):
    return True
  return False
```
### not_string
description

```
def not_string(str):
  return ('not {0}'.format( str)) if not( str.split()[0] == 'not') else str
```
### missing_char
description

```
def missing_char(str, n):
  return str[:n] + str[n+1:]
```
### front_back
description

```
def front_back(str):
  return str if len(str) <= 1 else str[-1:] + str[1:-1] + str[0]
```
### front3
description

```
def front3(str):
  return str[0:3]*3
```

## Warmup-2

### string_times
description

```
def string_times(str, n):
  return str*n
```
### num
description

```
```
### front_times
description

```
def front_times(str, n):
  return str[:3]*n
```
### string_bits
description

```
def string_bits(str):
  res = ''
  for i in range( len(str)):
    if i % 2 == 0:
      res += str[i]
  return res  
```
### string_splosion
description

```
def string_splosion(str):
  res = ''
  for i in range( len(str)+1):
    res += str[:i]
  return res
```
### last2
description

```
def last2(str):
  count = 0
  for i in range( len( str)-2):
    if str[i:i+2] == str[-2:]: count += 1
  return count
```
### array_count9
description

```
def array_count9(nums):
  count = 0
  for i in nums:
    if i == 9: count += 1
  return count
```
### array_front9
description

```
def array_front9(nums):
  for i in range( len(nums)):
    if i >= 4: break
    if nums[i] == 9: return True
  return False
```
### array123
description

```
def array123(nums):
  count = 0
  for i in range( len(nums)-1):
    count = ( count + 1 if nums[i]+1 == nums[i+1] else 0)
    if count >= 2: return True
  return False
```
### string_match
description

```
def string_match(a, b):
  count = 0
  for i in range( ( len(a) if len(a) >= len(b) else len(b)) - 1):
    if a[i:i+2] == b[i:i+2]:
      count += 1
  return count
```
