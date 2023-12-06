# pythonBasicoEfg

# Orientação a objetos

class Carro:
    marca = 'Do papai'
    modelo = 'Quase uma Ferrari'
    ligado = False
    andando = False

    def ligar(self):
        self.ligado = True
        print('Ligando.......')

    def desligar(self):
        self.ligado = False
        print('Desligando.....')

    def andar(self):
        self.andando = True
        print('Vrum Vrum')

    def parar(self):
        self.andando = False
        print('Parei')

    def exibir_informações_do_carro(self):
        ligado = "Ligado" if self.ligado else "Desligado"
        movimento = "Andando" if self.andando else "Parado"

        print(self.marca, self.modelo, ligado, movimento)


carro1 = Carro()
carro1.ligar()
carro1.andar()
carro1.parar()
carro1.desligar()
carro1.exibir_informações_do_carro()
carro1.andar()
carro1.parar()
carro1.exibir_informações_do_carro()
