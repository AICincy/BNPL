# Reddit Consumer Intelligence: Consumer Remedies and Complaints (SWARM-DELTA)

```
data_source_id: REDDIT-DELTA-001
swarm: SWARM-DELTA
subagents_served: [SA-DISPUTE, SA-FRAUD, SA-DISCLOSURE, SA-ESCALATION]
source: r/cashadvanceapps
extraction_date: 2026-04-12
claim_tag_default: OBS
source_reliability: CONSUMER_SELF_REPORT
```

---

## Signal Summary

```yaml
signal_summary:
  complaint_taxonomy:
    unauthorized_debit: 49  # consumers reporting debits without consent
    collections_referral: 138  # accounts sent to collections after non-payment
    provider_complaint: 255  # general complaints (scam, predatory, fraud framing)
    bank_account_issues: 399  # overdrafts, NSF, account closures triggered by EWA debits
  key_patterns:
    - pattern: Dave most-complained-about provider (1107 mentions, highest complaint volume)
    - pattern: Unauthorized double-debits reported across multiple providers
    - pattern: Consumers report providers debiting before payday (timing violations)
    - pattern: Subscription fees continuing after account closure attempts
    - pattern: Collections referral after ACH revocation (provider retaliation pattern)
    - pattern: Overdraft cascades from EWA debits (single EWA debit triggers multiple NSF fees)
    - pattern: Consumers successfully using CFPB complaints to resolve disputes
    - pattern: Bank account closure as nuclear option when ACH revocation fails
  escalation_paths_observed:
    - path: Provider dispute -> ACH revocation -> CFPB complaint -> resolution
    - path: Provider dispute -> bank dispute -> new bank account
    - path: Provider dispute -> mass arbitration signup -> settlement
    - path: Provider dispute -> state AG complaint
```

---

## Curated Posts

