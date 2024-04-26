# teste1
//Esquema relacionado a vendas de uma sapataria.





import java.util;
import java.util.ArrayList;
import java.util.Date;
import java.util.List;
    public void realizarVenda
public class Main {
    public static void main(String[] args) {
        Cliente cliente = new Cliente();
        Vendedor vendedor = new Vendedor();
        Produto produto = new Produto();
        cliente.realizarCompra(new Venda());
        vendedor.realizarVenda(new Venda());
        
public class Cliente {
    private int idCliente;
    private String nome;
    private String telefone;
    private String cpf;
    private Cupom cupomDesconto; 

    public Cupom consultarCupom(String codigoCupom) {
        return null;
    }

    public void realizarCompra(Venda venda) {
    }
}

public class Vendedor {
    private int idVendedor;
    private String nome;
    private String telefone;
    private String login;
    private String senha;
    private List<PedidoReporEstoque> pedidosReporEstoque;

    public boolean verificarLogin(String login, String senha) {
        return false;
    }

da(Venda venda) {
    }

    public void realizarEstorno(Venda venda) {
    }

    public void imprimirCupom(Venda venda) {
    }

    public void alterarSenha(String novaSenha) {
    }

    public PedidoReporEstoque gerarPedidoReporEstoque(Produto produto, int quantidade) {
        
        return null;
    }
}

public class Produto {
    private int idProduto;
    private String codigoBarra;
    private String descricao;
    private String marca;
    private double preco;
    private int quantidadeEstoque;

    public boolean verificarDisponibilidade(String tamanho) {
        return false;
    }

    public void diminuirEstoque(int quantidadeVendida) {
        
    }
}

public class Venda {
    private int idVenda;
    private Date dataVenda;
    private double valorTotal;
    private Pagamento formaPagamento;
    private Cliente cliente;
    private Vendedor vendedor;
    private List<ItemVenda> itensVenda;

    public void addItemVenda(Produto produto, String tamanho, int quantidade) {
    }

    public void aplicarDescontoCupom(String codigoCupom) {
   }

    public void finalizarVenda() {
    }
}

public class ItemVenda {
    private Produto produto;
    private String tamanho;
    private int quantidade;
    private double valorUnitario;
}

abstract class Pagamento {
    private int idPagamento;
    private String tipoPagamento;
    private double valorPago;

    public abstract boolean autorizarPagamento();
}

class PagamentoDebito extends Pagamento {
    private String banco;
    private String numeroCartao;

    public boolean autorizarPagamento() {
        return false;
    }
}

class PagamentoCredito extends Pagamento {
    private String bandeira;
    private int numeroParcelas;

    public boolean autorizarPagamento() {
        
        return false;
    }
}

class PagamentoPix extends Pagamento {
    private String chavePix;

    public boolean autorizarPagamento() {
        return false;
    }
}

class Estoque {
    private int idEstoque;
    private int quantidadeDisponivel;

    public boolean verificarDisponibilidadeProduto(String codigoBarra, String tamanho) {
        return false;
    }

    public void diminuirDisponibilidadeProduto(String codigoBarra, String tamanho, int quantidadeVendida) {
        
    }
}

class Cupom {
    private String codigo;
    private double desconto;
    private boolean valido;

    public void utilizarCupom() {
        
    }
}

class PedidoReporEstoque {
    private int idPedidoReporEstoque;
    private Produto produto;
    private int quantidade;
    private Date dataPedido;

    public void gerarPedido() {
    }
}
