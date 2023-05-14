# CeneoScraperN11
## Selektory CSS składowych opinii w serwisie Ceneo.pl

| składowa | nazwa | selektor |
| --- | --- | --- |
| opinia | opinion \/ single opinion | div.js\_product-review |
| identyfikator opinii | opinion\_id | [data-entry-id] |
| autor | author | span.user-post\_\_author-name |
| rekomendacja | recommendation | span.user-post\_\_author-recomendation \> em |
| liczba gwiazdek | score | span.user-post\_\_score-count |
| czy opinia jest potwierdzona zakupem | purchased | div.review-pz |
| data wystawienia opinii | opinion\_date | span.user-post\_\_published \> time:nth-child(1)[datetime] |
| data zakupu produktu | purchase\_date | span.user-post\_\_published \> time:nth-child(2)[datetime] |
| ile osób uznało opinię za przydatną | likes | button.vote-yes \> spanbutton.vote-yes[data-total-vote] |
| ile osób uznało opinię za nieprzydatną | dislikes | button.vote-no \> spanbutton.vote-no[data-total-vote] |
| treść opinii | content | div.user-post\_\_text |
| listę wad | cons | div.review-feature\_\_title--negatives ~ div.review-feature\_\_item |
| listę zalet | pros | div.review-feature\_\_title--positives ~ div.review-feature\_\_item |

## Wykorzystane biblioteki
- Requests
- BeautifulSoup
- Os
- Json
- Pandas
- Matplotlib
- Numpy