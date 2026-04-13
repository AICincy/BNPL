# Reddit Consumer Intelligence: Legal and Regulatory Signals (SWARM-BETA)

```
data_source_id: REDDIT-BETA-001
swarm: SWARM-BETA
subagents_served: [SA-REGZ, SA-REGE, SA-CFPB, SA-FTC]
source: r/cashadvanceapps
extraction_date: 2026-04-12
claim_tag_default: OBS
source_reliability: CONSUMER_SELF_REPORT
```

---

## Signal Summary

```yaml
signal_summary:
  legal_action_mentions: 114
  credit_reporting_mentions: 119
  tipping_fee_mentions: 31
  key_patterns:
    - pattern: Mass arbitration campaigns actively recruiting EWA users (Earnin, Dave, Brigit, Empower, MoneyLion)
    - pattern: Consumer awareness of CFPB complaint mechanism is high in this community
    - pattern: Credit reporting by EWA providers perceived as punitive (reporting negative but not positive)
    - pattern: Tipping model legality questioned by consumers (Earnin's 'optional' tips)
    - pattern: Users report successful CFPB complaints leading to balance forgiveness
    - pattern: Subscription fee structure challenged as deceptive (fee for access vs. fee for service)
  enforcement_relevant_signals:
    - signal: Multiple consumers report identical Dave double-debit pattern (systematic, not isolated)
    - signal: Brigit consistently clears balances post-ACH-revocation (possible voluntary compliance pattern)
    - signal: Mass arbitration filings increasing (consumer awareness of legal options growing)
    - signal: Ex-employee post confirms internal practices at unnamed payday lender
```

---

## Curated Posts

