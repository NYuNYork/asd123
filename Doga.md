print('4. feladat:')
talalat = 0
for f in range(1, 6):
  print(f'   {f}. kör:')
  x = rnd.randrange(10, 100)
  y = rnd.randrange(10, 100)
  if y > x: x, y = y, x
  print(f'     a két szám összege {x + y}, különbsége {x - y}. Mi lehet ez a két szám?')
  tx = int(input('       egyik szám: '))
  ty = int(input('       másik szám: '))
  if ty > tx: tx, ty = ty, tx
  if x == tx and y == ty:
    print('     helyes!')
    talalat += 1
  else:
    print(f'     sajnos nem, a válasz {x} és {y}')
print(f'   Végeztünk, helyes találataid száma: {talalat}')

# a = input('addj meg egy szót: ')
# b = int(input('addj meg egy számot:'))
# print(b*a)

# 2.

# import math

# a = int(input('1. oldal: '))
# b = int(input('2.oldal: '))
# c = int(input('3. oldal: '))
# s = (a + b + c) /2
# t = math.sqrt(s * ((s - a) * (s- b) * (s - c)))

# if a + b <= c or a + c <= b or b + c <= a: print('nem képezhető háromszög')

# else: print('képezhető háromszög')
# print(t)

# 3.

név = input('addjon meg egy nevet: ')
maxpont = int(input('addja meg a max pontot: '))
elértp = int(input('addja meg az eért pontot: '))

if elértp > maxpont: print('beviteli error')
százalék = elértp / maxpont * 100
print(f'{név} {százalék}%-ot ért el ')

if százalék < 51: print('1')
elif százalék < 65: print('2')
elif százalék < 77: print('3')
elif százalék < 90: print('4')
elif százalék > 90: print('5') 
