# Get Icon

[English](README.md)

## Estado e origem

Cópia do projeto upstream [get-icon/geticon](https://github.com/get-icon/geticon), com catálogo, gerador e créditos originais preservados. Código revisado em 01/10/2026. Não apresentado como criação original de Iuri. Plano futuro e contagens do README upstream são históricos, não roadmap pessoal ou números atuais verificados.

## Ideia, processo e arquitetura

Coleção de logos de tecnologias e gerador de Markdown/HTML para listar uma stack. `index.js` funciona em Node ou Deno, lê `settings.json`, `icons.json` e `input.txt`, procura nomes/IDs/aliases sem diferenciar maiúsculas e gera arquivo de saída pelo template. Nomes não encontrados são avisados e ignorados.

`icons/` contém SVGs; `data/` e `scripts/` apoiam manutenção do catálogo. Configuração padrão gera `output.md`, usa ícones de 21px e links para assets upstream. Design pertence aos logos e template de links, não a um dashboard criado neste fork. Não foi encontrado diário pessoal ou planejamento original nos arquivos revisados.

## Uso local

```bash
npm install
npm start
```

Ou, com Deno instalado:

```bash
npm run start:deno
```

Coloque uma tecnologia por linha em `input.txt` e revise `settings.json`. Esses comandos escrevem o arquivo configurado: não o aponte para documento valioso. Nada instalado ou executado nesta atualização. Dependências de manutenção são históricas e exigem revisão antes de reutilizar.

## Testes e limites

Manifest tem comandos de manutenção/check, mas não script de teste dedicado. Nenhum teste executado; sem afirmar cobertura ou aprovação. Verifique aliases, entradas desconhecidas, linhas vazias, caminhos de saída, template e renderização dos SVGs. Não confunda logos usados na documentação com afirmação de parceria ou endosso.

## Capturas

README upstream já contém preview e exemplos, preservados no README em inglês. Não são capturas datadas feitas nesta atualização. Capturas futuras do gerador devem mostrar entrada/saída real em arquivos datados sob `docs/assets/`, sem inventar interface ou resultado.

## Licenças e créditos

Licenças originais preservadas: código SVG de logos sob [CC0](LICENSE), scripts sob [MIT](MIT), com copyright de Tom Chen. Desenhos/logos podem continuar protegidos por copyright e marcas. A declaração MIT no package.json não converte toda a coleção em MIT. Nenhum arquivo de licença foi alterado.

O upstream credita Gil Barbara e colaboradores por logos. Catálogo completo, exemplos, instruções e avisos originais estão no [README em inglês](README.md#upstream-readme-preserved).
