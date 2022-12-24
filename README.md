## How to get one?

1. Star and [Fork](https://github.com/nvnine/kongkow.domain/fork) this repository
2. Add a new file called `example.kongkow.space.json` in the `./domains` folder to register `example` subdomain
3. Edit it (below is just an **example**, provide a **valid** JSON file with your needs; format you can [check here](https://jsonlint.com/)):

```json5
{
  "$schema": "../schemas/domain.schema.json",

  "description": "Project Description", // what is it?

  "domain": "kongkow.space",
  "subdomain": "example",

  "owner": {
    "repo": "https://github.com/username/repo",
    "email": "hello@example.com"
  },

  "record": {
    "A": ["1.1.1.1", "1.0.0.1"],
    "AAAA": ["::1", "::2"],
    "CNAME": "example.com.",
    "MX": ["mx1.example.com.", "mx2.example.com."],
    "NS": ["ns1.example.com.", "ns2.example.com."],
    "TXT": ["example_verification=1234567890"]
  },

  "proxy": false // disable CF proxy, true by default
}
```

4. Your pull request will be reviewed and merged. Please, don't ignore the pull requestchecklist. If you ignore the checklist, your pull request will be ignored too. _Make sure to keep an eye on it in case we need you to make any changes!_
5. After the pull request is merged, please allow up to 24 hours for the changes to propagate _(usually, it takes 5..15 minutes)_
6. Enjoy your new domain!

*Domains used for illegal purposes will be removed and permanently banned. Please, provide a clear description of your resource in the pull request.*
