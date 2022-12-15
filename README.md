
[<img src="https://github-ads.s3.eu-central-1.amazonaws.com/support-ukraine.svg?t=1" />](https://supportukrainenow.org)

# .github

There are 2 methods to fetch records based on specified locale only. These; `whereLocale` and `whereLocales` are methods.

```php
NewsItem::whereLocale('name', 'en')->get(); // Returns all news items with a name in English

NewsItem::whereLocales('name', ['en', 'nl'])->get(); // Returns all news items with a name in English or Dutch
```
If there is no record according to the specified locale, it will return an empty array.
