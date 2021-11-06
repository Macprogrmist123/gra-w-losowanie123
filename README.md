#py game 
#gra-w-losowanie123
#gra w której musisz zgadnąć liczbe od 1 do 10 masz na to 3 próby 


from random import randint

los = randint(1,10)
odp = -1
i = 1

odp = int(input("podaj liczbę:"))
if los == odp:
    print("zgadłeś liczbę")
    print("zgadłeś w probe nr:")
    print(i)
if los != odp:
    i = i + 1
    print("podałeś złą liczbę")
    if los > odp:
        print("trochę więcej")
    else:
        print("trochę mniej")
    print("---------------------")
    odp = int(input("podaj liczbę:"))
    if los == odp:
        print("zgadłeś liczbę")
        print("zgadłeś w probe nr:")
        print(i)
    if los != odp:
        i = i + 1
        print("podałeś złą liczbę")
        if los > odp:
            print("trochę więcej")
        else:
            print("trochę mniej")
        print("---------------------")
        odp = int(input("podaj liczbę:"))
        if los == odp:
            print("zgadłeś liczbę")
            print("zgadłeś w probe nr:")
            print(i)
        if los != odp:
            i = i + 1
            print("podałeś złą liczbę")
            print("odpowiedź to: ")
            print(los)







