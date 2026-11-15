# 02. Diagnóstico Técnico e Análise de Causa Raiz (RCA)

## 🎯 Objetivo desta Etapa
Isolar com precisão a origem do defeito — distinguindo falhas de **hardware**, **firmware/BIOS**, **software** ou **operação** — através de testes eliminatórios e evidências técnicas, evitando trocas desnecessárias de componentes.

---

## 🧪 Procedimento de Isolamento (Bancada)

Com a falha de inicialização (`LED DRAM`) confirmada na triagem, segui o fluxo lógico de eliminação:

1. **Teste de Módulos de Memória (Isolamento):**
   * Remoção dos módulos instalados, limpeza preventiva dos contatos e teste individual em cada slot da placa-mãe.
   * *Observação:* O Módulo A inicializou normalmente em todos os slots; o Módulo B impediu o POST em qualquer slot testado.

2. **Validação Cruzada (Cross-Check):**
   * O Módulo B (suspeito) foi testado em uma placa-mãe de referência da bancada.
   * *Observação:* A placa de referência apresentou o mesmo travamento na etapa de memória, confirmando que o defeito acompanha o componente.

3. **Verificação de Firmware e Estabilidade:**
   * Com o Módulo A instalado, acessei o BIOS para checar a versão do firmware, tensões da linha de memória e perfis de clock (XMP/JEDEC).
   * Execução de teste de estresse de memória e sistema por 2 horas para garantir ausência de falhas intermitentes nos slots da placa-mãe.

---

## 📌 Causa Raiz Identificada
* **Classificação:** Falha de Hardware (Defeito de Componente).
* **Causa Raiz:** Falha crítica no circuito integrado de um dos módulos de memória RAM (Módulo B), impedindo a conclusão do autoteste de inicialização (POST). Placa-mãe, processador e demais periféricos íntegros e operacionais.
