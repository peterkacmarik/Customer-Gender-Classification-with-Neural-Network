# Customer Gender Binary Classification with Neural Network

## Popis

Tento projekt implementuje model neurónovej siete na binárnu klasifikáciu pohlavia zákazníkov na základe rôznych charakteristík, ako sú vek, lokalita a nákupné správanie. Model je vytvorený pomocou PyTorch a zahŕňa predspracovanie dát, trénovanie modelu, vyhodnotenie a vizualizáciu výsledkov.

## Funkcie

- Predspracovanie dát pomocou pandas a scikit-learn
- Vlastný PyTorch Dataset a DataLoader
- Model neurónovej siete s konfigurovateľnou architektúrou
- Trénovacie a validačné cykly s včasným zastavením (early stopping)
- Vizualizácia trénovacích a validačných metrík
- Generovanie náhodných dát pre testovanie modelu

## Požiadavky

- Python 3.7+
- PyTorch
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib

## Inštalácia

1. Naklonujte tento repozitár:
   ```
   git clone https://github.com/peterkacmarik/Customer-Gender-Classification-with-Neural-Network.git
   cd Customer-Gender-Classification-with-Neural-Network
   ```

2. Nainštalujte potrebné balíky:
   ```
   pip install -r requirements.txt
   ```

## Použitie

1. Pripravte vaše dáta:
   - Uistite sa, že vaše dáta sú vo formáte CSV a umiestnite ich do priečinka `dataset`.
   - Očakávaný názov súboru je `sales_data.csv`.

2. Otvorte Jupyter notebook:
   ```
   jupyter notebook
   ```

3. Otvorte súbor `customer_gender_classification.ipynb` v Jupyter rozhraní.

4. Spustite všetky bunky v notebooku. Notebook bude:
   - Načítavať a predspracovávať dáta
   - Rozdeľovať dáta na trénovaciu a testovaciu množinu
   - Trénovať model neurónovej siete
   - Vyhodnocovať výkonnosť modelu
   - Generovať a zobrazovať vizualizácie výsledkov
   - Robiť predikcie na náhodných testovacích dátach

## Architektúra modelu

Model neurónovej siete pozostáva z:
- Vstupnej vrstvy
- Troch skrytých vrstiev s ReLU aktiváciou a batch normalizáciou
- Dropout vrstiev pre regularizáciu
- Výstupnej vrstvy so sigmoid aktiváciou pre binárnu klasifikáciu

## Výsledky

Výkonnosť modelu je vyhodnocovaná pomocou nasledujúcich metrík:
- Presnosť (Accuracy)
- Precíznosť (Precision)
- Návratnosť (Recall)
- F1 skóre

Generované sú vizualizácie zobrazujúce trénovacie a validačné:
- Straty (Loss)
- Presnosť (Accuracy)
- Precíznosť (Precision)
- Návratnosť (Recall)
- F1 skóre
- Rýchlosť učenia (Learning Rate)

## Prispievanie

Príspevky sú vítané! Neváhajte poslať Pull Request.

## Licencia

Tento projekt je licencovaný pod MIT licenciou - pre detaily pozrite súbor [LICENSE](LICENSE).
