# Analiza-opinii
Celem projektu jest przećwiczenie technik przetwarzania tekstu.

Pobrałam bazę około 40 tys. tweetów na temat nierówności na tle rasowym, głównie skupiłam się na międzynarodowym ruch walczącym o prawa osób czarnoskórych - Black Lives Matter ( BLM ).

Następnie przeanalizowałam jaką opinię mają użytkownicy twittera na ten temat.

Pobrałam wszytskie tweety przy pomocy biblioteki snscrape i utworzyłam DataFrame z nazwą użytkownika, czasem wpisu, liczbą polubień, językiem w jakim jest tweet, miejscem skąd został napisany oraz samym tweetu.

tweets_df = pd.DataFrame(attributes_container, columns=["User", "Date Created", "Number of Likes", "Lang",'Place', "Tweet"])

# 1. Preprocessing
Po pobraniu wszytskich tweetów przefiltrowałam je i skupiłam się tylko na tweetach anglojęzycznych. Zmieniłam także ich indeksy.
