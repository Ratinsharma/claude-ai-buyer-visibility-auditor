# SEO and AEO operator

Claude skill that audits one site in one niche. It checks whether Google can index and snippet the page, whether that page is actually better than what already ranks, and whether answer engines name and cite you. Then it writes one page brief and a 90-day sequence.

It does not promise a number-one ranking. It will not invent search volume, and it will not recommend a reciprocal link network.

## What changed

The previous skill scored ten pasted answers out of ten and treated `llms.txt` as the way to become visible. Google's own guide says AI Overviews use normal Search, and that Google ignores `llms.txt`. This version follows that.

Official references the skill is required to obey:

- [Creating helpful, reliable, people-first content](https://developers.google.com/search/docs/fundamentals/creating-helpful-content)
- [AI features and your website](https://developers.google.com/search/docs/appearance/ai-features)
- [Guide to optimizing for generative AI features](https://developers.google.com/search/docs/fundamentals/ai-optimization-guide)
- [Spam policies](https://developers.google.com/search/docs/essentials/spam-policies)

## What you get

- A niche defined as real queries, with Search Console data winning over guesses.
- Indexation and snippet gates. Unknown stays unknown.
- A comparison against pages already in the results, only when a results page was actually opened.
- An answer-engine log: named, URL cited, and who was recommended instead, per engine you pasted.
- One brief for the single URL that can win, and only if you have a first-hand fact rivals lack.
- A fixed order: fix the page you already have, then consider a new one, then editorial mentions.

## Install

```bash
npx skills add Ratinsharma/claude-ai-buyer-visibility-auditor
```

Restart Claude Code if needed. Then say: **Audit our SEO and AI visibility.**

Have the site URL ready. A Search Console query export for the last 90 days makes the audit real. Without it, query ideas stay labeled as hypotheses.

## What it will refuse

- A guaranteed rank.
- Commodity articles ("7 tips") as a growth plan.
- Bought or swapped links.
- A claim that uploading `llms.txt` gets you into AI Overviews.

## License

MIT. See [LICENSE](./LICENSE).
