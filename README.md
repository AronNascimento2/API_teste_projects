# Sobre o Projeto
API Rest de listagem de beneficiários,
com alguns dados básicos:
 * Nome;
 * Categoria;
 * Título;
 * Descrição;
 * Imagem;


# Como rodar?
  ### Primeiro, clone o projeto, com o seguinte comando:
  <blockquote>
    <code>git clone https://github.com/AronNascimento2/API_teste_projects.git</code>
  </blockquote>
  </br>

  ### Para rodar sem o docker (Necessita do mongodb rodando na porta 27017) execute o comando: </br></br>
  <blockquote>
    <code>npm run start</code>
  </blockquote>
  </br>


 
# Rotas
## Criar beneficiário </br></br>

<blockquote>
  <strong>Método:</strong> POST </br>
  <strong>URL:</strong> https://api-teste-projects.vercel.app/projects </br>
  <strong>Body (JSON):</strong> </br> </br>

  ```yaml
   {
    "name": "Terrus Carbon Coffe",
    "categorie": "Categoria x",
    "title": "Este projeto de redução de emissão ...",
    "description": "Lorem Ipsum is simply dummy ...",
    "image": "https://caminhodaimagem"
  }
  ```
</blockquote>
</br>

## Listar todos projetos: </br></br>

<blockquote>
  <strong>Método:</strong> GET </br>
  <strong>URL:</strong> https://api-teste-projects.vercel.app/projects </br>

  <strong>Resposta (JSON):</strong> </br></br>

  ```yaml
    [
      {
    "name": "Terrus Carbon Coffe",
    "categorie": "Categoria x",
    "title": "Este projeto de redução de emissão ...",
    "description": "Lorem Ipsum is simply dummy ...",
    "image": "https://caminhodaimagem"
  }
    ]
  ```
</blockquote>
</br>

## Listar um único projeto: </br></br>

<blockquote>
  <strong>Método:</strong> GET </br>
  <strong>URL:</strong> https://api-teste-projects.vercel.app/projects/:id </br>
  <strong>Resposta (JSON):</strong> </br></br>

  ```yaml
    {
    "name": "Terrus Carbon Coffe",
    "categorie": "Categoria x",
    "title": "Este projeto de redução de emissão ...",
    "description": "Lorem Ipsum is simply dummy ...",
    "image": "https://caminhodaimagem"
  }
  ```
</blockquote>
</br>

## Alterar um beneficiário: </br></br>

<blockquote>
  <strong>Método:</strong> PUT </br>
  <strong>URL:</strong>  https://api-teste-projects.vercel.app/projects/:id </br>
  <strong>Body (JSON):</strong> </br> </br>

  ```yaml
    {
 "name": "Terrus Carbon Coffe"
    }
  ```
</blockquote>
</br>

## Deletar um beneficiário </br></br>

<blockquote>
 <strong>Método:</strong> DELETE </br>
  <strong>URL:</strong> https://api-teste-projects.vercel.app/projects/:id
</blockquote>
</br>



