# Data Science Challenge: SignalDesk Workflow 

## Track Chosen
Track A: Fictional Domain Packet

## What I Built: 
A Jupyter notebook analyzing 7 days of workflow usage data to identify which AI-assisted workflows are healthy and what needs immediate investigation.

## Who It Is For: 
Product team deciding where to focus after launching new prompts and review policies.

## Data Or Source Used: 
`product_usage_events.csv` 

## Assumptions I Made
- User rating is the most reliable quality signal (more trustworthy than model confidence)
- The Aug 7 review policy change caused the Support Reply crash
- Flagged outputs correlate with quality issues 

## Data Issues Or Caveats I Noticed
- 2 missing user ratings (dropped during cleaning)
- 1 duplicate row on Aug 5 (removed)
- Team name casing inconsistency (fixed)
- Model confidence doesn't match user satisfaction (Aug 7: 91% confidence but 2.1 rating)

## What I Would Do Next With More Time
1. Find out what changed in the Aug 7 policy and why it broke Support Reply
2. Set up weekly alerts to catch problems like Aug 7 immediately
3. Test new policies on a small group first before rolling out to everyone
