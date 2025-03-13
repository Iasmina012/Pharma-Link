# Pharma-Link

# 1.DB

## Tabele:

### **Farmacie**
| ID_Farmacie | Nume | Adresa | Email | Nr. Telefon | ID_Card |
|------------|------|--------|-------|------------|---------|

### **Medicament**
| ID_Medicament | ID_Categorie | ID_Farmacie | Stoc | Nume | Pret | Cantitate | Data_Expirare | Formula Chimica |
|--------------|-------------|------------|------|------|------|----------|--------------|-----------------|

### **Categorie_Medicament**
| ID_Categorie | Nume | Descriere |
|-------------|------|-----------|

### **Comanda**
| ID_Comanda | Total | Data_Prelucrare | Tip_Plata |
|-----------|-------|----------------|----------|

### **Detalii_Comanda**
| ID_Detalii | ID_Comanda | ID_Medicament | Cantitate | ID_Client | Total |
|-----------|-----------|-------------|----------|---------|-------|

### **Card_Fidelitate**
| ID_Card | Status | Puncte_Fidelitate | Data_Inregistrare |
|--------|--------|------------------|----------------|

### **Client**
| ID_Client | Nume | Adresa | Email | Nr. Telefon | ID_Card |
|-----------|------|--------|-------|------------|---------|

## **Relatii:**
- **O farmacie creeaza mai multe carduri** (1:N)
- **O farmacie are mai multe medicamente** (1:N)
- **O comanda are mai multe medicamente** (1:N)
- **Mai multi clienti pot plasa mai multe comenzi** (N:N)
- **Un client are un card de fidelitate** (1:1)

