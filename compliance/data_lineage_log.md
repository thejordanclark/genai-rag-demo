# Data Lineage Log

## Purpose
Track all document ingestion and query operations for audit trail.

## Document Ingestion Log

| Timestamp | Document | Chunks | Embeddings | Status | Operator |
|-----------|----------|--------|------------|--------|----------|
| 2024-01-22 10:00 | clinical_protocol_summary.txt | 12 | 12 | Success | System |
| 2024-01-22 10:00 | adverse_event_guidelines.txt | 15 | 15 | Success | System |
| 2024-01-22 10:00 | patient_eligibility_criteria.txt | 18 | 18 | Success | System |
| 2024-01-22 10:00 | data_validation_rules.txt | 25 | 25 | Success | System |

## Query Log

| Timestamp | Query | Results | Sources | User |
|-----------|-------|---------|---------|------|
| 2024-01-22 10:15 | "What are the inclusion criteria?" | 3 | patient_eligibility_criteria.txt | Demo User |
