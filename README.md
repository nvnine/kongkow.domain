## How to get one?

1. Star and [fork](https://github.com/KongkowITPekanbaru/kongkow-domains/fork) this repository
2. Add a new file called `your-subdomain-name.kongkow.space.json` in the `./domains` folder to register `your-subdomain-name` subdomain
3. Edit it (below is just an **example**, provide a **valid** JSON file with your needs; format you can [check here](https://jsonlint.com/)):

```json5
{
  "$schema": "../schemas/domain.schema.json",
  "description": "My personal project", // what is it?
  "domain": "kongkow.space",
  "subdomain": "your-subdomain-name",
  "owner": {
    "repo": "https://github.com/user/repo", // URL to the target repository or your GitHub account
    "email": "my@email.com" // optional
  },
  "record": {
    "CNAME": "user.github.io.",
    //"TXT": ["..."],
    //"A": ["127.0.0.1"],
    //"AAAA": ["::1"],
    //"NS": ["..."],
  },
  "proxy": false // disable CF proxy, true by default
}
```

4. Your pull request will be reviewed and merged. Please, don't ignore the PR checklist (your PR will be ignored if you ignore this requirement). _Make sure to keep an eye on it in case we need you to make any changes!_
5. After the pull request is merged, please allow up to 24 hours for the changes to propagate _(usually, it takes 5..15 minutes)_
6. Enjoy your new domain!

> Domains, used for illegal purposes will be removed and permanently banned. Please, provide a clear description of your resource in the PR.
## If you don't know...

- What is GitHub pages and how to set up a custom domain, read the [docs here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- The difference between `A`, `CNAME`, and other record types, the article on Wikipedia [is here](https://en.wikipedia.org/wiki/List_of_DNS_record_types)