```yaml
posts:
- entry_id: REDDIT-0086
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

- entry_id: REDDIT-0087
  title: "Dave stole $320 from me. Never again."
  date: 2025-10-16
  score: 145
  type: post
  providers: [Dave]
  topics: [BANK_ACCOUNT, RECOVERY_SUCCESS, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o85uzj/dave_stole_320_from_me_never_again/
  text: |
    I requested an instant transfer on Saturday 10/12 and never received it. I can confirm this through bank transcripts.
    
    Fast forward to Tuesday 10/14. It was my settlement date. They withdrew the $320 I owed, even though I never got it to begin with.
    
    I spent two days wrestling with support. They kept insisting the money I requested was sent. They even refunded me $4.50 because the transfer wasn't instant (lmao).
    
    They eventually sent the money AFTER my settlement, which obviously did not help at...[truncated]

- entry_id: REDDIT-0088
  title: "Finally free"
  date: 2025-09-25
  score: 144
  type: post
  providers: [Cleo, Dave, Earnin, Tilt]
  topics: [BANK_ACCOUNT, DEBT_CYCLE, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nqloea/finally_free/
  text: |
    The last 3 years ive been in a revolving door and finally broke the cycle.
    
    Got enough cash to pay off my Dave balance. And closed the bank account connected to earnin, cleo, tilt, and money lion. And opened a new one that will be free of their taint and influence 
    
    It genuinely feels like a weight has been lifted off my chest now that i don’t have to worry about making sure my paycheque is big enough to repay and then re-borrow
    
    Big thank you to everyone here who asked the questions and answere...[truncated]

- entry_id: REDDIT-0089
  title: "I am glad to be done"
  date: 2025-10-08
  score: 118
  type: post
  topics: [BANK_ACCOUNT, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o1eo5l/i_am_glad_to_be_done/
  text: |
    I went through my bank account and saw how much I’ve gotten (and paid back) to cash advance apps. Please only use these apps temporarily, getting stuck in the loop is miserable. Thankfully I have revoked ACH from all the apps listed and closed all the accounts.

- entry_id: REDDIT-0090
  title: "My journey with cash advances comes to an end."
  date: 2025-07-17
  score: 100
  type: post
  providers: [Albert, Brigit, Cleo, Dave, Earnin, Empower, Klover]
  topics: [DEBT_CYCLE, LEGAL_ACTION, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1m27hfb/my_journey_with_cash_advances_comes_to_an_end/
  text: |
    I have been stuck in the never ending cycle of cash advance apps for roughly two years. Two years ago I had a rough month and needed a few bucks to get through. I started with Earnin.. there became my "addiction." It was so easy, and so harmless. I borrowed $200 and paid it back.. well, then I thought maybe I could get more.. and so I spiraled. Empower, Dave, Money Lion, Cleo, Brigit, Klover & Albert. It was wildly out of control. But I always seemed to manage. But the past year, I've made more ...[truncated]

- entry_id: REDDIT-0091
  title: "ACH revocation information for help"
  date: 2025-04-14
  score: 70
  type: post
  providers: [Brigit, Cleo, Earnin, Empower, FloatMe, Klover, MoneyLion]
  topics: [ACH_REVOCATION, BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1jza7oq/ach_revocation_information_for_help/
  text: |
    Because of this subreddit I was able to discover the ACH revocation and have successfully gotten these companies to fuck off via email. So I wanted to help as best I can. These are the terms of service stating no obligation to repay for the following apps 
    
    MoneyLion - customercare@moneylion.com
    
    Brigit - support@hellobrigit.com
    
    Earnin - I could not find an email 
    
    Cleo - team@meetcleo.com
    
    Klover - support@joinklover.com
    
    Empower - help@empower.me
    
    Vola - hello@volafinance.com
    
    FloatMe - suppo...[truncated]

- entry_id: REDDIT-0092
  title: "EX PAYDAY LOAN COMPANY EMPLOYEE INSIGHTS"
  date: 2026-02-06
  score: 68
  type: post
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qxuq4z/ex_payday_loan_company_employee_insights/
  text: |
    Worked for one of these and hated it and told myself when I left I'd share information on how to navigate it. \*\*\*\*\*\*\*\*\*\*\*\*\*\*none of this is legal or financial advice but just my own observations\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
    
    I have them separated by category, use this information how you will.
    
    TIPS FOR LOOKING FOR A LENDER
    
    \- Don't use a site that says they will "match" you with a lender, it's a lead provider and they are going to sell your information hundreds of times, if not ...[truncated]

- entry_id: REDDIT-0093
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

- entry_id: REDDIT-0094
  title: "Finally FREE (I think)"
  date: 2025-07-20
  score: 62
  type: post
  providers: [Dave]
  topics: [BANK_ACCOUNT, DEBT_CYCLE, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1m4be95/finally_free_i_think/
  text: |
    As we all know here, cash advances catch you, trap you and you can become dependent but you’re entire check goes to “settling dates” 
    
    I have a settlement date with Dave coming up on the 21st. I began this process on Thursday, so plenty of notices and room for everything to go through. I sent the template for the ACH revoke THREE times - no reply yet. I’ve called customer service.. they refused to adhere or help me and my revoke request. 
    
    I read on here there’s steps you can go through that hop...[truncated]

- entry_id: REDDIT-0095
  title: "Finally got out from under these apps - thanks to this fun."
  date: 2025-08-16
  score: 52
  type: post
  providers: [Cleo, Dave, Empower]
  topics: [BANK_ACCOUNT, RECOVERY_SUCCESS, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ms342s/finally_got_out_from_under_these_apps_thanks_to/
  text: |
    I just wanted to say thank you. - TO THIS *SUB* I can't edit the title of the post & didn't see the typo until it was posted 🙄
    
    I started using these cash advance apps over a year ago, when my paycheck direct deposit was lost. My check didn't get deposited for over a week, leaving me with no gas $$, no grocery $$, and as a single mom, I was desperate. Enter Cleo. Dave. Empower. Money Lion. All the usuals. I started with $50-100 from each app, just to get enough $$ to feed my kids for a bit. My b...[truncated]

- entry_id: REDDIT-0096
  title: "Albert has got me f’d up."
  date: 2025-10-28
  score: 44
  type: post
  providers: [Albert]
  topics: [BANK_ACCOUNT, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1oighfj/albert_has_got_me_fd_up/
  text: |
    On Friday They repaid themselves and took their $20 subscription fee cool no worries but a few hours go by And I go to request my $150 back and it’s unavailable. Somehow they were having issues linking my bank account that’s been linked since 2021! And then started to say they couldn’t link my account because another one of my amounts was negative. I was honestly like wtf is going on. This has never happened before. This morning I was finally able to get my advance amount, but 4 days later is ex...[truncated]

- entry_id: REDDIT-0097
  title: "Brigit past due balance cleared"
  date: 2025-11-08
  score: 42
  type: post
  providers: [Brigit]
  topics: [COLLECTIONS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ors6bn/brigit_past_due_balance_cleared/
  text: |
    I revoked ACH previously with them and got this email yesterday

- entry_id: REDDIT-0098
  title: "Finally out of the cycle!!!!!"
  date: 2025-11-17
  score: 38
  type: post
  providers: [Brigit, Dave, Klover]
  topics: [BANK_ACCOUNT, COLLECTIONS, DEBT_CYCLE, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ozl5lz/finally_out_of_the_cycle/
  text: |
    I have been in a horrible cycle with pay day loans and cash advances. I’m finally free. Today is Monday and I get paid on Wednesday. I made it without borrowing from Dave or klover! It’s been months maybe even a year or more since I’ve made it to the next check without borrowing. I still owe money to moneykey, Brigit and uprova but they are no longer able to deduct money from my account due to revoking ahc from uprova and closing my old bank account so moneykwy and Brigit couldn’t access. I have...[truncated]

- entry_id: REDDIT-0099
  title: "Finally Free"
  date: 2026-02-27
  score: 36
  type: post
  topics: [BANK_ACCOUNT, DEBT_CYCLE, LEGAL_ACTION, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rftt93/finally_free/
  text: |
    After almost two years of NEVER fully seeing my check and having to rely on the cycle of cash advances, I am FREE! My job payed out from a lawsuit and after every app took back their repayment, I revoked access, unlinked my bank card, and deleted them. While I understand that these apps can be “helpful”, they can also turn quite predatory. An $100 advance turns into a $300 advance, and judging on how deep, you probably downloaded more than one. Now you owe if not HALF your paycheck, the entirety...[truncated]

- entry_id: REDDIT-0100
  title: "Super Plus is a Fraud"
  date: 2025-08-01
  score: 35
  type: post
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1mf2lux/super_plus_is_a_fraud/
  text: |
    Please avoid super plus. They will charge you $15 for a membership and you will have continuous error trying to connect your bank card and it will never work.

- entry_id: REDDIT-0101
  title: "Class action lawsuits against cash advance apps taking claims"
  date: 2026-03-26
  score: 32
  type: post
  providers: [FloatMe, Klover, MoneyLion]
  topics: [BANK_ACCOUNT, LEGAL_ACTION]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1s4jo5k/class_action_lawsuits_against_cash_advance_apps/
  text: |
    MoneyLion, Klover, Grant, FloatMe, CreditGenie and more. Most are looking at advances in the last two years, YOU DO NEED EVIDENCE. Cashapp if you have paid to instantly transfer funds to your bank account and it took more than an hour. The claims are easy to fill out and are easily found on Google.

- entry_id: REDDIT-0102
  title: "Revoke ACH"
  date: 2025-05-14
  score: 31
  type: post
  topics: [ACH_REVOCATION, BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1km1npn/revoke_ach/
  text: |
    **\*\*Picture in comments of email addresses for popular cash advance apps\*\***
    
    \----------------------
    
    **Email template to revoke ACH:**
    
    Dear \[company\] Support Team,
    
    I am writing to formally revoke my authorization for automated clearinghouse (ACH) and debit card transactions for my \[company\] account associated with the email \[email\] and phone number \[phone #\]. This revocation applies to all future transfers out, including any charges from tips or Instant Transfer fees, and impacts...[truncated]

- entry_id: REDDIT-0103
  title: "Finally Out of the Cycle"
  date: 2026-03-12
  score: 30
  type: post
  providers: [Dave]
  topics: [DEBT_CYCLE, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rror0g/finally_out_of_the_cycle/
  text: |
    I’ve been in a cash advance cycle for 2 YEARS. I got a large sum of money this week and FINALLY pulled myself out of it and deleted all my accounts. At the lowest point I was advancing over 3x my paycheck. I was constantly panicking about paying everything back along with my bills. If you’ve heard of a cash advance app, chances are I was using it. I was using about 15 different cash advance apps. I really couldn’t believe I let it get this bad and I’m so happy to finally be out of it.
    
    For a bit...[truncated]

- entry_id: REDDIT-0104
  title: "Got away from Daves Settlements since you can't revoke anymore!"
  date: 2025-03-22
  score: 29
  type: post
  providers: [Dave, MoneyLion]
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1jhgk6s/got_away_from_daves_settlements_since_you_cant/
  text: |
    I was not able to revoke Dave. But after weeks of searching I figured out how to get around it. If you unlink Dave from your bank on The Plaid portal and you have an online bank that you don't keep any money in like MoneyLion. They will let you relink a new bank, in my case I relinked with MoneyLion, which changed the account and since I have no money in there and that is the only source they have to draw from I have made it out free and clear from Dave. It's been a month. Good luck! 
    
    BTW this ...[truncated]

- entry_id: REDDIT-0105
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

- entry_id: REDDIT-0106
  title: "Thanks for not letting this sub become full of spam and scams"
  date: 2024-12-05
  score: 27
  type: post
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1h72s0v/thanks_for_not_letting_this_sub_become_full_of/
  text: |
    Every other sub about borrowing money has gone to 💩 with wall to wall posts from spammers and scammers.  Thanks for keeping this one clean and useful mods!

- entry_id: REDDIT-0107
  title: "Two accounts with FloatMe"
  date: 2026-01-27
  score: 26
  type: post
  providers: [FloatMe]
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qol335/two_accounts_with_floatme/
  text: |
    If you download TextNow and get the free trial. Use that number to sign up. Use a different email than before. Connect a new bank account (if you've switched direct deposit accounts) FloatMe will allow you to create another account. Even if you never payed off the balance with the first account. Just an FYI.

- entry_id: REDDIT-0108
  title: "Review of FrontPay"
  date: 2024-10-25
  score: 25
  type: post
  topics: [BANK_ACCOUNT, TIPPING_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1gc5i9w/review_of_frontpay/
  text: |
    Hey so I came across a post here for FrontPay and gave it a try. There is no app but the website worked. It was easy to sign up and I got approved after connecting my bank account. The funds arrived in about 6 hours and I did not have to tip. I was looking for a new cash advance app so this worked for me

- entry_id: REDDIT-0109
  title: "Am I free from Dave?"
  date: 2025-07-29
  score: 23
  type: post
  providers: [Dave]
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1mcoukx/am_i_free_from_dave/
  text: |
    Can’t afford to pay it right now. I tried working something out with them MULTIPLE times and they were unwilling to do so. Now? they can smd.
    
    Can anyone who has successfully not paid back an advance yet tell me if this is what they did? Is this enough to protect my bank account? (lol @ the only $1 i’ve been keeping in there to protect my money)
    
    I also reported my debit card as lost and am getting a new one shipped since they had that on file and wouldn’t let me remove it until settling the bal...[truncated]

- entry_id: REDDIT-0110
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

- entry_id: REDDIT-0111
  title: "Stay Away From Payna/Paena"
  date: 2026-01-30
  score: 22
  type: post
  topics: [BANK_ACCOUNT, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qr76r0/stay_away_from_paynapaena/
  text: |
    Take this as a warning. Received and paid back one small advance with no issue. 
    
    Have been attempting to log back into my account for 2 days with no luck.
    
    Have reached out to their founder Aaron amd have not heard back.
    
    Received an email this morn that $25 will be debited from my bank account for a transaction that I never requested.

- entry_id: REDDIT-0112
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

- entry_id: REDDIT-0113
  title: "Thinking you’re gonna dodge Dave App by disconnecting from plaid.com???"
  date: 2025-07-05
  score: 18
  type: post
  providers: [Dave]
  topics: [ACH_REVOCATION, DEBT_CYCLE, SUBSCRIPTION_FEES, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ls9rjn/thinking_youre_gonna_dodge_dave_app_by/
  text: |
    Well guess what I thought that it’s that easy to disconnect from Dave by creating an account with plaid.com and getting a new debit card. I did all of that a month ago after being trapped by Dave for almost a year. I have endless emails of going back and forth trying to revoke ach authorization.  No luck so after reading endless posts and comments I took other people’s bright ideas and thought it would be just that easy so I did disconnect from plaid got a new debit card everything was good for ...[truncated]

- entry_id: REDDIT-0114
  title: "I am done with the cycle"
  date: 2026-03-19
  score: 17
  type: post
  providers: [Cleo, Earnin, MoneyLion, Tilt]
  topics: [ACH_REVOCATION, DEBT_CYCLE, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rxy4oj/i_am_done_with_the_cycle/
  text: |
    I made the decision to revoke ACH access from Tilt, the last cash advance app left standing on my phone. I will no longer rely on any of these predatory apps ever again. For the record, I have used EarnIn, Tilt, MoneyLion, Cleo, and probably a few others. Revoked from all of them and haven’t looked back. Time to be more responsible with my spending moving forward.

- entry_id: REDDIT-0115
  title: "Earnin - ACH Authorization"
  date: 2025-04-24
  score: 17
  type: post
  providers: [Earnin]
  topics: [ACH_REVOCATION, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1k75d71/earnin_ach_authorization/
  text: |
    This is going to sound dumb to many people.
    
    Am I the only one who has revoked ACH authorization from EarnIn and felt guilty about it?
    
    I had to do it. I could not afford to pay them back this time, even with rescheduling. My back was against the wall after about 5 years of using the app.
    
    It feels like they’ve helped me through a lot of tough times financially, and now I’m stiffing them in return.
    
    I don’t like how this feels. Can anyone here tell me how dumb it is for me to feel this way? Or c...[truncated]

```

