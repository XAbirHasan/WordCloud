# WordCloud
 You can use this for word cloud. I give example english, bangla and hindi. Feel free to use thanks.

*Use google colab for better visual experience.
## details
Word cloud (also known as a tag cloud) is a visual representation of words. Cloud creators are used to highlight popular words and phrases based on frequency and relevance. They provide you with quick and simple visual insights that can lead to more in-depth analyses.

Here I show english, bangla and hindi news article data wordcloud.

## How to use

here you use your dataset.
```
input_path = '/content/dummy_dataset.csv' # your data set
```

test your data language using what_language() method

```
textEnglish = 'my name is abir.'
print(what_language(textbangla))
```

for dataset text split 
```
# use this to split text data.
bangla_article = []
english_article = []
hindi_article = []
l =  len(new_df)
for i in range(0, l):
    the_text = str(the_text_list[i]).translate({ord(i): None for i in '{}'})
    if the_text is not np.nan and len(the_text)>0:
        if detect(the_text) == 'en':
            english_article.append(the_text)
        elif  detect(the_text) == 'bn':
            bangla_article.append(the_text)
        elif  detect(the_text) == 'hi':
            hindi_article.append(the_text)
```

To find word cloud provide your font path and text on wordcloud() method

```
# bangla font path
font_path = '/content/BenSenHandwriting.ttf'
wordcloud(bangla_article, font_path)
```

for resolution change in word cloud use your own height and width

```
wordcloud = WordCloud(font_path=path, width = 3000, height = 2000, colormap='Set2').generate(bidi_text)
```

## Source file
* **[WordCloud](https://github.com/XAbirHasan/WordCloud/blob/master/wordCloud.ipynb)**

## Authors

* **AbirHasan**

Check out my other works [@XAbirHasan](https://github.com/XAbirHasan)

