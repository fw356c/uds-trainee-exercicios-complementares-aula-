#Exercício 1

#Main:

	public class Main {
    		public static void main(String[] args) {
      		Macaco macaco = new Macaco("kenji");
       		macaco.andar();
       		macaco.comerBanana();

		}
	}

#Classe Animal:

	public abstract class  Animal{
    		private String nomeAnimal=null;
  


    	public Animal(String nomeAnimal,Integer quantidadePatas){
        	this.nomeAnimal=nomeAnimal;
        	this.quantidaDePatas=quantidadePatas;

    	}

    	public void andar() {
        	System.out.println("O"+nomeAnimal+"esta Andando!");
        
    	}


	}

#Classe Macaco:
	public class Macaco extends Animal {
    	public Macaco(String nomeAnimal, Integer quantidaDePatas) {
        	super(nomeAnimal, quantidaDePatas);
    	}

    	public void andar() {
        	this.distancia = this.distancia + 10;
        	this.peso = this.peso - 1;
    	}

    	public void comerBanana() {
        	System.out.println("O"+nomeAnimal+"esta Comendo Banana!");
    		}
	}

