#Exercicio 3


#Interface Pato:

public interface Pato {
    void voar();
}


#Classe PatoDeCabe�aVermelha:

public class PatoDeCabe�aVermelha implements Pato {
    public PatoDeCabe�aVermelha() {
    }

    public void voar() {
        System.out.println("Batendo as asas");
    }
}



#classe PatoCibernetico:


public class PatoCibernetico implements Pato {
    public PatoCibernetico() {
    }

    public void voar() {
        System.out.println("Ligando o jetpack");
    }
}


#Main:


public static void main(String[] args) {
	  Pato pato = new PatoDeCabe�aVermelha();
                System.out.println("Pato de cabe�a Vermelha Voa:");
                pato.voar();
                Pato patoCibernetico = new PatoCibernetico();
                System.out.println("Pato cibernetico Voa:");
                patoCibernetico.voar();
}

