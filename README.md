# Visitantes
public class Visitante {
    private String nome;
    private String fone;
    private String cidadeResidencia;
    private String sexo;
    private String profissao;
    private int nascimento;
    
        
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

    public int getNascimento() {
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

    public void setNascimento(int nascimento) {
        this.nascimento = nascimento;
    }
    
}








public class festa {
    public static void main(String[] args) {
        ArrayList<Visitante> Visitantes = new ArrayList<>();
        
        int options, isRunning = 1;
        
        ArrayList<String> cidades = new ArrayList<String>();
        int quantHomens = 0, quantMulheres = 0, quantMenores = 0;
        
        while(isRunning == 1) {
            options = Integer.parseInt(JOptionPane.showInputDialog("1) Novo cadastro \n2) Mostrar resultado \n3) Fechar"));
            
            if (options == 1) {
                Visitante v = new Visitante();
                
                v.setNome(JOptionPane.showInputDialog("Informe o nome:"));
                v.setCidadeResidencia(JOptionPane.showInputDialog("Informe a cidade:"));
                v.setSexo(JOptionPane.showInputDialog("Informe o sexo (F ou M):"));
                v.setProfissao(JOptionPane.showInputDialog("Informe a profissão"));
                v.setFone (JOptionPane.showInputDialog("Telefone:"));
                v.setNascimento(Integer.parseInt(JOptionPane.showInputDialog("Ano de nascimento (AAAA):")));
                
                if (v.getNascimento() > 2004 ) {
                    quantMenores++;
                }
                
                if (v.getSexo().equals("M")) {
                    quantHomens++;
                } else if (v.getSexo().equals("F")) {
                    quantMulheres++;
                }
                
                if (!cidades.contains(v.getCidadeResidencia())) {
                    cidades.add(v.getCidadeResidencia());
                }
                
                Visitantes.add(v);
            } else if (options == 2) {
                JOptionPane.showMessageDialog(null, "INFO\n\n Total: "+ Visitantes.size() + "\n Homens: " + quantHomens + " - " + (quantHomens * 100 / Visitantes.size()) + "%" + "\n Mulheres: " + quantMulheres + " - " + (quantMulheres * 100 / Visitantes.size()) + "%" + "\n Menores de Idade: " + quantMenores + "\n Cidades: " + cidades.size());
            } else {
                isRunning = 0;
            }
            
        }
    }
}
