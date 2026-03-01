# TOOLS.md — Sales Machine

## Sales Pipeline Workflow

### Daily Process
1. **Lead Review** → Check `leads/new/` for inbound leads
2. **Qualify** → Research + BANT assessment → Move to `leads/qualified/`
3. **Outreach** → Send first touch email, log in `calls/outreach-log.md`
4. **Follow-up** → Check `pipeline/active.md` for stale conversations
5. **Update** → Log all activities in daily activity tracker

### File Structure
```
sales/
  pipeline/
    active.md         # Current deals in progress
    closed-won.md     # Victory log with deal details
    closed-lost.md    # Loss analysis for pattern spotting
  leads/
    new/              # Incoming leads to process
    qualified/        # Passed BANT, ready for outreach
    nurture/          # Long-term prospects
  calls/
    outreach-log.md   # Daily call & email activity
    meeting-notes/    # Individual prospect meeting notes
  templates/
    cold-email/       # Tested email sequences
    objection-responses.md  # Common objections + proven responses
  reports/
    weekly-pipeline.md     # Pipeline health & metrics
    conversion-rates.md    # Lead → meeting → close analytics
```

## Email Templates

### Cold Outreach Sequence
**Email 1: Research + Value**
```
Subject: {Company} + {Pain Point} question

{Name},

Saw {specific company update/news/achievement}. 

{Related pain point based on their industry/role} is something we help {similar companies} solve.

Worth a 15-min conversation?

{Your name}
```

**Email 2: Case Study (3 days later)**
```
Subject: How {Similar Company} solved {Problem}

{Name},

Following up on {previous email topic}.

{Similar Company} had the same challenge and saw {specific result} after implementing our solution.

5-minute call to discuss if it makes sense for {Their Company}?

{Your name}
```

### Objection Response Library
| Objection | Response Framework |
|-----------|-------------------|
| "Too expensive" | "Understand budget is important. What range were you thinking?" |
| "Need to think about it" | "Of course. What specific aspects need consideration?" |
| "Not the right time" | "When would be a better time to revisit this?" |
| "Need approval" | "Who else would be part of that decision?" |

## Pipeline Management

### Deal Stages
1. **Lead** → Initial contact made
2. **Qualified** → BANT confirmed, pain point identified
3. **Demo** → Solution presented, next steps agreed
4. **Proposal** → Pricing sent, under review
5. **Negotiation** → Terms being finalized
6. **Closed-Won** → Contract signed
7. **Closed-Lost** → Deal dead, reason logged

### Daily Metrics to Track
- New leads processed
- Calls made / emails sent
- Meetings scheduled
- Proposals sent
- Deals closed
- Pipeline value by stage

## Research Sources
- **Company**: Website, LinkedIn company page, recent news
- **Contact**: LinkedIn profile, recent posts, mutual connections
- **Industry**: Recent industry reports, competitor analysis
- **Pain Points**: Common challenges in their role/industry

## Follow-up Cadence
- **Day 0**: Initial outreach
- **Day 3**: Value-add follow-up
- **Day 7**: Different angle/case study
- **Day 14**: Helpful resource
- **Day 21**: Final attempt + break-up email
- **Day 90**: Quarterly check-in (nurture sequence)