```yaml
posts:
- entry_id: REDDIT-0146
  title: "Several cash advance apps are getting sued and you may be owed money"
  date: 2026-02-22
  score: 155
  type: post
  providers: [Albert, Dave, Earnin, FloatMe, Klover, MoneyLion, Payactiv]
  topics: [BANK_ACCOUNT, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rc0ky2/several_cash_advance_apps_are_getting_sued_and/
  text: |
    If you've used any of these apps in the past few years and paid fees for instant transfers or got hit with a subscription you couldn't cancel, lawyers are signing up users right now for mass arbitration cases. Completely free, no court, no calls with a lawyer. You just fill out a form and wait.
    
    Here are the ones where you can actually sign up today:
    
    * **Current** – Accused of calling its advances simple "paycheck advances" while allegedly charging fees that work out to illegal interest rates. ...[truncated]

- entry_id: REDDIT-0147
  title: "My journey with cash advances comes to an end."
  date: 2025-07-17
  score: 100
  type: post
  providers: [Albert, Brigit, Cleo, Dave, Earnin, Empower, Klover]
  topics: [DEBT_CYCLE, LEGAL_ACTION, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1m27hfb/my_journey_with_cash_advances_comes_to_an_end/
  text: |
    I have been stuck in the never ending cycle of cash advance apps for roughly two years. Two years ago I had a rough month and needed a few bucks to get through. I started with Earnin.. there became my "addiction." It was so easy, and so harmless. I borrowed $200 and paid it back.. well, then I thought maybe I could get more.. and so I spiraled. Empower, Dave, Money Lion, Cleo, Brigit, Klover & Albert. It was wildly out of control. But I always seemed to manage. But the past year, I've made more ...[truncated]

- entry_id: REDDIT-0148
  title: "FAQ: How to Revoke ACH Authorization from Cash Advance Apps"
  date: 2025-05-20
  score: 67
  type: post
  providers: [Brigit, Chime, Cleo, Dave, Earnin, Empower, FloatMe, MoneyLion, Possible Finance]
  topics: [ACH_REVOCATION, BANK_ACCOUNT, COLLECTIONS, CREDIT_REPORTING, DEBT_CYCLE, LEGAL_ACTION, PROVIDER_COMPLAINT, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1krhivj/faq_how_to_revoke_ach_authorization_from_cash/
  text: |
    **1. What does it mean to revoke ACH authorization, and is it legal?**
    
    When you use a cash advance app like Earnin, Brigit, or Dave, you give the app permission to pull money from your bank account using something called ACH authorization. ACH stands for Automated Clearing House. It’s the system that moves money electronically between banks. This is how the app collects repayment automatically on your payday.
    
    Revoking ACH authorization means you're taking back that permission. And yes, it’s 10...[truncated]

- entry_id: REDDIT-0149
  title: "Cash advance breakdown November"
  date: 2024-11-30
  score: 41
  type: post
  providers: [Brigit, Dave, Earnin, Empower, Klover, Possible Finance]
  topics: [SUBSCRIPTION_FEES, TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1h3iqxb/cash_advance_breakdown_november/
  text: |
    Hi all. I wanted to share a breakdown of cash advances I was able to receive from 9 different cash advance apps this past week. I wanted to test as many cash advance apps out as possible to determine the highest amount of advances I was able to receive and what other fees/subscriptions are associated with each app.
    
    Listed below are the apps and total cash advance dollar amounts received + any transfer or subscription fees associated with each, starting with the highest amount offered. Hopefully...[truncated]

- entry_id: REDDIT-0150
  title: "Finally Free"
  date: 2026-02-27
  score: 36
  type: post
  topics: [BANK_ACCOUNT, DEBT_CYCLE, LEGAL_ACTION, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rftt93/finally_free/
  text: |
    After almost two years of NEVER fully seeing my check and having to rely on the cycle of cash advances, I am FREE! My job payed out from a lawsuit and after every app took back their repayment, I revoked access, unlinked my bank card, and deleted them. While I understand that these apps can be “helpful”, they can also turn quite predatory. An $100 advance turns into a $300 advance, and judging on how deep, you probably downloaded more than one. Now you owe if not HALF your paycheck, the entirety...[truncated]

- entry_id: REDDIT-0151
  title: "Brigit lawsuit. Did anyone else receive this email??"
  date: 2024-11-09
  score: 33
  type: post
  providers: [Brigit]
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1gne1im/brigit_lawsuit_did_anyone_else_receive_this_email/

- entry_id: REDDIT-0152
  title: "Class action lawsuits against cash advance apps taking claims"
  date: 2026-03-26
  score: 32
  type: post
  providers: [FloatMe, Klover, MoneyLion]
  topics: [BANK_ACCOUNT, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1s4jo5k/class_action_lawsuits_against_cash_advance_apps/
  text: |
    MoneyLion, Klover, Grant, FloatMe, CreditGenie and more. Most are looking at advances in the last two years, YOU DO NEED EVIDENCE. Cashapp if you have paid to instantly transfer funds to your bank account and it took more than an hour. The claims are easy to fill out and are easily found on Google.

- entry_id: REDDIT-0153
  title: "Dave Changed the Rules—and You Might Not Like Them"
  date: 2025-05-16
  score: 27
  type: post
  providers: [Dave]
  topics: [ACH_REVOCATION, BANK_ACCOUNT, COLLECTIONS, CREDIT_REPORTING, DEBT_CYCLE, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ko9dqm/dave_changed_the_rulesand_you_might_not_like_them/
  text: |
    Getting out of the cash advance debt cycle by revoking ACH authorization has been the hot topic on this sub, and that's awesome!  It's great to see people reclaim their paycheck.  
    
    As many other posts detail, **most** cash advance apps have pretty limited consequences if you don't repay them.  You won't be able to borrow again, but they explicitly waive their rights to report you to a credit bureau, refer you to a collections agency or sue.  
    
    However, Dave is different, and they’ve recently up...[truncated]

- entry_id: REDDIT-0154
  title: "Review of FrontPay"
  date: 2024-10-25
  score: 25
  type: post
  topics: [BANK_ACCOUNT, TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1gc5i9w/review_of_frontpay/
  text: |
    Hey so I came across a post here for FrontPay and gave it a try. There is no app but the website worked. It was easy to sign up and I got approved after connecting my bank account. The funds arrived in about 6 hours and I did not have to tip. I was looking for a new cash advance app so this worked for me

- entry_id: REDDIT-0155
  title: "How to borrow money for free"
  date: 2023-11-28
  score: 23
  type: post
  providers: [Brigit, Dave, Earnin, MoneyLion]
  topics: [BANK_ACCOUNT, CREDIT_REPORTING, SUBSCRIPTION_FEES, TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1866k2u/how_to_borrow_money_for_free/
  text: |
    I've spent a ton of time reading through the T&Cs of borrowing apps like Brigit, Dave, Earnin, and MoneyLion.  Almost every one of them quietly lays out how you can borrow up to $250 or $500 (depending on the app) at zero cost.
    
    None of these apps charge interest (or performa credit check), but the cost of using them can of course add up - [the average cost of borrowing $100 from these apps is $19.08]([URL] and you usually have to repay them within a week or two, which still puts the APR well in...[truncated]

- entry_id: REDDIT-0156
  title: "Beware of Dave Technologies  Unauthorized ACH Withdrawal, Privacy Breach, and Ongoing Bad Faith"
  date: 2025-07-01
  score: 22
  type: post
  providers: [Dave]
  topics: [BANK_ACCOUNT, LEGAL_ACTION, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1lp76py/beware_of_dave_technologies_unauthorized_ach/
  text: |
    **TL;DR:** Dave Technologies withdrew $500 from my bank after I revoked authorization, mishandled my dispute for months, exposed another customer's sensitive banking info in a regulatory complaint (which they acknowledged), and ignored multiple compensation demands despite escalating to their Chief Legal Officer. I’m sharing my story publicly after exhausting all direct resolution options.
    
    Hi Reddit,
    
    I want to share my ongoing nightmare with Dave Technologies to warn others considering their s...[truncated]

- entry_id: REDDIT-0157
  title: "How do you survive bad credit when you need money fast?"
  date: 2025-08-21
  score: 21
  type: post
  topics: [CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1mwis4e/how_do_you_survive_bad_credit_when_you_need_money/
  text: |
    So here’s my deal: my credit score is trash (543 last time I checked), and the bank won’t even look at me for a loan. I need around $1,200 because my car broke down alternator and battery gone and I literally can’t get to work without it. The payday loan route is tempting, but I know how ugly that can get.
    
    I ran into MoneyFor while searching and it seems like they’re big on breaking down options for people like me. Stuff like fast loans, credit score building, and ways to get cash advances with...[truncated]

- entry_id: REDDIT-0158
  title: "Is money lion legit and what are your experiences"
  date: 2025-09-18
  score: 18
  type: post
  providers: [MoneyLion]
  topics: [CREDIT_REPORTING, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nk3a07/is_money_lion_legit_and_what_are_your_experiences/
  text: |
    My Take on MoneyLion feel free to add your own opinions and input in the comments of the thread 
    
    I know a lot of people are curious if money lion is safe, and Im always seeing people asking about it or asking for a reference to an app that helps with credit or cash advances. I had a ton of questions myself before I downloaded it but not alot of the post are very helpful. So, I wanted to share my experience and hopefully clear things up for anyone on the fence.
    
    The app can be a little confusing...[truncated]

- entry_id: REDDIT-0159
  title: "Dave Lawsuit?"
  date: 2025-03-25
  score: 16
  type: post
  providers: [Dave]
  topics: [ACH_REVOCATION, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1jjxiva/dave_lawsuit/
  text: |
    So I heard Dave is going through a lawsuit right now because people wanted to revoke ACH and couldn't. I mean, if it's true, I'm hoping they get taken to the cleaners.

- entry_id: REDDIT-0160
  title: "My Dave Horror Story"
  date: 2025-09-19
  score: 15
  type: post
  providers: [Dave]
  topics: [ACH_REVOCATION, BANK_ACCOUNT, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nl2snl/my_dave_horror_story/
  text: |
    I want to warn others about the Dave app. Personally I’ve never had an issue before this. 
    
    I requested one simple extension on my settlement a week in advance, because of a medical bill. 
    
    I’ve never missed a payment or asked for delays before. I have always been on time and I’ve had them for years. 
    
    I contacted support & I followed all of their instructions, providing my full address, government ID, selfie, name, date of birth, and last four of my Social Security number. Each time, they took ...[truncated]

- entry_id: REDDIT-0161
  title: "Can Dave and Brigit and Cleo send you to collections at all ?"
  date: 2025-05-04
  score: 15
  type: post
  providers: [Brigit, Cleo, Dave]
  topics: [COLLECTIONS, DEBT_CYCLE, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1kexd4y/can_dave_and_brigit_and_cleo_send_you_to/
  text: |
    Trying to get out of this cycle. I do intend to pay it back . But with current costs of living while it bought me time it just is not sustainable for me like I thought it would help. So if it comes to it do you know if they will take me to collections? Or sue?

- entry_id: REDDIT-0162
  title: "“Your $40 b00st is waiting, Subscribe to any plan to claim it” Bait and switch?"
  date: 2026-03-01
  score: 12
  type: post
  providers: [Cleo]
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ri9l32/your_40_b00st_is_waiting_subscribe_to_any_plan_to/
  text: |
    “Your $40 boost is waiting, Subscribe to any plan to claim it” doesn’t have any terms and conditions or disclosures attached to it. Yet after I subscribed and Cleo charged me $5.99 it’s nowhere to be found… I should’ve expected Cleo wouldn’t change their deceptive ways even after the class action lawsuit a year ago… Anyone else fall for this trap?

- entry_id: REDDIT-0163
  title: "My experience using Ualett."
  date: 2025-07-08
  score: 12
  type: post
  providers: [Ualett]
  topics: [CREDIT_REPORTING, GIG_WORKER]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1lusydr/my_experience_using_ualett/
  text: |
    Ualett is a great app if you need some quick cash. One thing I like about them is there's no credit check to qualify and they don't report to your credit report. Your job is your credit. I do gig apps and was able to qualify for $550 which was deposited in two business days after signing the paperwork.
    
    Two things that I don't like about the app is the weekly payments and the high interest rate. Having weekly payments had me constantly stressing about paying it off. It does help you pay it off f...[truncated]

- entry_id: REDDIT-0164
  title: "New invoice from True Finance LLC"
  date: 2026-01-11
  score: 11
  type: post
  topics: [CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q9lak3/new_invoice_from_true_finance_llc/
  text: |
    Is this a scare tactic? I got this in my email today, after my revoke went through… and I believe my old debit card was tied to true also so they couldn’t debit it… but their ToS clearly say they there’s no obligation to repay, no credit reporting etc .

- entry_id: REDDIT-0165
  title: "Does Dave send you to collections, put themselves on your credit, or sue if you revoke ACH?"
  date: 2025-09-26
  score: 10
  type: post
  providers: [Dave]
  topics: [ACH_REVOCATION, COLLECTIONS, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nqo7to/does_dave_send_you_to_collections_put_themselves/

```

