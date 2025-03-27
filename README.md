# MAHieroglyphenOCR

Dieses Git-Repository beinhaltet alle relevanten Daten zur Masterarbeit *"Maschinelle Erkennung Altägyptischer Hieroglyphen - Vom Bild zu maschinenlesbarem Text"* von David Konieczny aus dem Jahr 2025.

Es stellt alle Datensätze sowie jeglichen relevanten Programmiercode in Form von Jupyter-Notebooks bereit.

Citation: 
Konieczny, D. (2025). *Maschinelle Erkennung Altägyptischer Hieroglyphen - Vom Bild zu maschinenlesbarem Text*. Masterarbeit, FernUniversität in Hagen.

Bibtex:
```
@mastersthesis{konieczny2025maschinelle,
  author       = {David Konieczny},
  title        = {Maschinelle Erkennung Altägyptischer Hieroglyphen - Vom Bild zu maschinenlesbarem Text},
  year         = {2025},
  month        = mar,
  school       = {FernUniversität in Hagen},
  type         = {Masterarbeit},
}
```

## Abschnitt *analysis*
**Verteilung_Git.ipynb**: 

Führt die Verteilungsanalyse auf Basis der CSV-Datei *Werning_D_A-Hieroglyphs_in_TLA_and_PT-20092021-OpenXML(bearbeitet).csv* (Quelle: Daniel A. Werning, Egyptian Hieroglyphic Signs in the Thesaurus Linguae Aegyptiae and in the Pyramid Texts: Evaluation for an Expansion of the Unicode Set, 29. Sept. 2021, OSF, https://osf.io/ys8hj (CC BY-SA 4.0 Int.)) aus.

**Hieroglyphen_Ranking.csv**: Ranking der Hieroglyphen nach Anzahl in der Aufstellung von Werning.

**klassen_anzahlen_Klassifikator.xlsx**: Ranking der Klassen bzgl. der Summe (SUM) ihrer Beispiele im finalen Datensatz vor Data Augmentation.


## Abschnitt *data*
**unicode_gardinercodes.csv**: Liste der 1072 Gardiner-Codes im Block der Standardhieroglyphen.

**unicode_gardinercodes_kurz.csv**: Gekürzte Version der vorherigen Liste.

**Datensatz_Inschriften**: Sammlung von Bildern von Inschriften/hieroglyphischen Texten (Kap. 4.1).

**Trainingsdatensatz_Segmentierer**: Sammlung von annotierten Bildern von Inschriften/hieroglyphischen Texten für das Training des Segmentierers (Kap. 4.2).

**Testdatensatz_Segmentierer**: Sammlung von annotierten Bildern von Inschriften/hieroglyphischen Texten für das Testing des Segmentierers (Kap. 4.2).

**Datensatz_Fonts**: Teildatensatz für den Klassifikator (Kap. 4.3) mit den Patches, die aus Fonts generiert wurden.

**Annotation_ausgeschnitten**: Teildatensatz für den Klassifikator (Kap. 4.3) mit den Patches, die durch die Annotation der Bilder generiert wurden.

**Manuell_ausgeschnitten**: Teildatensatz für den Klassifikator (Kap. 4.3) mit den Patches, die durch die manuelles Ausschneiden aus dem Wörterbuch von Erman & Grapow generiert wurden.

**Datensatz_Final**: Finaler Datensatz (vor Data Augmentation) für den Klassifikator (Kap. 4.3).



## Abschnitt *src*
**Klassifikator Datensatz und Training.ipynb**:

In Google Colab lauffähiges Jupyter Notebook, das den Code für die Erstellung des Datensatzes für den Klassifikator und für das YOLO-Modelltraining und die anschließende Evaluation enthält. 

