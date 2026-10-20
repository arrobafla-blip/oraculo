# ORÁCULO — site estático para GitHub Pages

Um diário visual em português brasileiro para explorar ciclos lunares, tarot simbólico, escrita pessoal e referências do céu. A versão inicial usa HTML, CSS e JavaScript puros: não requer Node.js, compilação, banco de dados ou chaves de API.

## Conteúdo do projeto

- `index.html` — site completo, estilos e scripts em um único arquivo.
- `README.md` — estas instruções.

## Publicar gratuitamente no GitHub Pages

1. Entre em [github.com](https://github.com/) e crie um repositório. Para publicar em `https://SEU-USUARIO.github.io/`, nomeie-o `SEU-USUARIO.github.io`. Para um endereço de projeto, qualquer nome serve e o endereço será parecido com `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.
2. Extraia `oraculo-github-pages.zip` no computador. Abra a pasta `oraculo`.
3. No repositório do GitHub, escolha **Add file → Upload files** e envie `index.html` e `README.md` que estão dentro da pasta `oraculo` (não é necessário enviar a pasta ZIP).
4. Confirme as alterações em **Commit changes**.
5. Abra **Settings → Pages**. Em **Build and deployment**, escolha **Deploy from a branch**, selecione `main` e a pasta `/(root)`, depois salve.
6. Aguarde o GitHub publicar. O endereço aparece na própria tela **Settings → Pages**. Pode levar alguns minutos para ficar disponível.

Não é necessário tornar o repositório público para todos os tipos de conta/planos, mas a disponibilidade do Pages em repositórios privados depende das regras atuais do GitHub. Considere que o código e o conteúdo estático do repositório podem ser públicos.

## Funcionalidades implementadas

- Página inicial responsiva com navegação e atalhos.
- Estimativa da fase lunar com base em um ciclo médio de aproximadamente 29,53 dias, oito fases selecionáveis, significados, práticas e perguntas.
- Tiragem aleatória dos 22 Arcanos Maiores, com significado simbólico, pergunta e sugestão prática. A tiragem pode ser preparada como um novo registro no diário.
- Diário com título, texto, data, emoção e intenção; pesquisa; edição; exclusão individual; confirmação dupla antes de excluir tudo; exportação e importação JSON.
- “Meu céu pessoal” para guardar data, horário e cidade de nascimento, local da Revolução Solar e temas de acompanhamento.
- Biblioteca introdutória sobre elementos, ciclos lunares, Arcanos Maiores e práticas cotidianas.
- Layout adaptável para celular, tablet e desktop, sem dependência de build.

## Limitações conhecidas

- **A fase lunar é aproximada.** Usa uma estimativa de ciclo médio, não uma efeméride astronômica de precisão; pode divergir da fase exata em determinado horário e local.
- **Não há cálculo astrológico natal ou de Revolução Solar.** A seção “Meu céu” apenas guarda referências. Não calcula nem inventa posições planetárias, casas, aspectos, trânsitos ou interpretações.
- O tarot é uma seleção aleatória de cartas e oferece conteúdo simbólico para reflexão; não prevê o futuro de forma garantida.
- O site não sincroniza dados entre dispositivos e não tem recuperação de conta.

## Privacidade e backups

- O diário e os dados de “Meu céu” são salvos no `localStorage` do navegador atual. Este site não envia esses dados para um servidor.
- Os dados não são compartilhados automaticamente entre dispositivos ou navegadores.
- Limpar os dados do site/navegador, usar modo privado ou perder acesso ao dispositivo pode apagar os registros.
- Use **Exportar backup JSON** no diário com regularidade. O arquivo contém o conteúdo escrito e **não é criptografado**; guarde-o em local privado.
- A importação combina registros pelo ID e permite substituir os de mesmo ID. Faça backup antes de importar.
- Em computador compartilhado, evite salvar informações íntimas ou limpe os dados locais ao terminar.
- Não coloque dados pessoais natais em arquivos, commits, README, issues ou outros conteúdos do repositório. Os campos do site ficam no navegador, mas o repositório publicado é separado e pode ser público.
- O site carrega as fontes Playfair Display e DM Sans do Google Fonts quando há internet. Se indisponíveis, usa fontes de sistema como alternativa. Não são enviados os dados dos formulários a esse serviço.

## Personalizar

Edite `index.html` em um editor de texto e altere os textos, cores e conteúdos. As cores principais estão no início do CSS, dentro de `:root`. A lista de fases lunares e os 22 Arcanos Maiores estão em estruturas JavaScript próximas ao fim do arquivo. Preserve uma cópia de segurança antes de editar.

## Teste local

Basta abrir `index.html` em um navegador moderno. Não há etapa de instalação. Para testar o backup, crie um registro de exemplo, exporte o JSON e importe-o novamente.

## Nota

ORÁCULO é um projeto pessoal de reflexão e organização. Não substitui orientação médica, psicológica, financeira ou jurídica, nem apresenta astrologia ou tarot como ciência ou previsão garantida.
