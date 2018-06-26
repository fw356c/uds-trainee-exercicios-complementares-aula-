import java.util.Scanner;

	public class Main {
    		public static void main(String[] args) {
        	Integer pontosIniciais = 100;

        	System.out.println("ESCOLHA 1 para Numeros Pares e 2 Para Numeros Impares\nSe acertar ganha 10 se errar perder 10\nQUE OS JOGOS COMECEM !!!!!!");

        	while ( pontosIniciais >= 0 ) {
            	if (pontosIniciais==0){
                	break;
            	}
  	    	Scanner scanner = new Scanner(System.in);
            	Integer escolha = scanner.nextInt();
            	Random random = new Random();
            	Integer numeroRandomico = random.random();
	    	if (escolha == 1) {
                	isPar(numeroRandomico);
                	if (isPar(numeroRandomico) == true) {
                    	pontosIniciais += 10;
                	} else pontosIniciais -= 10;
            	} else if (escolha == 2) {
                	isPar(numeroRandomico);
                	if (isPar(numeroRandomico) == false) {
                    	pontosIniciais += 10;
                	} else pontosIniciais -= 10;
            	}

            	System.out.println(pontosIniciais);
        	}
    	}

    	private static boolean isPar(Integer numero) {
        	return (numero % 2) == 0;
    		}

	}


Função Random.java


	public class Random {

    		public int random() {
        	int random=(int)(Math.random()*99);
        	System.out.println(random);

        	return random;
    		}

	}


