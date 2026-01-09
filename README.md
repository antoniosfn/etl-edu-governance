# 📊 Pipeline de Processamento Professor x Competência x Subárea (via Google Colab)

A pipeline executa a integração, validação e geração de combinações entre Professores, Competências e Subáreas, a partir de arquivos estruturados enviados em formato `.zip`.

O processamento é automático, compatível com Google Colab e suporta múltiplos segmentos (ex: Cidades, Energia, TICs, Saúde), um .zip para cada segmento.

**IMPORTANTE:** Utilize o arquivo "EXEMPLO.zip" presente na pasta como referência absoluta para nomeação dos arquivos e padronização dos nomes das colunas. Qualquer divergência em relação a essa nomenclatura, seja no nome dos arquivos ou nas colunas, inviabiliza o processamento do pipeline, resultando em erros ou descarte de dados.

---

## 🚀 Visão Geral do Pipeline

O pipeline segue o modelo **ETL**:

1. **Extract**  
   - Upload de um ou mais arquivos `.zip`
   - Extração automática do conteúdo

2. **Validate**  
   - Validação de Professores
   - Validação de Competências
   - Validação de Subáreas

3. **Transform**  
   - Normalização de nomes
   - Unpivot das subáreas
   - Geração das combinações válidas

4. **Load / Output**  
   - Arquivo `.xlsx`
   - Arquivo `.csv`
   - Script `.sql`
   - Relatório `.txt`
