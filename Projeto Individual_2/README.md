# Projeto Indivdual 2 - Curso do Senac / Resilia / CNSeg
# Banco de Dados para o Sistema RESILIADATA
## Descrição do Projeto

O RESILIADATA demanda um banco de dados sólido para armazenar informações cruciais sobre empresas parceiras, tecnologias empregadas e os colaboradores associados. O desenho do banco de dados abrange três elementos principais: Empresa, Tecnologia e Colaborador, com seus respetivos atributos e inter-relações."


## 🖥️ Diagramas 

Este projeto envolve o desenvolvimento de um banco de dados fictício para o sistema RESILIADATA, desempenhando um papel crucial na análise estratégica das tecnologias adotadas pelas nossas empresas parceiras e no mapeamento dos seus colaboradores.<br><br>
**LÓGICO**
![](/img/logico.png)

**Conceitual**
![](/img/conceitual.png)

### Funcionalidades:

1. **Cadastro detalhado de empresas parceiras:** Permite uma visão integrada das organizações que fazem parte do nosso ecossistema.
   
2. **Registro de tecnologias:** Categorização por área de aplicação (webdev, dados, marketing, etc.), facilitando a identificação de tendências e competências.
   
3. **Tabela de associação tecnológica:** Monitora e avalia as tecnologias em uso pelas empresas parceiras, garantindo uma visão atualizada do panorama tecnológico.
   
4. **Cadastro de colaboradores:** Uma base de dados para gerenciar informações sobre os profissionais envolvidos, promovendo uma rede de talentos conectada.


## Perguntas do Projeto

1. **Quais entidades são necessárias?**

- Empresa
- Tecnologia
- Colaborador

2. **Quais são os principais campos e seus tipos?**

**Empresa:**
- ID (Chave Primária, Inteiro)
- Nome (Texto)
- Contato (Texto)
- tecnologia_id (Chave estrangeira, Inteiro)
- colaborador_id (Chave estrangeira, Inteiro)

**Tecnologia:**
- ID (Chave Primária, Inteiro)
- Nome (Texto)
- Área (Texto)

**Colaborador:**
- ID (Chave Primária, Inteiro)
- Nome (Texto)
- Posição (Texto)
- Salário (Float)

3. **Como essas entidades estão relacionadas?**

- Uma empresa pode utilizar várias tecnologias (relacionamento um para muitos entre Empresa e Tecnologia).
- Um colaborador pertence a uma empresa específica (relacionamento um para muitos entre Empresa e Colaborador).

4. **Simule 2 registros para cada entidade.**

**Empresa:**
- ID: 1, Nome: "Casas Venâncio", Contato: "+552196532-xxxx", tecnologia_id: "2", colaborador_id: "1,3,4,7,9"
- ID: 2, Nome: "Ana Eletro", Contato: "+551198653-xxxx", tecnologia_id: "1", colaborador_id: "2,5,6,8"

**Tecnologia:**
- ID: 1, Nome: "PDV", Área: "Vendas"
- ID: 2, Nome: "Registros", Área: "Recursos Humanos"

**Colaborador:**
- ID: 1, Nome: "Gabriel Silva", Cargo: "Analista de Vendas", Empresa_ID: 1
- ID: 2, Nome: "Fernanda Oliveira", Cargo: "Assistente Administrativo", Empresa_ID: 2
- ID: 3, Nome: "Carlos Ferreira", Cargo: "Vendedor", Empresa_ID: 1
- ID: 4, Nome: "Ana Oliveira", Cargo: "Ajudante Geral", Empresa_ID: 1
- ID: 5, Nome: "Pedro Santos", Cargo: "Vendedor", Empresa_ID: 2
- ID: 6, Nome: "Mariana Lima", Cargo: "Gerente", Empresa_ID: 2
- ID: 7, Nome: "Rafael Costa", Cargo: "Caixa", Empresa_ID: 1
- ID: 8, Nome: "Carolina Martins", Cargo: "Fiscal", Empresa_ID: 2
- ID: 9, Nome: "Paulo Rodrigues", Cargo: "Supervisor", Empresa_ID: 1