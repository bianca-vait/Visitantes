# Visitantes
public class Visitante {
    private String nome;
    private String fone;
    private String cidadeResidencia;
    private String sexo;
    private String profissao;
    private String nascimento;
    private int quantHomens = 0;
    private int quantMulheres = 0;
    
    public Visitante(){
        
    }

    
    public void Visitante(String fone, String cidadeResidencia, String sexo, String profissao, String nascimento) {
        this.nome = "Matheus";
        this.fone = "4822223333";
        this.cidadeResidencia = "Criciuma";
        this.sexo = "M";
        this.profissao = "Marceneiro";
        this.nascimento = "1970";
    }
    

    public Visitante(String nome, String fone, String cidadeResidencia, String sexo, String profissao, String nascimento) {
        this.nome = nome;
        this.fone = fone;
        this.cidadeResidencia = cidadeResidencia;
        this.sexo = sexo;
        this.profissao = profissao;
        this.nascimento = nascimento;
    }
        
    public String getNome() {
        return nome;
    }
        
    public String getFone() {
        return fone;
    }

    public String getCidadeResidencia() {
        return cidadeResidencia;
    }

    public String getSexo() {
        return sexo;
    }

    public String getProfissao() {
        return profissao;
    }

    public String getNascimento() {
        return nascimento;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public void setFone(String fone) {
        this.fone = fone;
    }

    public void setCidadeResidencia(String cidadeResidencia) {
        this.cidadeResidencia = cidadeResidencia;
    }

    public void setSexo(String sexo) {
        this.sexo = sexo;
    }

    public void setProfissao(String profissao) {
        this.profissao = profissao;
    }

    public void setNascimento(String nascimento) {
        this.nascimento = nascimento;
    }

    @Override
    public String toString() {
        return "Nome:" + nome + "\nFone:" + fone + "\nCidadeResidencia:" + cidadeResidencia + "\nSexo:" + sexo + "\nProfissao:" + profissao + "\nNascimento:" + nascimento;
    }
    
    public void total(){
        
    }
    
    public int contaHomens(){
        if ("M".equals(sexo)){
            this.quantHomens = quantHomens+1;
        } else if ("F".equals(sexo)){
            this.quantHomens = quantHomens+0;
        }
        return quantHomens;
        
        
    }
    
    public int contaMulher(){
        if ("F".equals(sexo)){
            this.quantMulheres = quantMulheres+1;       
    }
        return quantMulheres;   
        }
}








public class executaVisitantes {
    public static void main(String[] args) { 
        
        //Scanner ler = new Scanner (System.in);
        String nome, fone, cidadeResidencia, sexo, profissao, nascimento;
        
        /*System.out.println("Informe o nome");
        nome = ler.next();
        
        System.out.println("Informe o telefone");
        fone = ler.next();
        
        System.out.println("Informe a cidade de residencia");
        cidadeResidencia = ler.next();
        
        System.out.println("Informe o sexo");
        sexo = ler.next();
        
        System.out.println("Informe a profissao");
        profissao = ler.next();
        
        System.out.println("Informe o nascimento");
        nascimento = ler.next();*/
        
        nome = JOptionPane.showInputDialog(null, "Informe o nome:");
        fone = JOptionPane.showInputDialog(null, "Informe o telefone:");
        cidadeResidencia = JOptionPane.showInputDialog(null, "Informe a cidade de residencia:");
        sexo = JOptionPane.showInputDialog(null, "Informe o sexo:");
        profissao = JOptionPane.showInputDialog(null, "Informe a profissao:");
        nascimento = JOptionPane.showInputDialog(null, "Informe o nascimento:");
        
        
            Visitante v1 = new Visitante();
            v1.setNome(nome);
            v1.setFone(fone);
            v1.setCidadeResidencia(cidadeResidencia);
            v1.setSexo(sexo);
            v1.setProfissao(profissao);
            v1.setNascimento(nascimento);
            
        nome = JOptionPane.showInputDialog(null, "Informe o nome:");
        fone = JOptionPane.showInputDialog(null, "Informe o telefone:");
        cidadeResidencia = JOptionPane.showInputDialog(null, "Informe a cidade de residencia:");
        sexo = JOptionPane.showInputDialog(null, "Informe o sexo:");
        profissao = JOptionPane.showInputDialog(null, "Informe a profissao:");
        nascimento = JOptionPane.showInputDialog(null, "Informe o nascimento:");
            
            Visitante v2 = new Visitante();
            v2.setNome(nome);
            v2.setFone(fone);
            v2.setCidadeResidencia(cidadeResidencia);
            v2.setSexo(sexo);
            v2.setProfissao(profissao);
            v2.setNascimento(nascimento);
            
        nome = JOptionPane.showInputDialog(null, "Informe o nome:");
        fone = JOptionPane.showInputDialog(null, "Informe o telefone:");
        cidadeResidencia = JOptionPane.showInputDialog(null, "Informe a cidade de residencia:");
        sexo = JOptionPane.showInputDialog(null, "Informe o sexo:");
        profissao = JOptionPane.showInputDialog(null, "Informe a profissao:");
        nascimento = JOptionPane.showInputDialog(null, "Informe o nascimento:");
            
            Visitante v3 = new Visitante();
            v3.setNome(nome);
            v3.setFone(fone);
            v3.setCidadeResidencia(cidadeResidencia);
            v3.setSexo(sexo);
            v3.setProfissao(profissao);
            v3.setNascimento(nascimento);
            
        nome = JOptionPane.showInputDialog(null, "Informe o nome:");
        fone = JOptionPane.showInputDialog(null, "Informe o telefone:");
        cidadeResidencia = JOptionPane.showInputDialog(null, "Informe a cidade de residencia:");
        sexo = JOptionPane.showInputDialog(null, "Informe o sexo:");
        profissao = JOptionPane.showInputDialog(null, "Informe a profissao:");
        nascimento = JOptionPane.showInputDialog(null, "Informe o nascimento:");
            
            Visitante v4 = new Visitante(nome,fone,cidadeResidencia, sexo, profissao, nascimento);
            v4.setNome(nome);
            v4.setFone(fone);
            v4.setCidadeResidencia(cidadeResidencia);
            v4.setSexo(sexo);
            v4.setProfissao(profissao);
            v4.setNascimento(nascimento);
            
            
            
        
            
            System.out.println(v1.toString());
            System.out.println(v2.toString());
            System.out.println(v3.toString());
            System.out.println(v4.toString());
            
            System.out.println("Quantidade de homens:" + v1.contaHomens());
            System.out.println("Quantidade de mulheres:" + v1.contaMulher());
        }
                    
         
                
                
    }
