# Launchpad — Engineering Boot Camp

A working browser prototype for a three-week engineering onboarding program.

## Run

No installation or API keys required. Open `dist/index.html` in a browser, or run:

```sh
python3 -m http.server 8080 --directory dist
```

Then visit http://localhost:8080.

## Demo walkthrough

1. Start as Maya Chen. Inspect role, skills, learning foundations and graduation passport.
2. Mark API conventions complete in My journey.
3. Open ENG-101 in Task marketplace. Start the quest; optionally choose an eligible partner.
4. Open the quest from My quests. Submit work evidence, AI approach, judgment, verification and learning reflection.
5. In Review desk, confirm individual contribution evidence, optionally verify AI practice, and approve.
6. Return to My journey and Cohort arena to see progress, points and achievements.
7. Switch to the partner: their task still needs their own evidence and review.
8. Use Reset demo to restore the starting state.

## Rules

- Graduate through 3 basic OR 2 intermediate OR 1 expert approved contributions. Mixed paths do not combine.
- Approved basic/intermediate/expert contributions earn 100/175/300 points.
- AI use is optional. Only reviewer-verified AI judgment earns an AI badge. AI usage volume earns no points.
- Pair tasks allow at most 2 learners with separate evidence, approval and credit.
- Prerequisites must be completed before claiming a quest.
- Recommendations use transparent rules: craft 40, team 25, skill overlap up to 25, prerequisite readiness 10. They do not use a live AI model.

## Data and limits

Six fictional profiles and twenty curated Jira-style tasks. All data is synthetic. Workday, Jira and AI vendor integrations are not connected. Browser localStorage saves progress on the same origin. No server database, cross-device synchronization, authentication or real reviewer authorization. Review desk is an explicit demo role switch, not a secure production approval system. Training completion is self-reported. No real work is submitted to company systems.

## Project submission

Include this source in your GitHub repository. Capture screenshots of My journey, marketplace, submission and review. Describe prompts, iterations and learning in your project document, and record the walkthrough in under five minutes. Source repository: https://github.com/sudhajchandran/GenAI

Public working demo: https://engineering-launchpad-bootcamp.tealhawk1.chatgpt.site (no sign-in required).

## Files

- dist/index.html: application shell
- dist/style.css: responsive interface
- dist/app.js: sample data, recommendations and workflow
- tests/rules.cjs: workflow rule checks
