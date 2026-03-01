# TOOLS.md — SEO Engine

## File Structure
```
seo/
  keywords.md         # Target keywords + search volume + difficulty
  calendar.md         # Content publishing schedule
  clusters.md         # Topic clusters + internal linking map
  outreach.md         # Link building outreach tracker
  competitors.md      # Competitor analysis
  reports/            # Weekly/monthly performance reports
  content/            # Drafted articles ready for review
```

## Keyword Research Workflow
1. **Seed keywords**: Start from niche + competitor analysis
2. **Expand**: Use web search to find related long-tail queries, "People Also Ask", related searches
3. **Evaluate**: Volume (higher = better), Difficulty (lower = better), Intent (match your monetization)
4. **Cluster**: Group related keywords into topic clusters
5. **Prioritize**: Quick wins first (low difficulty + decent volume + clear intent)

## Content Pipeline
1. Research target keyword + top 10 ranking pages
2. Identify content gaps (what are they missing?)
3. Write outline with H2s mapped to search intent
4. Draft article (1500-3000 words for main articles, 800-1200 for supporting)
5. Add internal links (3-5 per article)
6. Optimize: title tag, meta description, URL slug, image alt tags
7. Save to `seo/content/{slug}.md` for review

## Article Template
```markdown
---
title: {SEO Title - 55-60 chars}
meta_description: {155-160 chars, includes target keyword}
target_keyword: {primary keyword}
secondary_keywords: {2-3 related terms}
word_count_target: {1500-3000}
internal_links: {list 3-5 existing pages to link to}
---

# {H1 - Can differ from title tag}

{Opening paragraph - directly answer the search query}

## {H2 - addresses a sub-topic/question}
...
```

## Outreach Email Template
```
Subject: {Personalized - reference their specific content}

Hey {Name},

I noticed your article on {their topic} — particularly liked {specific detail}.

I just published a {complementary resource type} on {your topic} that covers {angle they're missing}.

Thought it might be a useful addition to your piece for readers who want to {benefit}.

Here's the link: {URL}

Either way, keep up the great work on {their site}.

{Your name}
```

## Link Building Tactics (White Hat Only)
1. **Resource pages**: Find pages that list tools/resources in your niche
2. **Broken link building**: Find broken outbound links on relevant sites, offer your content as replacement
3. **Guest posting**: Write genuinely useful content for relevant sites
4. **Original research**: Publish data/surveys that others will cite
5. **Connectively (formerly HARO)**: Respond to journalist queries for press mentions
