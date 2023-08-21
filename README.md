# Folha-de-pagamento-com-VT-Inss
Folha de pagamento com VT e INSS

salarioB  =  float ( input ( "Digite o salario: " ))
vale  =   input ( "Descontar o Vale Transporte?" )
se  salarioB  < 1302,00 :
se  salarioB  < 1320,01 :
    inss  =  salarioB * 0,075
    print ( f"Calculo do INSS R$ { inss } " )
    salarioL  = ( salarioB - inss )
    print ( "Seu salário líquido é de: R$" , salarioL )
elif  salarioB  < 2571. 29 :
    inss  =  salarioB * 0,09
elif  salarioB  > 1320,00 e salarioB < 2571. 30 :    
    inss  =  ( salarioB - 1320 ) * 0,09 + 99    
    print ( f"Calculo do INSS R$ { inss } " )
    salarioL  = ( salarioB - inss )
    print ( "Seu salário líquido é de: R$" , salarioL )
elif  salarioB  < 3856. 94 :
    inss  =  salarioB * 0,12
elif  salarioB  > 2571,29 e salarioB < 3856. 95 :     
    inss  =  ( salarioB - 2571,29 ) * 0,12 + 99 + 112,62       
    print ( f"Calculo do INSS R$ { inss } " )
    salarioL  = ( salarioB - inss )
    print ( "Seu salário líquido é de: R$" , salarioL )
elif  salarioB  < 7507. 49 :
    inss  =  salarioB * 0,14
elif  salarioB  > 3856,94 e salarioB < 7507. 50 :     
    INSS  =  ( salárioB - 3856,95 ) * 0,14 + 99 + 112,62 + 154,28         
    print ( f"Calculo do INSS R$ { inss } " )
    salarioL  = ( salarioB - inss )
    print ( "Seu salário líquido é de: R$" , salarioL )
elif  salarioB  > 7507. 50 :
    inss  =  salarioB - 876 , 95
elif  salarioB  > 7507. 49 :
    inss  =  ( salarioB - 3856 , 95 ) * 0,14 + 99 + 112,62 + 154,28         
    print ( f"Calculo do INSS R$ { inss } " )
    salarioL  = ( salarioB - inss )
    print ( "Seu salário líquido é de: R$" , salarioL )
senão :
    print ( "Sem comentários!" )
#print(salarioB, " ", salarioL)
    print ( "Ops! Algo deu errado, contate seu programador!" )
se  vale  ==  "s"  ou  vale  ==  "S" :
    valVale  =  salarioL * 0,06
    valVale  =  ( salarioB - inss ) * 0,06
    print ( f"Desconto do vale transporte é de R$ { valVale } " )
    salarioL  =  salarioB  -  valVale
    salarioL  =  ( salarioB - inss )  -  valVale
    print ( "Seu salário líquido é de: R$" , salarioL )
