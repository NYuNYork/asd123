szoveg = input('szöveg: ')

if szoveg[len(szoveg) - 1] == '.':
    print('kijelentő mondat')
elif szoveg[len(szoveg) - 1] == '?':
    print('kérdő mondat')
elif szoveg[len(szoveg) - 1] == '!':
    print('felkiáltó, felszólító vagy óhajtó mondat')
else:
    print('nem volt írásjel a mondat végén :(')
