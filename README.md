

# petmatch-analise-sistema 🐾

## PetMatch – Sistema Inteligente de Adoção de Pets

📌 **Sobre o Projeto**
Este é um projeto de estudo focado em Engenharia de Requisitos e Análise de Sistemas. O PetMatch foi idealizado para conectar animais de abrigos e ONGs a tutores ideais por meio de um algoritmo de compatibilidade, visando reduzir as taxas de abandono pós-adoção.

---

📋 **Requisitos Funcionais**

* **RF01 - Cadastro do Pet:** O sistema permite registrar Nome, Tipo (Cachorro/Gato), Idade, Porte (P/M/G), Energia (Baixa/Média/Alta) e Necessidades Especiais.
* **RF02 - Questionário do Tutor:** Coleta dados sobre o tipo de imóvel, tempo livre disponível e orçamento planejado para os cuidados com o pet.
* **RF03 - Algoritmo de Match:** Cruza as respostas do questionário com o perfil do animal (ex: tutor em apartamento com pouco tempo livre recebe recomendação de pets de porte pequeno e baixa energia).
* **RF04 - Solicitação de Contato:** Gera uma ponte direta enviando os dados de contato do tutor (E-mail e WhatsApp) para a ONG responsável pelo animal.
* **RF05 - Cancelamento de Solicitação:** Permite que o tutor cancele uma intenção de adoção antes que a ONG faça o primeiro contato.
* **RF06 - Filtros de Busca Avançados:** Permite que o usuário busque pets manualmente por critérios como espécie, idade ou porte, sem depender apenas do match automático.

---

💾 **Modelagem de Dados (Estrutura Simples)**

### Tabela: Pets
* ID (Chave Primária)
* Nome
* Tipo (Cachorro/Gato)
* Idade
* Porte (P/M/G)
* Nível de Energia (Baixa/Média/Alta)
* Necessidades Especiais
* Status de Adoção (Disponível/Adotado)

### Tabela: Tutores
* ID (Chave Primária)
* Nome Completo
* E-mail
* Celular (WhatsApp)
* Tipo de Imóvel (Casa/Apartamento)
* Tempo Disponível (Pouco/Médio/Muito)
* Orçamento para o Pet (Baixo/Médio/Alto)

### Tabela: Histórico de Matches
* ID (Chave Primária)
* ID do Tutor (Chave Estrangeira)
* ID do Pet (Chave Estrangeira)
* Data da Solicitação
* Status do Contato (Pendente/Enviado para ONG)


