# My AI Pulse — MVP Product Requirements Document

**Status:** Approved demo scope

**Date:** July 18, 2026

**Brand:** My AI Pulse — powered by Skilium, the AI Skills Company

## 1. Product in One Sentence

My AI Pulse is a mobile-first, always-on AI companion that separates AI signal from noise, prepares three useful signals and three practical activity choices automatically, then lets visitors explore, complete, and share their daily progress.

## 2. Immediate Goal

Submit a qualifying entry to the AWS Builder Center Always-On Agent Weekend Challenge while creating a public, touchable demonstration of Skilium's practical AI-learning approach.

## 3. Primary User

A busy professional, operator, or manager who wants to keep up with AI but has limited time and needs concise, practical guidance.

## 4. Core User Problem and Product Promise

AI information is abundant, noisy, and difficult to prioritize. Busy professionals cannot easily tell what matters, why it matters, or what to do next.

**Our specialty is separating signal from noise.** My AI Pulse reduces the daily AI information stream to three relevant signals, explains their practical importance, and converts awareness into one useful action.

The product promise is:

> Less AI noise. More useful action.

## 5. Approved MVP Experience

### Agent behavior

1. A scheduled AWS trigger wakes the agent without a user clicking anything.
2. The agent collects public AI/AWS source items that do not require external API keys.
3. Deterministic rules filter and rank relevant items.
4. Amazon Bedrock Nova Micro converts the strongest items into three concise signals and three activity choices: Quick Win, Apply It, and Scale It.
5. The result is stored once and reused for all visitors.
6. The public application displays the latest prepared pulse.

### Visitor interactions

- Browse and expand three daily signals.
- Read why each signal matters.
- Choose from three practical activities and reusable prompts.
- Copy the prompt.
- Complete one, two, or all three activities.
- See progress update on the current device.
- Copy share-ready progress text for LinkedIn or WhatsApp.
- Return later to see the newest agent-generated pulse.

## 6. Screen Structure

| Section | Purpose | Main Interaction |
|---|---|---|
| Header | Establish My AI Pulse, Skilium, and AWS credibility | See last refresh time and autonomous status |
| Today | Show three ranked AI signals | Tap cards to expand details |
| Try | Turn awareness into action | Copy prompt and mark complete |
| Pulse | Make progress visible | View completion state and share text |
| About | Explain the agent and challenge | View architecture/repository links |

## 7. MVP Success Criteria

| Measure | Target |
|---|---:|
| Time to understand product | Under 60 seconds |
| Daily signals displayed | 3 |
| Practical activities displayed | 3 |
| Manual action required to generate pulse | 0 |
| External API keys required | 0 |
| Bedrock calls per scheduled run | 1 maximum |
| User login required | No |
| Mobile usability | Works at 360 px width and above |
| Public repository | Available and documented |
| AWS challenge article | 500+ words with all required sections |

## 8. Explicitly Deferred

The following are not part of the challenge MVP:

- User accounts and authentication.
- Server-side personal profiles.
- Private notes or My Space.
- Email, SMS, or push notifications.
- Cross-device synchronization.
- Full adoption scoring.
- Admin dashboard.
- Native mobile applications.
- Paid subscriptions.
- Multiple personalized content feeds.

These may be considered after challenge submission and user feedback.

## 9. Privacy and Cost Rules

- Completion state stays in browser storage on the visitor's device.
- No sensitive personal data is required.
- Public feed content is treated as untrusted input and constrained before model use.
- The generated daily result is cached so visitors do not trigger new model calls.
- Prompts and outputs are short and structured.
- The agent runs on a limited schedule rather than continuously.
- AWS cost and usage protections must be configured before deployment.

## 10. Definition of Done

The MVP is done when the scheduled agent runs without a button click, saves a valid daily pulse, the public mobile interface loads and supports every approved interaction, the repository explains how it works, testing evidence is captured, and the Builder Center article is published with the required public link.
