# witr

> Translate at the command line using Wikipedia's interwiki.

## What does it do?
Have you noticed that when you see a Wikipedia page there's a bunch of languages on the left side? This script tries to find a translation to a term by going to the Wikipedia page thus named and looking up the corresponding translation for your language of choice.

## Usage
`witr [lang_origin] [lang_destination] terms`

## Examples
Try this for English-to-Japanese translations:
`witr en ja Spiderman roller_coaster gnome "Akira Kurosawa"`

```bash
[en] Spiderman         [ja] スパイダーマン
[en] roller_coaster    [ja] ローラーコースター
[en] gnome             [ja] ノーム (妖精)
[en] Akira Kurosawa    [ja] 黒澤明
```

Try this for English-to-Korean translations:
`witr en ko Spiderman roller_coaster kimchi Seoul`

```bash
[en] Spiderman         [ko] 스파이더맨
[en] roller_coaster    [ko] 롤러코스터
[en] kimchi            [ko] 김치
[en] Seoul             [ko] 서울특별시
```

Since it's Wikipedia, you can also use it to find versions of names in others languages. So querying for "Christopher Columbus" in English Wikipedia and looking up the Spanish Wikipedia's equivalent would output "Cristóbal Colón". Try it:
`witr en es "Christopher Columbus"`

## Dependencies
Must have `curl` and `xsel` installed. Try:
`sudo apt-get install curl xsel`

