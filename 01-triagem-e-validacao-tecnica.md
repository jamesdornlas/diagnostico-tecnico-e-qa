# 01. Triagem Inicial e Validação Técnica

## 🎯 Objetivo desta Etapa
Garantir que nenhum equipamento ou chamado avance para análises complexas ou trocas sem antes passar por uma verificação padronizada, separando falhas reais de erros de configuração, incompatibilidade ou relatos imprecisos.

---

## 📋 Cenário de Exemplo (Caso Anonimizado #01)
* **Equipamento:** Desktop Corporativo / Workstation (Linha Modular)
* **Sintoma Reportado pelo Cliente:** *"O equipamento liga, gira os coolers, mas não apresenta imagem no monitor após atualização de sistema e reinicializações."*
* **Histórico:** Produto dentro do período de garantia, sem histórico anterior de retorno.

---

## 🔍 Checklist de Triagem e Inspeção Inicial
Antes de iniciar testes invasivos ou substituição de peças, executo o protocolo padrão de validação:

1. **Inspeção Física e Integridade:**
   * Verificação de lacres de segurança, sinais de impacto físico, oxidação, umidade ou danos nos conectores de vídeo (HDMI/DisplayPort) e alimentação.
   * *Resultado:* Estrutura íntegra, sem indícios de dano físico externo ou mau uso aparente.

2. **Validação do Ambiente e Periféricos:**
   * Teste em bancada homologada utilizando cabos de vídeo, monitor e fonte de alimentação conhecidos como funcionais (padrão *Known Good*).
   * *Resultado:* O sintoma de "sem vídeo" persistiu na bancada, descartando falha nos periféricos do cliente.

3. **Leitura de Sinais de Diagnóstico (POST):**
   * Observação dos LEDs de diagnóstico da placa-mãe (*EZ Debug LED*) e sinais sonoros (*beeps*).
   * *Resultado:* LED indicador de **DRAM** aceso continuamente, travando a sequência de inicialização antes do vídeo.

---

## ✅ Conclusão da Triagem
* **Status:** **Falha Validada (Procedente para Diagnóstico Profundo).**
* **Próximo Passo:** Encaminhar o equipamento para isolamento de componentes e identificação da causa raiz (`02-diagnostico-e-causa-raiz.md`).
