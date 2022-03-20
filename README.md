def spravka():
    izbor=input(": ")
    if izbor==("1"):
        cena=input("цена на еденичен продукт:")
        nacenka=input("процент наценка:")
        cena2= float(cena) * float(nacenka)/100
        cena3= float(cena) + float(cena2)
        print("продажна цена:"+ str(cena3) )
    elif izbor==("2"):
        cena=input("цена на бутилка: ")
        nacenka=input("процент наценка: ")
        cena2=float(cena)/14
        cena3=float(cena2) * float(nacenka)/100
        cena4= float(cena2)+float(cena3)
        print("цена на малкото: "+ str(cena4))
    elif izbor==("3"):
        produkt=input("име на продукт: ")
        kolichestvo=input("количество: ")
        cena=input("цена на продукт: ")
        print((produkt)+str(kolichestvo)+str(cena))
    elif izbor==("4"):
        menu()
    else:
        print("грешна команда")





def menu():
    print("""
                 menu 
             1-справка цена
             2-излизане """)

    izbor=input(": ")
    if izbor==("1"):
        print("""цена на 
        1 - еденичен продукт
        2 - за цена на малко бутилка
        3 - друга стока
        4 -за връшане към предишното меню""")

        spravka()

    elif izbor==("2"):
        print("Довиждане!")
        quit()
    else:
        print("грешна команда")




greet=print("""
        Добре дошъл в Softbar.
Най-добрия софтуер за барове и ресторанти!!!""")

login=print("""
Въведете информация за влизане:""")
user=input("user:")
password=input("password:")
if user==("vlado") and password==("190596"):
    print("Добре дошли")
    menu()
else:
    print("грешно име или парола !")

