# TOOLS.md — Intelligence Operations

## Research Workflow

### Daily Intelligence Cycle
1. **Source monitoring** → Scan key sources for new developments
2. **Signal detection** → Flag unusual patterns, sentiment shifts, news
3. **Verification** → Cross-check claims, validate sources, fact-check
4. **Analysis** → Synthesize findings, identify implications
5. **Report generation** → Package insights for stakeholder consumption

### File Structure
```
research/
  active/
    current-projects.md    # Ongoing research assignments
    monitoring-list.md     # Sources and topics being tracked
  reports/
    weekly-digest.md       # Key developments and trends
    deep-dives/            # Comprehensive analysis on specific topics
    competitive-intel/     # Competitor analysis and updates
    market-research/       # Industry trends and sizing studies
  sources/
    primary-contacts.md    # Industry insiders, expert network
    data-vendors.md        # Subscription services, APIs, feeds
    monitoring-feeds.md    # RSS, alerts, automated sources
  methodology/
    research-templates.md  # Standard analysis frameworks
    source-validation.md   # Credibility assessment criteria
    confidence-scoring.md  # How to rate finding reliability
```

## Research Templates

### Market Analysis Framework
```markdown
# [Market/Industry] Research Brief

## Executive Summary
[2-3 sentences: key findings and implications]

## Market Size & Growth
- **Current market size**: $X billion (Source, Date)
- **Growth rate**: X% CAGR (Source, Date)
- **Key growth drivers**: [List top 3]

## Competitive Landscape
| Company | Market Share | Key Differentiator |
|---------|--------------|-------------------|
| | | |

## Key Trends
1. **[Trend Name]** (Confidence: High/Med/Low)
   - Evidence: [Supporting data]
   - Implications: [What it means]

## Risks & Opportunities
- **Opportunities**: [List with rationale]
- **Threats**: [List with likelihood]

## Data Gaps & Next Steps
- [ ] [What information is still needed]
- [ ] [Recommended follow-up research]

## Sources
1. [Source name, URL, access date]
2. [Source name, URL, access date]
```

### Competitive Intelligence Template
```markdown
# [Company] Competitive Profile

## Company Overview
- **Founded**: [Year]
- **Revenue**: $X (Year, Source)
- **Employees**: [Count] (Date, Source)
- **Funding**: $X raised (Date, Source)

## Product Analysis
- **Core offering**: [Description]
- **Key features**: [Unique capabilities]
- **Pricing model**: [How they charge]
- **Target customer**: [ICP description]

## Recent Developments
- **Product launches**: [List recent releases]
- **Partnerships**: [Key alliances announced]
- **Personnel changes**: [Leadership hires/departures]
- **Funding rounds**: [Recent investments]

## Strengths vs. Weaknesses
| Strengths | Weaknesses |
|-----------|------------|
| | |

## Strategic Assessment
- **Market position**: [Where they sit competitively]
- **Growth trajectory**: [Direction and speed]
- **Threats to us**: [How they compete with us]
- **Opportunities**: [Ways to compete with them]

## Intelligence Gaps
- [ ] [What we don't know but should]

**Last Updated**: [Date]
**Analyst**: [Your name]
```

## Source Management

### Primary Sources (Tier 1)
- **Company filings**: 10-K, 10-Q, 8-K, earnings transcripts
- **Official statements**: Press releases, investor presentations
- **Regulatory data**: SEC filings, patent applications, clinical trials
- **Direct contacts**: Industry insiders, former employees, customers

### Secondary Sources (Tier 2)
- **Industry reports**: Gartner, IDC, McKinsey, PwC
- **Financial analysis**: Analyst reports, investment research
- **Academic research**: Peer-reviewed studies, university reports
- **Trade publications**: Industry magazines, professional associations

### Tertiary Sources (Tier 3)
- **News media**: WSJ, FT, Reuters, industry news sites
- **Social intelligence**: Twitter, LinkedIn, Reddit, Discord
- **Data aggregators**: Crunchbase, PitchBook, CB Insights
- **Web monitoring**: Company blogs, job postings, patent filings

## Data Validation Checklist

### Source Credibility
- [ ] **Author expertise**: Relevant experience and credentials?
- [ ] **Publication reputation**: Known for accuracy and objectivity?
- [ ] **Recency**: How current is this information?
- [ ] **Primary vs. secondary**: Original research or citing others?

### Data Quality
- [ ] **Sample size**: Large enough to be meaningful?
- [ ] **Methodology**: Clear and appropriate approach?
- [ ] **Bias indicators**: Any conflicts of interest or agenda?
- [ ] **Corroboration**: Other sources confirm these findings?

## Monitoring & Alerts Setup

### Daily Monitoring Sources
- **Google Alerts**: [Key terms for your industry/companies]
- **RSS Feeds**: Industry publications, company blogs
- **Social listening**: Twitter lists, LinkedIn follows
- **News wires**: Reuters, Bloomberg, AP for breaking news

### Weekly Deep Dives
- **Earnings releases**: Quarterly results and guidance
- **Regulatory filings**: New patents, SEC documents
- **Industry surveys**: Customer satisfaction, market research
- **Competitor analysis**: Product updates, pricing changes

### Alert Triggers
- **Stock movements**: >10% daily change in key companies
- **Volume spikes**: Unusual trading activity
- **News sentiment**: Negative coverage of key players
- **Regulatory changes**: New rules affecting your industry
- **Personnel moves**: Key executive changes at competitors