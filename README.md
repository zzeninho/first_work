# first_work
meu primeiro trabalho em python
print('CONVERTOR DE MINUTOS PARA SISTEMA CENTESIMAL')
continuar = 's'
while continuar == 's':
    print('horario:\n 7:00 as 17:00 == 1 \n 7:30 as 17:30 == 2')
    ponto =int(input('qual você escolhe?'))
    sexta =str(input('é sexta(s/n)?'))
    hentrada = float(input('qual foi o horario de entrada:'))
    hsaida =float(input('qual foi o horario de saida:'))
    dentrada = hentrada
    add = 0
    minutos =0

    # convertor do minutos para o trem lá
    if ponto == 1 and sexta == 'n':
        if hsaida > 1700 :   
            hsaida -= 1700
            if hsaida >= 100:
                while hsaida >= 100:
                    hsaida -= 100
                    minutos += 60
            minutos += hsaida
        resutado = (minutos/60) 
    #-------------------------------------------------------------        
        if dentrada < 700:
            while dentrada != 700:  
                add += 1
                dentrada += 1 
     # tranformando o numero em horas normais           
                if dentrada == 660 or dentrada == 560 or dentrada == 460:
                    dentrada -= 60
                    dentrada += 100
        resutado += (add/60)
        print('o total é {:.2f}'.format(resutado)) 
    #---- --------- ---- ---------- 
    if ponto == 2 and sexta == 'n':
        if hsaida > 1730 :   
            hsaida -= 1730
        if hsaida >= 100:
            while hsaida >= 100:
                hsaida -= 100
                minutos += 60
        minutos += hsaida
        resutado = (minutos/60) 
        if dentrada < 730:
            while dentrada != 730:
                dentrada += 1 
                add += 1
                if dentrada == 660 or dentrada == 560 or dentrada == 460:
                    dentrada -= 60
                    dentrada += 100
        resutado += (add/60)
        print('o total é {:.2f}'.format(resutado)) 
    #------------------------ dias de sexta----------------------------------------------------------------
    if ponto == 1 and sexta == 's':
        if hsaida > 1600 :   
            hsaida -= 1600
        if hsaida >= 100:
            while hsaida >= 100:
                hsaida -= 100
                minutos += 60
        minutos += hsaida
        resutado = (minutos/60) 
        if dentrada < 700:
            while dentrada != 700:
                dentrada += 1 
                add += 1
                if dentrada == 660 or dentrada == 560 or dentrada == 460:
                    dentrada -= 60
                    dentrada += 100
        resutado += (add/60)
        print('o total é {:.2f}'.format(resutado))
    if ponto == 2 and sexta == 's':
        if hsaida > 1630 :   
            hsaida -= 1630
        if hsaida >= 100:
            while hsaida >= 100:
                hsaida -= 100
                minutos += 60
        minutos += hsaida
        resutado = (minutos/60) 
        if dentrada < 730:
            while dentrada != 730:
                dentrada += 1 
                add += 1
                if dentrada == 660 or dentrada == 560 or dentrada == 460:
                    dentrada -= 60
                    dentrada += 100
        resutado += (add/60)
        print('o total é {:.2f}'.format(resutado))
    continuar = str(input('quer continuar (s/n)?'))
