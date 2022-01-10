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
