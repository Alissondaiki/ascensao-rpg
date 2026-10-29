# Ascensão — RPG Pessoal (v1.0)

Um mini-RPG de evolução pessoal feito com HTML, CSS e JavaScript puro. Sem conta, backend, API ou assinatura.

## O que já funciona
- XP, níveis e ranks
- Atributos: Inteligência, Força, Disciplina, Energia e Finanças
- Missões diárias e semanais predefinidas
- Criar e excluir missões personalizadas
- Conquistas e histórico
- Sequência de dias ativos
- Salvamento local automático
- Exportar/importar backup JSON
- Layout responsivo para celular
- Manifest e service worker para instalação como PWA e cache offline

## Testar localmente
O jeito mais confiável de testar a instalação PWA é publicar em HTTPS. Para abrir apenas a interface, abra `index.html` no navegador; o salvamento local funciona, mas instalação e modo offline exigem um servidor HTTP/HTTPS.

## Publicar gratuitamente no GitHub Pages
1. Crie ou entre numa conta gratuita em https://github.com/
2. Crie um repositório público, por exemplo `ascensao-rpg`.
3. Envie os quatro arquivos deste pacote para a raiz do repositório: `index.html`, `manifest.json`, `sw.js`, `icon.svg`.
4. No repositório, abra **Settings → Pages**.
5. Em **Build and deployment**, selecione **Deploy from a branch**, branch `main` e pasta `/ (root)`, depois **Save**.
6. Aguarde o link HTTPS gerado em Settings → Pages.
7. Abra esse link no Chrome do Android. No menu ⋮, selecione **Instalar app** ou **Adicionar à tela inicial**.

O GitHub Pages hospeda sites estáticos; não é necessário pagar por servidor para este projeto. Os nomes exatos dos menus podem variar com a interface do GitHub.

## Importante sobre os dados
- O progresso fica no armazenamento local do navegador no aparelho. Ele não sincroniza entre dispositivos.
- Limpar os dados do site/navegador pode apagar o progresso.
- Use **Exportar backup** regularmente e guarde o JSON fora do navegador.
- O sistema é uma primeira versão: a pontuação é local e pode ser alterada no navegador; não existe conta nem validação externa.
- A PWA precisa ser servida por HTTPS (ou localhost) para o service worker e a instalação funcionarem como esperado.

## Personalização futura
É possível adicionar inventário, árvore de habilidades, objetivos mensais, avatares e notificações. Para manter o custo em R$ 0, evitar serviços pagos e APIs com cobrança.
