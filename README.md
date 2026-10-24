# Radar Night PWA — MVP 0.1

Protótipo instalável para Android. Interface, mapa, localização sob permissão, agenda de demonstração e relatos locais funcionam no navegador.

## Rodar

É necessário servir por HTTPS ou localhost (não abrir o HTML diretamente como arquivo). Em um computador com Python:

```bash
python -m http.server 8080
```

Acesse `http://localhost:8080` no computador ou publique os arquivos em um host HTTPS. No Android/Chrome, abra o endereço e use **Instalar app** ou menu ⋮ → **Adicionar à tela inicial**.

## Limitações desta versão

- Eventos e locais são dados fictícios de demonstração; confirme tudo antes de sair para trabalhar.
- Mapa e tiles precisam de internet.
- GPS pede permissão do navegador e só centraliza o mapa no aparelho.
- Relatos são guardados apenas na memória desta sessão e não são enviados a outros motoristas.
- A tela de rádio é uma demonstração; o teste de microfone só verifica a permissão local. Rádio walkie-talkie real requer backend de sinalização e mídia (por exemplo WebRTC com serviço de sinalização), autenticação, canais e controles de abuso.
- Não existe feed real de casas/eventos nem previsão de público conectada ainda.
