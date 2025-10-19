# Instruções rápidas — normalizar nomes de mídia e publicar

Este repositório contém páginas HTML com referências a imagens, áudios e vídeos. Alguns arquivos no seu diretório local têm nomes com espaços, acentos ou caracteres que dificultam o funcionamento em hosts estáticos. Os passos abaixo ajudam a normalizar os nomes e a publicar sem usar GitHub.

Passos locais (Windows PowerShell):

1. Abra o PowerShell na pasta do projeto (ex.: c:\Users\user\OneDrive\Documents\Percia-dpwpls).
2. Execute o script para renomear/mover:

```powershell
.\rename_files.ps1
```

3. Abra `galeria.html` num browser local para verificar se todas as imagens/áudios/vídeos carregam.

Publicar sem GitHub:

- Usar um serviço de hospedagem estática como Netlify (arrastar a pasta), Vercel (deploy via CLI), ou um serviço de FTP do seu provedor de hospedagem.
- Você também pode usar serviços como Firebase Hosting ou Azure Static Web Apps.

Observações:
- O script tenta identificar e mover os arquivos mais comuns citados no HTML. Se algum arquivo não for encontrado, ele imprime uma mensagem e você pode renomeá-lo manualmente.
- Faça backup antes de executar o script se tiver dúvidas.
