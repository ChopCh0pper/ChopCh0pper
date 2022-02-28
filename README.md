def count_number_6(n):
    c = 0
    s = ''
    while n > 0:
        s += str(n % 6)
        n = n // 6
    if len(s) == 2:
        return True


def count_number_5(n):
    c = 0
    s = ''
    while n > 0:
        s += str(n % 5)
        n = n // 5
    if len(s) == 3:
        return True


def lust_number_11(n):
    c = 0
    s = ''
    while n > 0:
        s += str(n % 11)
        n = n // 11
    if s[::-1][-1] == '1':
        return True


for n in range(100):
    if count_number_6(n) and count_number_5(n) and lust_number_11(n):
        print(n)
