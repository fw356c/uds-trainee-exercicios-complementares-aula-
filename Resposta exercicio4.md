#Exercicio 4

#Main

	public class Main {
    		public static void main(String[] args) {
        		Macaco macaco = new Macaco("kenji",4);
        		macaco.andar();
        		macaco.comerBanana();
		}
	}

#Classe Animal:

	public abstract class Animal {
    		private String nomeAnimal = null;
    		private Integer quantidaDePatas = null;
    		protected Integer distancia = 0;
    		protected Integer peso = 20;

    	public Animal(String nomeAnimal, Integer quantidadePatas) {
        	this.nomeAnimal = nomeAnimal;
        	this.quantidaDePatas = quantidadePatas;
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
        	this.peso = this.peso + 1;
    		}
	}