---

## Curated Comments (Highest Signal)

```yaml
comments:
- entry_id: REDDIT-0166
  date: 2026-02-27
  score: 18
  type: comment
  topics: [CREDIT_REPORTING, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rfr1cm/i_hate_this_addiction_this_is_klover_moneylion/o7m99mz/
  text: |
    I just wanted you to know it’s not an addiction it is very hard to get out of the cycle because once your payday comes around you have no check so you have to repeat the withdrawals all over again. It’s so hard to get out of the cycle if you don’t have a way to just pay them all at once but my best advice would be decrease the amount you take each pay period for each or from one and eventually you can get out of it. But you can’t spend either it’s so stressful. It’s sad because a lot report to c...[truncated]

- entry_id: REDDIT-0167
  date: 2026-01-05
  score: 12
  type: comment
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q2qr9s/i_hate_that_i_have_to_borrow_money_just_to_never/nxs8zuc/
  text: |
    Fuck em.
    
     If they weren't doing something with questionable business ethics, they wouldn't need to put in print "we will not come after you for our money". You think they want to loan out money with the chance of not getting repaid out of the kindness of their hearts? Unlikely, however they must do this bypass the law. Take em for as much as you can. They would do the same to you.
     Fintech all over are getting sued left and right. You prolly qualify for one. Go search fintech lawsuits.

- entry_id: REDDIT-0168
  date: 2025-05-30
  score: 12
  type: comment
  providers: [Possible Finance]
  topics: [ACH_REVOCATION, CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1kz9zft/ach_revoke_help/mv3tl1y/
  text: |
    Possible is an actual loan that reflects on your credit report and not a cash advance, so I don’t think it would be a great decision to revoke ACH authorization from them. But that’s just me, though.

- entry_id: REDDIT-0169
  date: 2026-01-26
  score: 11
  type: comment
  providers: [Albert, Brigit, Cleo, Dave, Earnin, FloatMe, Gerald, Klover, MoneyLion, Possible Finance, Tilt, Ualett, Varo]
  topics: [LEGAL_ACTION, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qm53ja/ultimate_list_of_cash_advance_apps/o1qswau/
  text: |
    List of things that worked for me with NO DIRECT DEPOSIT :
    
    Albert
    
    AdvanceAmerica (loan shark payday loan)
    
    Atm dot com
    
    Brigit
    
    Cleo
    
    CreditGenie\* - I'm 90% sure I got one through here and then asked to delete account and now I'm permabanned. I emailed them a few min ago to see if I could reopen my account. Edit: they responded and reopened my account. I was able to get $100 from them! Sweet
    
    Dave
    
    Earnin
    
    FloatMe
    
    Frontpay
    
    Grant
    
    Grid...I think? I think I was approved but I haven't finished...[truncated]

- entry_id: REDDIT-0170
  date: 2025-05-31
  score: 11
  type: comment
  providers: [Dave]
  topics: [CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1kziowo/am_i_in_the_clear/mv70qh1/
  text: |
    Haven’t paid over $300 back to Dave since December. Nothing hit my credit

- entry_id: REDDIT-0171
  date: 2024-11-18
  score: 10
  type: comment
  providers: [Brigit]
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1guch6y/anyone_else_get_this_email/lxtdjeu/
  text: |
    It's legit!  Brigit settled a large lawsuit with the government for deceptive practices, and a whole $9 is flowing to each customer.  Better than nothing, right?
    
    [Here's the background and details on what happened at Brigit]([URL] if you're interested.

- entry_id: REDDIT-0172
  date: 2026-02-23
  score: 9
  type: comment
  providers: [Dave]
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rc0ky2/several_cash_advance_apps_are_getting_sued_and/o6x20sp/
  text: |
    Dave is scheduled for arbitration this week too

- entry_id: REDDIT-0173
  date: 2026-04-02
  score: 9
  type: comment
  topics: [ACH_REVOCATION, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1sa41vv/where_has_this_subreddit_been_all_my_life/odtaejf/
  text: |
    Revoke ACH from the cash advance apps. It's completely legal, and they are giving you a non recourse advance. You won't get sued for not paying it back.

- entry_id: REDDIT-0174
  date: 2026-02-02
  score: 8
  type: comment
  topics: [ACH_REVOCATION, DEBT_CYCLE, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qs4l7f/i_built_a_directory_of_cash_advance_apps/o33ved0/
  text: |
    As long as you don't get stuck in the cycle, they're not the worst. You can also just...not repay them, if you feel like you'll get stuck in the cycle. Search this sub for "revoke ACH" and look for the auto mod comment. You can get a cash advance & not repay them and there's nothing they can do, or their own terms and conditions. Nothing on your credit, they can't sue you, they don't even harass you to repay it. (I revoked them all once I got stuck in the cycle & couldn't get out from under them...[truncated]

- entry_id: REDDIT-0175
  date: 2025-05-16
  score: 8
  type: comment
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ko9dqm/dave_changed_the_rulesand_you_might_not_like_them/msoopu1/
  text: |
    They are such scum. I hope that class action messes them up

- entry_id: REDDIT-0176
  date: 2025-12-24
  score: 8
  type: comment
  topics: [CREDIT_REPORTING, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1pumg48/need_another_app_asap/nvrz3dy/
  text: |
    you’re like the only person that I’ve read actually get a loan from one of these lenders, everytime I apply i get trapped in a loop where it just keeps recommending other lenders. My credit score is around 568, not great but ive seen a lot worse. How’s yours?

- entry_id: REDDIT-0177
  date: 2026-02-27
  score: 7
  type: comment
  providers: [Possible Finance]
  topics: [CREDIT_REPORTING, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rfr1cm/i_hate_this_addiction_this_is_klover_moneylion/o7mc2hf/
  text: |
    Actually, very few apps report to credit bureaus.  It's one of the things that traps people in the cycle. Your credit score doesn't budge despite a strong track record of making on-time payments, so ou still can't qualify for a credit card or loan with a higher limit and better payment terms.
    
    Possible Finance and Upgrade Boost Money are two products that do report to credit bureaus, so if can make all of your repayments on time, they may be a good solution.

- entry_id: REDDIT-0178
  date: 2025-07-06
  score: 7
  type: comment
  topics: [CREDIT_REPORTING, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ls9rjn/thinking_youre_gonna_dodge_dave_app_by/n1mqnrd/
  text: |
    I have scammed every single one of these money apps. 
    
    Simply email their support, stating you are revoking all ACH connections and to remove any associated debit cards and banks information. 
    
    If charges go through, show your bank, reverse charge. Typically the company's follow through and I have never had this happen. 
    
    I have also done this for $2500 total through "Tribal" Lending services. These Indian companies are not federally recognized thus, once you take a loan out, do the same thing, ...[truncated]

- entry_id: REDDIT-0179
  date: 2025-10-11
  score: 7
  type: comment
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o1e06i/stopping_dave/nixx6p5/
  text: |
    Try reading there’s a lot more to it than me “being mad” they wanted their money back. They legitimately broke the law and have class action lawsuits because of this type of behavior, but yeah I’m totally the problem here for being mad about that. 
    
    I clearly state that I planned to pay them back and was going through something that didn’t allow me to do that, and revoked access which they ignored completely among other ridiculous things I literally spelled out for you to read. 
    
    There’s always ...[truncated]

- entry_id: REDDIT-0180
  date: 2026-01-14
  score: 6
  type: comment
  topics: [TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qcnqfk/paid_699_for_a_10_cash_advance_lol_go_to_hell/nzk4kpy/
  text: |
    The audacity of that fee is wild. Might as well ask for a tip too.

- entry_id: REDDIT-0181
  date: 2025-06-09
  score: 6
  type: comment
  topics: [CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1l7i6lx/largest_cash_advance_ive_gotten/mwwur2i/
  text: |
    My credit score is bad too 636, owe $1300 in credit card debt lol

- entry_id: REDDIT-0182
  date: 2026-01-30
  score: 6
  type: comment
  topics: [LEGAL_ACTION, PROVIDER_COMPLAINT, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qr76r0/stay_away_from_paynapaena/o2oi67b/
  text: |
    If you email the owner Aaron and tell him you’re opening a civil lawsuit for fraud due to taking funds without permission he’ll literally respond within 20 mins return your money and delete your account….i just did it

- entry_id: REDDIT-0183
  date: 2026-01-31
  score: 6
  type: comment
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qr76r0/stay_away_from_paynapaena/o2pgbf8/
  text: |
    This ! I just emailed them today and requested they close my account. They took all my info , connected my card then put me on a “waiting list” it’s been a month. I told them I do not feel comfortable knowing they have all this information and access and idek if I’m approved or not . I’m about to send another email threatening a lawsuit

- entry_id: REDDIT-0184
  date: 2025-03-18
  score: 6
  type: comment
  topics: [LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1jdwxpr/dave_literally_lowered_my_amount_within_minutes/midxsuq/
  text: |
    They use to be helpful! I’m with you! I use to be able to narrow like 400 bucks, now I’m lucky if I can get $50 and I make more now! It’s all good I just don’t use them! Right now they are going through a huge class action law suite. You should look into it!

- entry_id: REDDIT-0185
  date: 2025-02-22
  score: 6
  type: comment
  topics: [LEGAL_ACTION, TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ivhz8y/so_dave_has_fees_now/me5qv8y/
  text: |
    From what I read last time I opened the app just to see it said they did away with the tip feature and now have this set service fee instead. I assume it has to do with the lawsuit regarding the tipping.

- entry_id: REDDIT-0186
  date: 2025-12-14
  score: 6
  type: comment
  providers: [Dave]
  topics: [COLLECTIONS, CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1pmj99m/how_long_does_dave_chase_you_try_to_charge_you/nu0ijju/
  text: |
    There are various posts on this topic.  You can formally withdraw your consent to these pay apps. And choose to not repay them. I wasn't aware of this until recently. 
    They will not send your account to a debt collector or affect your credit score.  You just can't borrow from them anymore. Dave app was the most resistant of these.

- entry_id: REDDIT-0187
  date: 2025-10-17
  score: 5
  type: comment
  topics: [CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o85uzj/dave_stole_320_from_me_never_again/nk1zg0r/
  text: |
    OP I agree w/ all saying F ‘em back, got instant transfer of $600 & they been waiting months for it so far…unless I receive anything saying they’ll go for my credit score, they will never get that back from me 🤷🏾‍♂️

- entry_id: REDDIT-0188
  date: 2025-10-17
  score: 5
  type: comment
  topics: [CREDIT_REPORTING]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o85uzj/dave_stole_320_from_me_never_again/njw3vqg/
  text: |
    You are dumb. It will not… they don’t report to any of the three credit bureaus. Know you stuff before commenting bullshit

- entry_id: REDDIT-0189
  date: 2025-07-17
  score: 5
  type: comment
  providers: [Dave]
  topics: [ACH_REVOCATION, LEGAL_ACTION, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1m27hfb/my_journey_with_cash_advances_comes_to_an_end/n3mym74/
  text: |
    Yes you can revoke ACH and they can’t take the money from your account or sue you. However if they suspect you are trying to commit fraud they will sue you. Dave is the only one that people struggle with that I know of.

- entry_id: REDDIT-0190
  date: 2024-09-11
  score: 5
  type: comment
  providers: [Brigit, Cleo, Dave, Earnin]
  topics: [SUBSCRIPTION_FEES, TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1cyxxzq/new_cash_advance/lmm0nvi/
  text: |
    Brigit has a fee of $6/ month and I always get approved for $50. One plus with Brigit is the more on time payments you make, the more ‘extensions’ you earn.  Meaning if you end up being short to pay back you can ask to push your repayment date another week. 
    
    Dave is $1/ month and in the very beginning I was approved for $250. However I ended up with more bills and since most of these are based on your paycheck and how much you spend, i eventually only started to qualify for $175 a week. But the...[truncated]

```