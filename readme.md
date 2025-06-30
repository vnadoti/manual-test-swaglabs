# Plano de Teste para SwagLabs
![logo](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/swag-labs.png)

## Introdução

Este documento descreve o plano de testes manuais e automação para o Swag Labs, um aplicativo web para compras.

## 1. 📄 Escopo

### Escopo e Objetivos
Este plano de teste abrange o teste das principais funcionalidades  SwagLabs:

Explorar livremente o sistema de e-commerce para identificar comportamentos inesperados, verificar funcionalidades principais, analisar aspectos de UI/UX, segurança e usabilidade, além de levantar possíveis requisitos para testes manuais futuros.

> **Nota:** Este teste exploratório visa compreender o comportamento da aplicação sem roteiro fixo, permitindo avaliar a experiência do usuário, validar funcionalidades e descobrir possíveis falhas não documentadas.

## 2. 🔍Abordagem de Testes

### Testes Manuais (100%)
- Testes exploratórios para entender o comportamento do aplicativo
- Testes de UI/UX para verificar os elementos da interface.
- Testes de usabilidade para garantir fluxos de trabalho eficientes para o usuário.
- Verificação de mensagens de erro e validação.

## 3. 💻 Ambiente de teste
O ambiente de teste para testes é o seguinte:

- Sistema operacional: Windows 11 
- Navegador: Google Chrome Versão 138.0.7204.50 (Compilação oficial) (64 bits)

## 4. 📑Casos de Testes

As Casos de testes estão disponíveis no arquivo
- `casos-teste.md`

## 5. Avaliação e priorização de riscos

### Estratégia de Priorização de Testes
1. **Testes de Caminho Crítico** - Foco nos fluxos de usuários que impactam a funcionalidade principal
2. **Testes de Alto Risco** - Priorização de testes em áreas de alto risco
3. **Testes de Casos Extremos** - Abordagem de cenários incomuns, se o tempo permitir

## 6. Procedimento de Relatório de Defeitos

### Modelo de Relatório de Defeito
Cada relatório de defeito deve incluir:
- **ID**: Identificador único (ex.: BUG-001)
- **Título**: Breve descrição do problema
- **Descrição**: Explicação detalhada do problema
- **Etapas para Reproduzir**: Etapas numeradas para replicar o problema
- **Comportamento Esperado**: O que deve acontecer
- **Comportamento Obtido**: O que realmente acontece
- **Ambiente**: Navegador, Sistema Operacional, tamanho da tela, etc.
- **Capturas de Tela/Vídeos**: Evidência visual do problema
- **Severidade**: Crítica, Alta, Média, Baixa
- **Prioridade**: Alta, Média, Baixa

### 🚨Definições de Severidade
- **Crítica**: Travamento do aplicativo, perda de dados, violação de segurança
- **Alta**: Funcionalidade principal quebrada, sem solução alternativa
- **Média**: Problema de funcionalidade com solução alternativa disponível
- **Baixa**: Problema menor, problema visual

### ⏰Definições de Prioridade
- **Alta**: Deve ser corrigida imediatamente
- **Média**: Deve ser corrigida na próxima versão
- **Baixa**: Pode ser corrigida quando o tempo permitir

## 7. Sobre
📅 **Data de Execução:** Julho de 2025  
🧪 **Tipo de Teste:** Manual  
👤**Testador**: Victor Nadoti
🧠 **Base:** Casos de teste previamente documentados
🌐 **Sistema Testado:** SwagLabs