# Verificação de Segurança com Semgrep e MobSF

Este projeto usa ferramentas de segurança para verificar se o código está seguro e protegido contra vulnerabilidades. As ferramentas que utilizamos são:

## Semgrep (SAST)
O **Semgrep** é uma ferramenta de análise estática de código, o que significa que ela lê o código e encontra possíveis falhas de segurança antes mesmo de o código ser executado. Ele verifica o código e destaca problemas comuns, como padrões de código vulneráveis.

## MobSF (DAST)
O **MobSF** é uma ferramenta de análise dinâmica de segurança para app mobile. Ela testa o código enquanto ele está rodando, simulando ataques reais para encontrar vulnerabilidades que só aparecem quando o código está funcionando.

### Como o workflow funciona:

1. Quando você envia uma alteração para o repositório (push), o workflow de segurança é acionado.
2. **Semgrep** verifica o código em busca de problemas de segurança diretamente no código fonte.
3. **MobSF** testa o código rodando, simulando ataques para encontrar vulnerabilidades.

Este processo garante que nosso código esteja seguro tanto antes quanto depois de ser executado!