# Lacrei-Sa-de

# 📊 Desafio Técnico – Lacrei Saúde

Justificativa Técnica

- Dados normalizados para evitar redundância
- Separação de entidades garante integridade referencial
- Índices criados para melhorar performance em consultas

 Proposta 1: Tabela de Domínio (plano_saude)
- Vantagem:  Flexível e expansível
-  Desvantagem : Requer JOINs extras

Proposta 2: Enum
- Vantagem:  Mais simples e performático para poucos valores
-  Desvantagem: Pouco flexível para mudanças

Uso de `jsonb`

- Quando usar:
  - Dados personalizados por profissional
  - Campos que não exigem estrutura fixa

- Quando evitar:
  - Filtros por valores internos
  - Relações com integridade referencial
