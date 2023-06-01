# CeneoScraperN12
##
| składowa | nazwa | selektor |
| --- | --- | --- |
| opinia | opinion | div.js_product-review |
| identyfikator opinii | opinion_id | ["data-entry-id"] |
| autor | author | span.user-post__author-name |
| rekomendacja | recommendation | span.user-post__author-recomendation > em |
| liczba gwiazdek | score | span.user-post__score-count |
| czy opinia jest potwierdzona zakupem | confirmed | div.review-pz |
| data wystawienia opinii | opinion_date | span.user-post__published > time:nth-child(1)["datetime"] |
| data zakupu produktu | purchase_date | span.user-post__published > time:nth-child(2)["datetime"] |
| ile osób uznało opinię za przydatną | up_votes | span[id^="votes-yes"] |
| ile osób uznało opinię za nieprzydatną | down_votes | span[id^="votes-no"] |
| treść opinii | content | div.user-post__text |
| listę wad | cons | div.review-feature__col:has(> div.review-feature__title--negatives) > div.review-feature__item |
| listę zalet | pros | div.review-feature__col:has(> div.review-feature__title--positives) > div.review-feature__item |
## Wykorzystane biblioteki
* Requests
* BeautifulSoup
* Json
* Os
* Pandas
* Numpy
* Matplotlib
* Requirements