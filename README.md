# hugo-notice

[![Awesome](https://awesome.re/badge.svg)](https://github.com/budparr/awesome-hugo)

## About


It is a [Hugo](https://gohugo.io) theme component providing a shortcodes





## Usage

1. Add the `hugo-shortcodes` as a submodule to be able to get upstream changes later 

`git submodule add https://github.com/talz26/hugo-shortcodes.git themes/hugo-shortcodes`

2. Add `hugo-shortcodes` as the left-most element of the `theme` list variable in your site's or theme's configuration file `config.yaml` or `config.toml`. Example, with `config.yaml`:
    ```yaml

    theme: ["hugo-shortcodes", "my-theme"]
    ```
    or, with `config.toml`,

    ```toml
    theme = ["hugo-shortcodes, "my-theme"]

3. In your site, use the shortcode, this way: 

```html
{{</* blockquote
  cite="Mark Twain"
  text="The more things are forbidden, the more popular they become."
/*/>}}
```

{{< blockquote
  cite="Mark Twain" text="The more things are forbidden, the more popular they become."
/>}}

With anonymous source:

```html
{{</* blockquote
  text="Obsessed is a word that the lazy use to describe the dedicated."
/*/>}}
```

{{< blockquote
  text="Obsessed is a word that the lazy use to describe the dedicated."
/>}}

With source and citation link:

```html
{{</* blockquote
  citelink="https://style.mla.org/urls-some-practical-advice/"
  cite="Angela Gibson, URLs: Some Practical Advice"
  text="Ensuring the enduring availability and retrievability of a source is not the primary objective of documentation, even though the Internet allows for the retrieval of online works referred to in other online works."
/*/>}}
```

{{< blockquote
  citelink="https://style.mla.org/urls-some-practical-advice/"
  cite="Angela Gibson, URLs: Some Practical Advice"
  text="Ensuring the enduring availability and retrievability of a source is not the primary objective of documentation, even though the Internet allows for the retrieval of online works referred to in other online works."
/>}}

With citation link but no source:

```html
{{</* blockquote
  citelink="https://bitly.is/2mkxskj"
  text="When you create your own Branded Short Domain, you can expect to see up to a 34% increase in CTR when compared to standard bit.ly links."
/*/>}}
```

{{< blockquote
  citelink="https://bitly.is/2mkxskj"
  text="When you create your own Branded Short Domain, you can expect to see up to a 34% increase in CTR when compared to standard bit.ly links."
/>}}

With longer quotations:

```html
{{</* blockquote cite="Erin Cummings" >}}
  At the end of the day, you are solely responsible for your success and your failure. And the sooner you realize that, you accept that, and integrate that into your work ethic, you will start being successful. As long as you blame others for the reason you aren't where you want to be, you will always be a failure.
{{< /blockquote */>}}
```

{{< blockquote cite="Erin Cummings" >}}
  At the end of the day, you are solely responsible for your success and your failure. And the sooner you realize that, you accept that, and integrate that into your work ethic, you will start being successful. As long as you blame others for the reason you aren't where you want to be, you will always be a failure.
{{< /blockquote >}}
