listaBart = []
listaHomer = []
listaNulos = []
#LISTAS
def voto():
  programa = int(input("Digite seu voto: [1] Bart [2] Homer: "))
  if programa == 1:
    listaBart.append(programa)
  elif programa == 2:
    listaHomer.append(programa)
  else:
    listaNulos.append(programa)

def executar():
  if len(listaHomer) > len(listaBart):
    print(f"O personagem mais votado foi Homer com {len(listaHomer)} votos e o menos votado foi Bart com {len(listaBart)} voto(s). Houve um total de {len(listaNulos)} voto(s) nulo(s).")
  elif len(listaBart) > len(listaHomer):
    print(f"O personagem mais votado foi Bart com {len(listaBart)} votos e o menos votado foi Homer com {len(listaHomer)} voto(s). Houve um total de {len(listaNulos)} voto(s) nulo(s).")
  else:
    print(f"Bart e Homer empataram com {len(listaHomer)} e {len(listaBart)} votos. Houve um total de {len(listaNulos)} votos nulo(s).")

def main():
    for i in range (5):
        voto ()
    executar()

# EXECUÇÃO
if __name__ == '__main__':
   main()


