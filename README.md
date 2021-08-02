npx json-server --watch api/data/dados.json


# consultas

`
  query Listar($userId: ID!) {
    user(id: $userId) {
      nome,
      email,
      ativo,
      role {
        type
      }
    }
  }

  query TodosUsuarios {
    users {
      id,
      nome,
      email,
      role {
        type
      }
    }
  }
`