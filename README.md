# Olá! Eu sou a Yasmin Lopes 👋

![ADS](https://img.shields.io/badge/Status-Estudante-blue?style=for-the-badge)
![Foco](https://img.shields.io/badge/Foco-Engenharia%20de%20Dados-orange?style=for-the-badge)

Análise e Desenvolvimento de Sistemas | Aspirante à Engenharia de Dados | SQL | Python | Cloud (AWS)

---

### 🛠 Tecnologias e Ferramentas
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![SQL](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

---

### 🚀 Sobre Mim

* 🎓 *Atualmente no 3º semestre*, mergulhando em Modelagem de Dados e SQL para construir bases sólidas em arquitetura de dados.
* 🎯 *Objetivo:* Transição de carreira com foco em Engenharia de Dados, transformando dados brutos em soluções inteligentes e escaláveis.
* 📚 *Mentalidade:* Entusiasta da cultura "Agir rápido, aprender rápido". Sou uma "esponja" para absorver novos conhecimentos técnicos todos os dias.

### ⚙️ No que estou focada agora:

* *SQL & Bancos de Dados:* Praticando consultas complexas, joins e estruturação de tabelas diariamente.
* *Lógica de Programação:* Resolvendo desafios em plataformas como LeetCode para fortalecer o raciocínio lógico.
* *Documentação:* Registro cada nova descoberta técnica, transformando erros de sintaxe em guias de aprendizado práticos.

---

### 📊 Demonstração Técnica Recente
Abaixo, um trecho do pipeline que desenvolvi para monitoramento de hardware, utilizando POO e Pandas:

```python
# Trecho do pipeline de extração e limpeza (Camada Silver)
def transform_data(self):
    df = pd.DataFrame(self.raw_data)
    
    # Limpeza de Preço com Regex
    df['price_numeric'] = df['price'].apply(lambda x: float(re.sub(r'[R\$\s\.]', '', x).replace(',', '.')))
    
    # Categorização Automática
    df['category'] = df['item'].apply(lambda x: 'GPU' if 'GPU' in x else 'CPU')
    
    return df


