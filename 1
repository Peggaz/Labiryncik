class Stan:
    def __init__(self, x=0, y=0, poprzednik=None):
        self.x = x
        self.y = y
        self.poprzednik = poprzednik


HistoriaStanow = []
StanyDoEkspansii = []


def szukaj():
    S = Stan()
    StanyDoEkspansii.append(S)
    HistoriaStanow.append(S)
    while True:
        S = wybierz_stan_do_ekspansji()
        if S is None:
            print("Brak drogi ucieczki")
            break
        if czy_rozwiazanie(S):
            while True:
                if S is not None:
                    print("(" + str(S.y) + "; " + str(S.x) + ")")
                    S = S.poprzednik
                else:
                    break
            break
        LS = ekspanduj_stan(S)
        LS = filtruj_stany(LS)
        uaktualnij_stany(LS)


def uaktualnij_stany(LS):
    for s in LS:
        StanyDoEkspansii.append(s)
        HistoriaStanow.append(s)


def spelnia_ograniczenia(S):
    return 0 <= S.x <= 9 and 0 <= S.y <= 9


def jest_nowa(S):
    for h in HistoriaStanow:
        if S.x == h.x and S.y == h.y:
            return False
    return True


def filtruj_stany(LS):
    StanyOk = []
    for s in LS:
        if spelnia_ograniczenia(s) and jest_nowa(s):
            StanyOk.append(s)
    return StanyOk


def ekspanduj_stan(S):
    NoweStany = []
    if S.x + 1 <= 9:
        if trasa[S.x + 1][S.y] == 0:
            NoweStany.append(Stan(S.x + 1, S.y, S))
    if S.y + 1 <= 9:
        if trasa[S.x][S.y + 1] == 0:
            NoweStany.append(Stan(S.x, S.y + 1, S))
    if S.x - 1 >= 0:
        if trasa[S.x - 1][S.y] == 0:
            NoweStany.append(Stan(S.x - 1, S.y, S))
    if S.y - 1 >= 0:
        if trasa[S.x][S.y - 1] == 0:
            NoweStany.append(Stan(S.x, S.y - 1, S))
    return NoweStany


def wybierz_stan_do_ekspansji():
    if len(StanyDoEkspansii) == 0:
        return None
    S = StanyDoEkspansii[0]
    StanyDoEkspansii.remove(S)
    return S


def czy_rozwiazanie(S):
    return S.x == 9 and S.y == 9


trasa = [[0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 1, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 1, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 1, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0, 1, 0, 1, 0],
         [0, 0, 0, 0, 1, 0, 0, 0, 1, 0],
         [0, 0, 0, 0, 1, 0, 1, 0, 1, 0],
         [0, 0, 0, 1, 1, 0, 1, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 1, 0, 0, 0]]
for i in trasa:
    print(i)
print("\n0  1  2  3  4  5  6  7  8  9\n")
szukaj()
