# Landing Page Frontend - Antonio Pereira

Landing page estática para candidatura de Antonio Pereira à vaga de Desenvolvedor Frontend presencial em Campinas/SP.

O objetivo é apresentar, de forma objetiva, competências em HTML5, CSS3, JavaScript, responsividade, acessibilidade, Git/GitHub e colaboração técnica, usando o VotoData Brasil como projeto demonstrável de produto, dados, documentação e entrega auditável.

## Escopo

- Página estática em HTML, CSS e JavaScript puro.
- Sem build obrigatório e sem dependências externas de runtime.
- Layout responsivo, navegação acessível e suporte a `prefers-reduced-motion`.
- Publicação isolada via GitHub Pages.
- Conteúdo autoral, sem uso de assets, marca, imagens ou identidade visual da Relier.

## Execução local

A partir da raiz do repositório:

```bash
npm run start
```

Acesse:

```text
http://127.0.0.1:8000/landing/relier-frontend/
```

Opcionalmente, a página também pode ser servida diretamente do diretório da landing com um servidor estático local.

## GitHub Pages

O workflow `.github/workflows/deploy-landing-pages.yml` publica somente o diretório:

```text
landing/relier-frontend
```

Para habilitar:

1. Acesse `Settings > Pages`.
2. Configure `Source` como `GitHub Actions`.
3. Execute o workflow manualmente ou faça push na `main` com mudanças na landing.

## Workflow moderno

A evolução da landing pode ser feita em GitHub Codespaces com apoio do Codex e dos agentes do projeto:

- `DOCS_PRODUCT_AGENT`: clareza de posicionamento, README e linguagem profissional.
- `UX_AGENT`: responsividade, acessibilidade e experiência visual.
- `QA_CI_AGENT`: lint, testes e validação de regressão.
- `SECURITY_AGENT`: exposição pública, ausência de segredos e uso seguro do Pages.

Codex é tratado como ferramenta de produtividade para scaffolding, revisão, documentação e refino. As decisões técnicas, a validação final e a responsabilidade da entrega permanecem com Antonio.

## Contato

Contatos configurados na landing:

- E-mail: `icloud.pereira@icloud.com`.
- LinkedIn: `https://www.linkedin.com/in/antonio-pereira-professional/?locale=pt`.
- GitHub do projeto: `https://github.com/k3L0w/votodata-brasil`.

## Segurança

Esta landing não precisa de segredos para funcionar. O deploy usa GitHub Pages com permissões restritas no workflow:

- `contents: read`
- `pages: write`
- permissão de identidade do GitHub Pages

Não publicar chaves de acesso, senhas, chaves privadas, arquivos de ambiente ou credenciais no HTML, CSS, JS, README ou workflows. Não adicionar formulários que enviem dados sensíveis sem backend, política de privacidade e tratamento explícito.
