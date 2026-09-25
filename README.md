algoritmo "Caixa_Eletronico"

var
   saque, saldo: inteiro
   nota100, nota50, nota20, nota10, nota5: inteiro

inicio

   saldo <- 1500

   escreva("Digite o valor do saque: ")
   leia(saque)

   se (saque > saldo) entao
      escreval("Saque invalido!")

   senao

      nota100 <- saque div 100
      saque <- saque mod 100

      nota50 <- saque div 50
      saque <- saque mod 50

      nota20 <- saque div 20
      saque <- saque mod 20

      nota10 <- saque div 10
      saque <- saque mod 10

      nota5 <- saque div 5
      saque <- saque mod 5

      escreval("Notas entregues:")
      escreval(nota100, " nota(s) de 100")
      escreval(nota50, " nota(s) de 50")
      escreval(nota20, " nota(s) de 20")
      escreval(nota10, " nota(s) de 10")
      escreval(nota5, " nota(s) de 5")

   fimse

fimalgoritmo
