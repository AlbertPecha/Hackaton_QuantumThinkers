# Analitzador de Risc de Fuga i Share of Wallet 🚀

Aquest projecte forma part de la **Hackató Interhack**. L'objectiu és proporcionar una eina d'anàlisi de dades per a l'equip comercial que permeti detectar, de manera ràpida i senzilla, quins clients estan derivant les seves compres a la competència o estan en risc de deixar de comprar.

## 📋 Descripció del Problema
En el sector dental/mèdic, és vital diferenciar entre:
1. **Commodities:** Productes de consum regular on la manca de compra indica una possible fuga (Churn).
2. **Productes Tècnics:** Productes amb un patró més variable.

Aquesta solució se centra en el **Share of Wallet**: comparem el **Potencial teòric** de compra del client vs. les seves **Ventes reals**.

## 🛠️ Com funciona el programa?
El codi realitza tres passos clau:
1. **Unificació:** Creua les dades de vendes amb el catàleg de productes.
2. **Agregació:** Suma les vendes totals per client i família de producte.
3. **Detecció de Gaps:** Identifica aquells clients on la venda real és inferior al 20% del seu potencial estimat, generant una alerta prioritzada per volum de negoci.

## 📁 Estructura del Projecte
L'algoritme espera els següents fitxers a la carpeta arrel:
- `Datasets.xlsx - Ventas.csv`: Històric de transaccions.
- `Datasets.xlsx - Productos.csv`: Catàleg amb jerarquia de famílies.
- `Datasets.xlsx - Potencial.csv`: Estimació de potencial per client/família.

## 🚀 Instal·lació i Ús

1. Clona el repositori:
   ```bash
   git clone [https://github.com/AlbertPecha/Hackaton_QuantumThinkers.git](https://github.com/AlbertPecha/Hackaton_QuantumThinkers.git)
