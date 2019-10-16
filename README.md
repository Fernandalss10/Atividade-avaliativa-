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

