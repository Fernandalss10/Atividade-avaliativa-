# Atividade-avaliativa-
Valendo 2,0 pontos 

1) 

>> Alternativa D.

2) 

a--  

void main() {
  
  int var1 = 1;
  int var2 = 2;
  String var3 ='Olá Mundo';
  print(var1);
  print(var2);
  print(var3);
}


b--

void main() {
  
  print ("Dez primeiros números positivos: ");
  chamada();
}
  
  void chamada(){
  for (int i = 1; i < 11; i++) {
    print(i);
  }
  }


c--

void main() {
  int num = 50;
  chamada(num);
}
  void chamada(int a){
    for (int i = 1; i <= a; i++) {
    print(i);
  }
  }
  
  
d--

void main() {
  int num = 4;
  chamada(num);
}
  
  void chamada(int a){
    int soma = 0;
    
  for (int i = 1; i <= a; i++) {
    print(i);
    soma = soma+1;
    
  }
    print (soma);
  }


e--

void main() {
  Animal a = new Animal ('Gato', 2);
  a.som();
  a.andar();
}
  class Animal {
    String nome;
    int idade;
    
    Animal(this.nome, this.idade);
    
    void som (){   
      print ('$nome emitiu som!');   
    }
    
     void andar(){      
      print ('$nome andou!');   
    }
  }
  
  
  
  
------------------------------------------------ ATIVIDADE PARA PONTO (4,0 pontos)  ----------------------------------------------


void main(){

  Banco b = new Banco('Nome', 000, 'Normal', 1000.00);
  

  print ("1- Criar conta");
  print ("2- Depósito");
  print ("3- Saque");
  print ("4- Saldo");
  print ("5- Transferência");

print ("-----------------------");
b.criar_conta();
print ("-----------------------");     
b.deposito(200.00);
print ("-----------------------");     
b.saque(100.00);
print ("-----------------------"); 
b.saldo();
print ("-----------------------");
b.transferencia(300.00);
print ("-----------------------");
         
}
class Banco {
  String nome; 
  int num;
  String tipo;
  double saldo_atual;
  double valor_depos;
  double valor_saque;
  double valor_trans;
  
  Banco(this.nome, this.num, this.tipo, this.saldo_atual);
  
  void criar_conta (){
    print ('Nome: $nome');
    print ('Conta: $num');
    print ('Tipo: $tipo');
    print ('Saldo: $saldo_atual');
  }
  
  void saldo (){
    print ('Saldo Atual: ${this.saldo_atual}');
  }
  
  void deposito (double valor_depos){
    this.saldo_atual = saldo_atual + valor_depos;
    print ("Depósito realizado com sucesso!");
    saldo();    
  }
  
  void saque (double valor_saque){
    
    if (saldo_atual >= valor_saque) {
    this.saldo_atual = saldo_atual - valor_saque;
    print ("Saque realizado com sucesso!");
    saldo(); 
    }
    else {
      print ("Saldo insuficiente!");
      saldo(); 
    }
  }
    
    void transferencia (double valor_trans){
    
    if (saldo_atual >= valor_trans) {
    this.saldo_atual = saldo_atual - valor_trans;
    print ("Tranferência realizada com sucesso!");
    saldo(); 
    }
    else {
      print ("Saldo insuficiente!");
      saldo(); 
    }
  }
  
  
  
}
  
