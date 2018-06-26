#Exercício 2

#Main

	public class Main {
    		public static void main(String[] args) {
                	Produto primeiroProduto = new Produto("Placa Mãe", 485.60);
                	Produto segundoProduto = new Produto("Placa de Video", 1330.99);
                	Produto terceiroProduto = new Produto("Memoria", 586.82);
                	Produto quartoProduto = new Produto("SSD", 189.98);
                	Produto quitoProduto = new Produto("Fonte", 269.48);
                	Pedido pedido = new Pedido();
                	pedido.adicionarProduto(primeiroProduto);
                	pedido.adicionarProduto(segundoProduto);
                	pedido.adicionarProduto(terceiroProduto);
                	pedido.adicionarProduto(quartoProduto);
                	pedido.adicionarProduto(quitoProduto);
                	pedido.calcularTotal();
	}

#Classe Pedido:

	import java.util.ArrayList;

	public class Pedido {
    		private static Double total;

    		public ArrayList<Produto> produtos = new ArrayList();


    		public  void adicionarProduto(Produto valorproduto){
        	this.produtos.add(valorproduto);
    		}

    	public void calcularTotal() {
        	produtos.stream().forEach((valorProduto)->{
            	total+=produtos.valorProduto;
        	});


        	}

    	}

#Classe Produto:

	import java.util.ArrayList;


	public class Produto {
    		String nomeProduto=null;
    		Double valorProduto=null;

    	public Produto(String nomeProduto,Double valorProduto){
        	this.nomeProduto=nomeProduto;
        	this.valorProduto=valorProduto;
    	}

    	public Produto(ArrayList<Produto> produtos) {
    		}
	}
