# Aurora Odontologia

Landing page de portfólio para uma clínica odontológica fictícia. O projeto demonstra uma experiência completa de descoberta e contato, com direção visual editorial, conteúdo em português e integração opcional de e-mail.

[![CI](https://github.com/oEnzoRibas/Aurora/actions/workflows/ci.yml/badge.svg)](https://github.com/oEnzoRibas/Aurora/actions/workflows/ci.yml)

## Demonstração da Plataforma

[![Prévia animada da Aurora mostrando o consultório, a seleção de clareamento e a confirmação do formulário demonstrativo.](docs/media/demo-preview.webp)](docs/media/demo.mp4)

[Assistir à demonstração completa · MP4, 37 s, 720p, sem áudio](docs/media/demo.mp4)

O vídeo percorre a clínica, apresenta a equipe, navega por um depoimento e abre uma pergunta frequente. Depois, acompanha a escolha de clareamento até o envio do formulário com dados fictícios.

<details>
<summary>Ver a página inicial em desktop e mobile</summary>

![Página inicial da Aurora em desktop e mobile. O título “Um novo olhar para o seu sorriso” aparece ao lado de uma fotografia conceitual do consultório.](docs/images/aurora-preview.webp)

</details>

## Comece por aqui

Requisitos: Node.js 22 ou 24 e npm. A instalação local abre em modo demonstração e dispensa credenciais.

```sh
npm ci
npm run dev
```

Acesse [http://localhost:3000](http://localhost:3000). Para percorrer o fluxo, selecione **Tenho interesse** em um tratamento, preencha o formulário com dados fictícios e clique em **Simular envio**.

| Comando | O que faz |
| --- | --- |
| `npm run dev` | Inicia o servidor com recarregamento durante o desenvolvimento |
| `npm run lint` | Executa as regras do ESLint para Next.js e TypeScript |
| `npm run typecheck` | Gera os tipos das rotas e valida o TypeScript |
| `npm run build` | Compila e otimiza o projeto para produção |
| `npm start` | Serve o build de produção na máquina local |

## Guia para desenvolvedores

| Documento | Quando consultar |
| --- | --- |
| [Arquitetura e mapa do código](docs/arquitetura.md) | Entender os módulos, as fronteiras entre cliente e servidor e onde fazer cada alteração |
| [API de contato](docs/api-contato.md) | Implementar ou testar o contrato HTTP, a validação e o envio pelo Resend |
| [Operação e implantação](docs/operacao.md) | Configurar ambientes, Vercel, WhatsApp, metadados e entrega de e-mail |
| [Como contribuir](CONTRIBUTING.md) | Preparar mudanças, reproduzir problemas e revisar uma entrega |
| [Relatar uma vulnerabilidade](SECURITY.md) | Entrar em contato com a manutenção por um canal privado |

## Stack

Next.js App Router e TypeScript estruturam a aplicação. Tailwind CSS e tokens em CSS compõem a interface. O FAQ usa um Accordion shadcn/ui adaptado com Radix. Motion e Lucide cuidam das animações e ícones. React Hook Form e Zod validam as entradas com o mesmo esquema usado pela API.

## Autoria

Desenvolvimento e portfólio de **[Enzo Ribas (@oEnzoRibas)](https://github.com/oEnzoRibas)**. A Aurora é uma marca fictícia. Equipe, depoimentos, contatos e fotografias são demonstrativos.
