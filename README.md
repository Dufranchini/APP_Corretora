# Estrutura do Projeto - Sistema de Monitoramento com Drone

## 📂 Estrutura
```
src/
├── html/
│   └── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── php/
│   ├── conexao.php
│   └── recebe_dados.php
└── assets/
    ├── img/
    └── icons/
```

## 🚀 Como usar
1. Coloque a pasta `src` dentro do `htdocs` do XAMPP.
2. Crie um banco de dados chamado `tcc_monitoramento` com a tabela:
   ```sql
   CREATE TABLE coordenadas (
       id INT AUTO_INCREMENT PRIMARY KEY,
       latitude VARCHAR(50),
       longitude VARCHAR(50),
       data_hora TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
   ```
3. Acesse `http://localhost/src/html/index.html`.
4. Clique em "Carregar Dados do GPS" para testar a integração inicial.
