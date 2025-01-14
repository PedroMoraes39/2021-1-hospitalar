# Padrões de projeto

### Importante:
>O padrão de escrita adotado é o Airbnb, por favor leia a respeito. [link](https://airbnb.io/javascript/react/)

- Todo código fonte deve obrigatóriamente estar na pasta src
- Utilize a extensão .ts para arquivos typescript e a extensão .tsx para arquivos typescript react (onde existe algum comando no modelo html)
- Toda página e componente deve estar contido em uma pasta com seu nome em pascal case (TipoAssim)
- Na pasta de cada página ou componente deve existir um arquivo index.tsx e um styles.ts
- Código contido em index.tsx:

  ```
  import React from 'react'
  import {useStyles} from './styles'

  export function (Nome) ():React.ReactElement {
      const classes = useStyles()

      return <div></div>
  }
  ```

- Código contido em styles.ts:

  ```
  import { makeStyles } from '@material-ui/core'

  export const useStyles = makeStyles((theme) => ({}))
  ```

# Criando uma nova página

- Crie uma pasta como manda os padrões de projeto
- Importe sua página no arquivo routes.tsx e Adicione no componente switch o seguinte código:
  ```
  <Route path='(o caminho url do componente)' component={(Nome)} />
  ```

# Documentação útil

- [Material-UI](https://material-ui.com/)
- [Typescript](https://www.typescriptlang.org/docs/)
- [React pt-BR](https://pt-br.reactjs.org/docs/getting-started.html)
