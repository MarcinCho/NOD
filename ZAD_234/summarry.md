### Cel (Objective)

Głównym celem wykorzystania tego zestawu danych jest **stworzenie modelu predykcyjnego zachowań zakupowych klienta (Customer Lifetime Value - CLV)**. Model ten pozwoli zidentyfikować, którzy klienci i jakie kategorie produktów generują największą wartość długoterminową, co umożliwi optymalizację budżetu marketingowego i strategii retencji.

### Wnioski z Analizy Danych (Key Findings from Data Analysis)

1.  **Wzorce Zakupowe (Purchase Patterns):** Analiza rozkładu kwoty zakupu (**Purchase Amount**) oraz częstotliwości (**Frequency**) wykaże, czy większość przychodów pochodzi od dużej liczby małych transakcji, czy od małej liczby klientów o wysokiej wartości (High-Value Customers).
2.  **Relacje Kategoria-Częstotliwość (Category-Frequency Relationship):** Stosunek między **Category** a **Frequency** (jak w Wykresie 3) pomoże zróżnicować produkty będące "zwykłymi zakupami" (wysoka częstotliwość) od tych "specjalnych/jednorazowych" (niska częstotliwość).
3.  **Preferencje Płatności (Payment Preferences):** Zależność między **Payment Method** a **Item Purchased** (jak w Wykresie 4) wskaże, czy pewne metody płatności są silnie skorelowane z wysoką lub niską kwotą transakcji.

---

### Propozycja Wykorzystania (Proposal for Utilization)

Wykorzystać zestaw danych do zbudowania systemu segmentacji klientów w oparciu o dwa kluczowe wskaźniki: **Częstotliwość** i **Średnia Kwota Zakupu (Average Purchase Amount)**.

1.  **Segmentacja RFM (Recency, Frequency, Monetary):** Zestaw danych pozwala na przeprowadzenie podstawowej segmentacji RFM, nawet bez precyzyjnego wskaźnika **Recency** (dostępne jest **Last Purchase (Days)**). Połączymy **Frequency** i **Purchase Amount** by zdefiniować 3 główne segmenty:
    * **Mistrzowie (Champions):** Wysoka `Frequency` i Wysoka `Purchase Amount`.
    * **Wierni (Loyalists):** Wysoka `Frequency` i Średnia/Niska `Purchase Amount`.
    * **Śpiochy (Hibernating):** Niska `Frequency` i Niska `Purchase Amount`.
2.  **Akcje Marketingowe (Targeted Actions):**
    * **Dla Mistrzów:** Oferowanie programów lojalnościowych premium i ekskluzywnych zniżek na nowe produkty w preferowanej **Category**.
    * **Dla Śpiochów:** Użycie **Review Rating** jako wskaźnika niezadowolenia i wysłanie spersonalizowanej kampanii reaktywacyjnej, oferującej zniżkę na **Item Purchased** w sezonie, w którym ostatnio kupowali.

Poprzez takie wykorzystanie, firma może **zwiększyć wskaźnik retencji** i **maksymalizować wartość życiową (CLV)** każdego segmentu klienta.