# DNS Blocklist - PDF Converters Blocklist

Lista de bloqueio DNS para AdGuard Home / Pi-hole / dnsmasq que bloqueia sites populares de conversão de PDF online (iLovePDF, SmallPDF, etc.).

## Por que bloquear conversores PDF online?

- Segurança: Evita upload acidental de documentos sensíveis para terceiros
- Produtividade: Impede uso de serviços web desnecessários na rede corporativa/ISP
- Controle: Reduz tráfego para serviços de conversão não autorizados

## Como usar

### 1) Regras personalizadas (AdGuard Home)
No painel do AdGuard Home:
Filtros -> DNS bloqueio -> Regras personalizadas -> cole o conteúdo do blocklist.txt

### 2) Lista externa (recomendado)
Adicione esta URL no AdGuard Home (Listas de bloqueio DNS -> Adicionar -> URL):
https://raw.githubusercontent.com/leonardocassio/dns-blocklist-pdf-converters/master/blocklist.txt

Lista completa:
https://github.com/leonardocassio/dns-blocklist-pdf-converters/blob/master/blocklist.txt

## Manutenção e contribuições

1. Monitoramento: Verifique Query Log do AdGuard para novos domínios
2. Novos sites: Fork -> adicione regra -> Pull Request
3. Formato: Sempre use ||dominio.com^

Exemplo:
||novoconversor.com^

## Autor

Leonardo Cassio (Recife, PE - BR)