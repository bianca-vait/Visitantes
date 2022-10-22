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
