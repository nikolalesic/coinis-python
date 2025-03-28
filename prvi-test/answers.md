# Zadaci

## 1. (Izrazi)
**a.** not 4 * 2 < 8 or (3 + 5) / 2 == 4

- 4 * 2 = 8, pa 8 < 8 je False.
- not False je True.
- (3 + 5) / 2 = 8 / 2 = 4, što je True.
- True or True daje True.

**b.** (5 > 3 or 2 < 1) and 7 + 3 == 10

- 5 > 3 je True, 2 < 1 je False.
- True or False je True.
- 7 + 3 == 10 je True.
- True and True daje True.

**c.** 4 * (6 - 2) > 10 and (3 + 2 == 5)

- 4 * (6 - 2) = 4 * 4 = 16, pa 16 > 10 je True.
- 3 + 2 == 5 je True.
- True and True daje True.

**d.** 3 ** 2 + 4 > 10 and not (4 % 2 == 0 or 7 % 3 == 0)

- 3 ** 2 = 9, pa 9 + 4 = 13, što je True.
- 4 % 2 == 0 je True, 7 % 3 == 0 je False.
- True or False je True.
- not True je False.
- True and False daje False.

**e.** 8 // 3 + 6 % 4 == 4 and 'a' in 'aeiou'

- 8 // 3 = 2, 6 % 4 = 2, pa 2 + 2 == 4, što je True.
- 'a' in 'aeiou' je True.
- True and True daje True.

## 2. (Stringovi)
**a.** `s = "danas"`

- `s = s + "."` ili `s += "."`

**b.** `s = "AbCCa"`

- `s[3:5]` daje `"Ca"`.

**c.** `s[6:10]` za `"Danas je poslednji čas u ovom semestru."`

- `"je p"`.

**d.** Poslednja tri karaktera:

- `s[-3:]`.

**e.** Ako je string parne dužine `s`, srednji elementi su:

- `s[len(s)//2 - 1 : len(s)//2 + 1]`.

## 3. (Liste)
**a.** Kolekcije su strukture podataka (liste, torke, skupovi, rečnici) koje omogućavaju skladištenje i manipulaciju grupama podataka.

**b.** `range(3, 8)` generiše: `[3, 4, 5, 6, 7]`.

**c.** `len(lista[3:])` za `lista = [10, 20, 30, 25, 65, 12]`

- `lista[3:] = [25, 65, 12]`, pa `len(lista[3:]) = 3`.

**d.** `a[2:4]` za `a = [1, 2, 5, 7]`

- `[5, 7]`.

**e.** Da štampamo samo prva tri elementa liste `l`:

- `if i < 3:`

## 4. (Kod)
**a.** Program za pobjednika:

```python
books = {"Marko": 320, "Ana": 290, "Jovan": 410}
winner = max(books, key=books.get)
print(f"Pobjednik je {winner} sa {books[winner]} strana.")