---

## Curated Comments (Highest Signal)

```yaml
comments:
- entry_id: REDDIT-0116
  date: 2026-02-12
  score: 18
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1r2z1w4/update_my_marketwatch_story_on_the_ach_loophole/o50isne/
  text: |
    This story is going to make these apps die. You’re not exposing how they are trapping people, you are exposing how people scam these apps

- entry_id: REDDIT-0117
  date: 2024-05-23
  score: 15
  type: comment
  providers: [Chime, Gerald, Klover]
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1cyxxzq/new_cash_advance/l5d1zon/
  text: |
    A few newer / lesser known cash advance apps:
    
    [Super.com]([URL] - Been advertising all over the place, so you may have seen it.  It's not a dedicated cash advance app, but offer advances up to $250 as one of its features.  It has a bunch of cash back offers, travel deals, etc.  You have to subscribe for $15/month to access advances (plus other fees), so if you're just using it for that, it's totally not worth it.  If you don't mind jumping though hoops with downloads, game play and other stuff ...[truncated]

- entry_id: REDDIT-0118
  date: 2026-01-24
  score: 15
  type: comment
  topics: [COLLECTIONS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ql9ksp/brigit_cleared_many_overdue_advances/o1cso3e/
  text: |
    Im 941 days past due for 50.99$ not forgiven yet.

- entry_id: REDDIT-0119
  date: 2024-05-30
  score: 13
  type: comment
  providers: [Branch, FloatMe, Gerald]
  topics: [ACH_REVOCATION, BANK_ACCOUNT, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1cyxxzq/new_cash_advance/l69k6k4/
  text: |
    Gerald is crap.  They stopped their membership fee and now make you buy something out of their shop or pay for a phone plan out of the advance.  Legit said I HAD to spend $30.20 in their store/phone. Out of $50.90 they were willing to give me. Still had to pay back the full $50.90.  Their store had like 5 "in stock" items.  Small bottles of head and shoulders were $9. Disposable razors 5pk for like $9. 120count roll of paper towels ONE SINGLE ROLL $9. Nahh.  It's not worth it.  
    
    Credit Genie wa...[truncated]

- entry_id: REDDIT-0120
  date: 2026-03-26
  score: 13
  type: comment
  topics: [COLLECTIONS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1s4d801/varo_advance/ocn024z/
  text: |
    It’s not going to collections. It’s in their terms that the cash advance is a non-recourse advance.
    
    You are obligated to pay it back. If you don’t though, they are not able to pursue you with debt collections through 3rd parties. You’ll be banned and unable to take out advances.
    
    They’ll email you and thats it.

- entry_id: REDDIT-0121
  date: 2025-04-24
  score: 12
  type: comment
  providers: [Dave, Possible Finance]
  topics: [BANK_ACCOUNT, DEBT_CYCLE, PROVIDER_COMPLAINT, RECOVERY_SUCCESS, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1k75d71/earnin_ach_authorization/movo6ys/
  text: |
    I understand how you’re feeling. But one thing you have to realize is that these apps are built in a predatory way from the start in a sense. They take advantage of people that are struggling financially, and charge you a fee for everything possible. Instant transfer to your bank account, $5 fee, subscription fee $10 a month, etc etc. revoking ACH is genuinely the only way out of the cycle because by using these apps you’re living off income that you don’t really have. If your paycheck is only $...[truncated]

- entry_id: REDDIT-0122
  date: 2025-09-23
  score: 12
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nou4tc/beware/nfue8jz/
  text: |
    Posts like this are 100% scam, 100% of the time.  THEY WILL STEAL FROM YOU.

- entry_id: REDDIT-0123
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

- entry_id: REDDIT-0124
  date: 2026-01-05
  score: 11
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q4nzmd/which_apps_am_i_missing/nxtx9xt/
  text: |
    Stay away from any other apps

- entry_id: REDDIT-0125
  date: 2026-01-05
  score: 11
  type: comment
  providers: [Albert, FloatMe]
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q4nzmd/which_apps_am_i_missing/nxvjaa4/
  text: |
    Confirming that OneBlinc, FloatMe, Vola and Credit Genie have all worked for me, I would personally stay away from Albert because in my experience they offer little money with high fees and other BS

- entry_id: REDDIT-0126
  date: 2025-09-15
  score: 11
  type: comment
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nht4mw/revoking_ach/nedyr6p/
  text: |
    Email this with your information included. 
    
    I am writing to formally revoke your authorization to initiate any ACH debits or withdrawals from my bank account on file effective immediately. Please consider this written notice as revocation of consent in accordance with the  Electric Funds Transfer Act and your Terms and Conditions.  
    
    Specifically, I am revoking authorization for any and all future electronic funds transfers, including, but not limited to cash advances and fees from the followin...[truncated]

- entry_id: REDDIT-0127
  date: 2026-02-21
  score: 10
  type: comment
  topics: [DEBT_CYCLE, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rau5o9/i_finally_paid_off_my_cash_advances_and_deleted/o6mdz6a/
  text: |
    None. Stay away from them if you can. It’s a cycle that it’s hard to get out of! But if you still want to use advances. I would suggest earn in. You can pay them off early, pay off each amount you took out instead of the whole thing. And atleast they limit you per day.

- entry_id: REDDIT-0128
  date: 2025-10-17
  score: 10
  type: comment
  providers: [Dave]
  topics: [ACH_REVOCATION, BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o8wh2r/im_fuming/nk0h9je/
  text: |
    Im not gonna lie to you, Dave is the most difficult of all. They are actual parasites and will use any method to get their money back. As far as I know they do not report, but your best method is:
    
    Revoke ACH via email, disconnect Plaid, change expiration date on card in the app, get a new debit card. If all else fails, get a new bank. I am not kidding.

- entry_id: REDDIT-0129
  date: 2025-10-01
  score: 10
  type: comment
  providers: [Dave]
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nuv8df/new_problem_with_you_guessed_it_dave/nh6xptw/
  text: |
    I tried revoking and got the same email. I disconnected through plaid and got an email from Dave saying to reconnect my bank account so I thought I was in the clear. But they still took the payment out the next week when I got paid

- entry_id: REDDIT-0130
  date: 2025-04-10
  score: 9
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1cyxxzq/new_cash_advance/mmfxzno/
  text: |
    So what? Stealing from a predatory app to begin with doesn't bother me one bit

- entry_id: REDDIT-0131
  date: 2026-01-10
  score: 9
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nrn76i/need_100_but_used_every_possible_no_pun_intended/nytbcm4/
  text: |
    This is absolutely a scam people. He's posted it in the borrow subreddit as well, trying to scam people....

- entry_id: REDDIT-0132
  date: 2026-02-11
  score: 9
  type: comment
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1r25lee/free_from_the_evil_bear/o4uxj07/
  text: |
    I’ll take it another step and close my bank account and open a new one if they want to try to charge me. I’m not playing around with David !!

- entry_id: REDDIT-0133
  date: 2025-11-10
  score: 9
  type: comment
  topics: [ACH_REVOCATION, BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1otl93w/cleo_did_i_do_it_am_i_finally_free_from_them/no5jdq5/
  text: |
    I sent this email to team@meetcleo.com
    
    Subject: Revocation of ACH Authorization and Account Cancellation
    
    I am writing to formally revoke authorization for [app] to initiate any ACH debits or withdrawals from my bank account on file effective immediately. Please consider this written notice as revocation of consent in accordance with the Electric Funds Transfer Act and your Terms and Conditions.
    Specifically, I am revoking authorization for any and all future electronic funds transfers, includi...[truncated]

- entry_id: REDDIT-0134
  date: 2025-04-24
  score: 9
  type: comment
  topics: [ACH_REVOCATION, BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1k6y3qh/revoking_ach_access_i_feel_free/motq2ny/
  text: |
    I saw on here to email them and then double checked all of their current terms and conditions and all said to email them (also printed as PDF to keep the no recourse thing from them in writing.
    
    I emailed each:
    
    Subject: Revocation of ACH Authorization and Account Cancellation
    
    Body:   
    I am writing to formally revoke any and all ACH authorizations previously granted to \[APP\] to debit my bank account. 
    
    Please cease all future ACH transactions and ensure that no further debits or credits are p...[truncated]

- entry_id: REDDIT-0135
  date: 2025-06-14
  score: 9
  type: comment
  topics: [DEBT_CYCLE, PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1laxt32/depending_on_paying_back_dave/mxts3w8/
  text: |
    Tbh, the ONLY way I was able to walk away from this vicious cycle was borrowing money from ALL of them and then not repaying. That way I had no choice but to stop. It’s honestly a really nasty vicious cycle and it does suck to need 50 bucks a week before you get paid or need $300 right after your paycheck hit, but it’s also nice to get paid and have an entire check. I had no self-control, but I knew that I was in a vicious cycle. Whatever happens when you don’t repay them, happens. That’s my att...[truncated]

- entry_id: REDDIT-0136
  date: 2025-10-31
  score: 9
  type: comment
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1okzrt8/i_need_help/nmehrxu/
  text: |
    I'm sorry you are going through this. It sounds like you should close your bank account and open a new one. Then you have the upper hand when it comes to negotiating repayment terms on your debts. Revoking is also an option for some of these. Or you could reach out to each provider and see if they will work with you.

- entry_id: REDDIT-0137
  date: 2025-09-21
  score: 9
  type: comment
  topics: [SUBSCRIPTION_FEES, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1nn13jh/repaid_through_cancelled_card/nfhoaj7/
  text: |
    This is probably happening because of Visa Account Updater (VAU) or Mastercard Automatic Billing Updater (ABU).
    
    When you report a card lost or stolen and get a new one, Visa and Mastercard send the updated card info to any companies that had your old card on file, as long as those companies are enrolled in the service. It is meant to stop recurring charges like subscriptions or loan payments from getting declined when your card changes.
    
    Even if you cancel the card, those companies can still ge...[truncated]

- entry_id: REDDIT-0138
  date: 2025-10-08
  score: 8
  type: comment
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o1eo5l/i_am_glad_to_be_done/nigrvde/
  text: |
    I sent this email template that I found here 
    
    I am writing to formally revoke your authorization to initiate any ACH debits or withdrawals from my bank account on file effective immediately. Please consider this written notice as revocation of consent in accordance with the Electric Funds Transfer Act and your Terms and Conditions.
    
    Specifically, I am revoking authorization for any and all future electronic funds transfers, including, but not limited to cash advances and fees from the following...[truncated]

- entry_id: REDDIT-0139
  date: 2025-12-31
  score: 8
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q06n2w/guilt/nwvnr5m/
  text: |
    I have and then I tried to get a new one and got scammed. I learned my lesson and so many are being investigated right now.

- entry_id: REDDIT-0140
  date: 2026-01-01
  score: 8
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q06n2w/guilt/nx0q4o0/
  text: |
    Don’t feel an ounce of guilt. They’re legit predatory lending apps. We’re living in a late stage capitalist dystopia and you do what you gotta do to get by. Use or be used. Not saying I endorse anyone doing it, but I sure as hell ain’t mad at em. That’s my philosophy anyways. Won’t shed a single tear for any of these corporations.

- entry_id: REDDIT-0141
  date: 2025-05-08
  score: 8
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1khbst1/do_you_think_there_has_been_an_extreme_influx_of/mr5wyuy/
  text: |
    Depending on how long you've been stuck, you have been paying crazy predatory fees that have surpassed the borrow amount. They are getting their money and then some. I don't think it's "free" money for most. Aside from those that do one and dip.

- entry_id: REDDIT-0142
  date: 2025-07-01
  score: 8
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1lp97yp/earnin_lost_this_battle/n0tfc84/
  text: |
    I’m not defending this practice but it’s hard to feel too bad for predatory companies. Companies that prey are financially insecure people using payday apps have to understand their core audience and yet they still take the risk. Sure they’re getting burned by some customers but the model is still extremely profitable for them or they wouldn’t be doing it.

- entry_id: REDDIT-0143
  date: 2025-02-22
  score: 8
  type: comment
  providers: [Dave]
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ivhz8y/so_dave_has_fees_now/me6gjqq/
  text: |
    Dave is a scam

- entry_id: REDDIT-0144
  date: 2025-05-19
  score: 8
  type: comment
  topics: [PROVIDER_COMPLAINT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1kq3mxd/is_lenme_a_scam/mt2vfbf/
  text: |
    i don't think its a scam but i don't think many ppl use it. nobody ever  replies to request on there

- entry_id: REDDIT-0145
  date: 2025-12-14
  score: 8
  type: comment
  providers: [Dave]
  topics: [BANK_ACCOUNT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1pmj99m/how_long_does_dave_chase_you_try_to_charge_you/nu0fv4e/
  text: |
    In my experience, Dave will keep trying you until they’re repaid. And they’ll sneak you. Need a whole new bank account. I also keep my money in my savings. I moved a tiny amount one day to grocery shop (store I was shopping at has terrible cell service and didn’t want to chance it) was able to check my balance when I got to the grocery store lot and one of the advance apps had snatched every penny out of that acct.

```