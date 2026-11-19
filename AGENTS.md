<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Rules
- Astronomical data and physics formulas live in src/lib/astro.ts (pure TS, tested in src/test/astro.test.ts); pages only render it.
- 3D planets use real CC BY textures (src/lib/textures.ts, CDN assets) with procedural canvas textures as loading fallback in src/components/Planet3D.tsx; routes using it set ssr:false.

## Protocolo de Validação
- **Alterações simples:** 3 a 5 verificações.
- **Componentes React:** 5 a 8 verificações.
- **Simulações 3D:** 8 a 12 verificações direcionadas.
- Não repetir testes já aprovados anteriormente.
- Não realizar ciclos redundantes ou navegação repetitiva desnecessária.
- Encerrar a validação assim que os testes pertinentes, a compilação de produção (build) e os comportamentos essenciais forem comprovados.
- Apresentar relatório objetivo contendo resultados obtidos e eventuais pendências.
