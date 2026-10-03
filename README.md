# Simple Port Scanner

Scanner de portas TCP em Python, multi-thread, feito para aprender como funcionam as ligações de rede e a fase de reconhecimento num teste de intrusão.

## Funcionalidades
- Pede o alvo e o intervalo de portas ao utilizador
- Valida os dados introduzidos
- Scan multi-thread (50 threads) para maior velocidade
- Mostra o nome do serviço de cada porta aberta
- Guarda o resultado em `resultado_scan.txt`

## Como usar
1. Instala o Python 3 (ou corre no Google Colab)
2. Corre: `python port_scanner.py`
3. Indica o alvo, a porta inicial e a porta final
  
## Exemplo de resultado

    Porta 22 aberta (ssh)
    Porta 80 aberta (http)
    
## Aviso legal
Usa esta ferramenta apenas em sistemas teus ou com autorização escrita. Alvos seguros para testes: `scanme.nmap.org`, o teu próprio computador e laboratórios como o TryHackMe. Fazer scan a sistemas de terceiros sem autorização é ilegal.

## O que aprendi
- Sockets e ligações TCP
- Threads com `ThreadPoolExecutor`
- Validação de entradas e tratamento de erros

## Próximos passos
- Identificar o serviço real com banner grabbing
- Receber argumentos pela linha de comandos
- Suporte para UDP
