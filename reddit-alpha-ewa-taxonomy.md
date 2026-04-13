# Reddit Consumer Intelligence: EWA Provider Taxonomy (SWARM-ALPHA)

```
data_source_id: REDDIT-ALPHA-001
swarm: SWARM-ALPHA
subagents_served: [SA-EWA-TAX, SA-DEMO]
source: r/cashadvanceapps
extraction_date: 2026-04-12
claim_tag_default: OBS
source_reliability: CONSUMER_SELF_REPORT
```

---

## Provider Mention Registry (r/cashadvanceapps)

```yaml
provider_registry:
  - provider: Dave
    total_mentions: 753
    complaint_mentions: 47
    ach_revocation_mentions: 94
    debt_cycle_mentions: 76
    avg_post_score: 6.0
    complaint_ratio_pct: 6.2

  - provider: Earnin
    total_mentions: 441
    complaint_mentions: 11
    ach_revocation_mentions: 32
    debt_cycle_mentions: 42
    avg_post_score: 5.8
    complaint_ratio_pct: 2.5

  - provider: Cleo
    total_mentions: 244
    complaint_mentions: 13
    ach_revocation_mentions: 19
    debt_cycle_mentions: 20
    avg_post_score: 8.3
    complaint_ratio_pct: 5.3

  - provider: Brigit
    total_mentions: 190
    complaint_mentions: 8
    ach_revocation_mentions: 15
    debt_cycle_mentions: 19
    avg_post_score: 9.2
    complaint_ratio_pct: 4.2

  - provider: Klover
    total_mentions: 170
    complaint_mentions: 5
    ach_revocation_mentions: 13
    debt_cycle_mentions: 20
    avg_post_score: 9.7
    complaint_ratio_pct: 2.9

  - provider: Empower
    total_mentions: 169
    complaint_mentions: 10
    ach_revocation_mentions: 14
    debt_cycle_mentions: 17
    avg_post_score: 8.2
    complaint_ratio_pct: 5.9

  - provider: MoneyLion
    total_mentions: 167
    complaint_mentions: 9
    ach_revocation_mentions: 16
    debt_cycle_mentions: 19
    avg_post_score: 9.5
    complaint_ratio_pct: 5.4

  - provider: Albert
    total_mentions: 151
    complaint_mentions: 13
    ach_revocation_mentions: 17
    debt_cycle_mentions: 15
    avg_post_score: 9.7
    complaint_ratio_pct: 8.6

  - provider: Tilt
    total_mentions: 147
    complaint_mentions: 8
    ach_revocation_mentions: 9
    debt_cycle_mentions: 15
    avg_post_score: 7.9
    complaint_ratio_pct: 5.4

  - provider: Possible Finance
    total_mentions: 132
    complaint_mentions: 11
    ach_revocation_mentions: 10
    debt_cycle_mentions: 16
    avg_post_score: 7.8
    complaint_ratio_pct: 8.3

  - provider: Chime
    total_mentions: 94
    complaint_mentions: 6
    ach_revocation_mentions: 3
    debt_cycle_mentions: 5
    avg_post_score: 3.9
    complaint_ratio_pct: 6.4

  - provider: FloatMe
    total_mentions: 50
    complaint_mentions: 5
    ach_revocation_mentions: 6
    debt_cycle_mentions: 6
    avg_post_score: 20.3
    complaint_ratio_pct: 10.0

  - provider: Varo
    total_mentions: 50
    complaint_mentions: 2
    ach_revocation_mentions: 0
    debt_cycle_mentions: 3
    avg_post_score: 7.9
    complaint_ratio_pct: 4.0

  - provider: Gerald
    total_mentions: 32
    complaint_mentions: 4
    ach_revocation_mentions: 3
    debt_cycle_mentions: 3
    avg_post_score: 10.4
    complaint_ratio_pct: 12.5

  - provider: Solo Funds
    total_mentions: 18
    complaint_mentions: 0
    ach_revocation_mentions: 0
    debt_cycle_mentions: 1
    avg_post_score: 8.0
    complaint_ratio_pct: 0.0

  - provider: Ualett
    total_mentions: 17
    complaint_mentions: 1
    ach_revocation_mentions: 0
    debt_cycle_mentions: 0
    avg_post_score: 7.5
    complaint_ratio_pct: 5.9

  - provider: Payactiv
    total_mentions: 3
    complaint_mentions: 0
    ach_revocation_mentions: 0
    debt_cycle_mentions: 0
    avg_post_score: 54.0

  - provider: Branch
    total_mentions: 2
    complaint_mentions: 0
    ach_revocation_mentions: 2
    debt_cycle_mentions: 0
    avg_post_score: 8.0

  - provider: DailyPay
    total_mentions: 2
    complaint_mentions: 0
    ach_revocation_mentions: 1
    debt_cycle_mentions: 0
    avg_post_score: 2.0

```

---

## Signal Summary

```yaml
signal_summary:
  consumer_behavioral_patterns:
    - pattern: Multi-app stacking is normative (users report 4-8 simultaneous EWA apps)
    - pattern: Gig workers (DoorDash, Uber, Spark) are disproportionately represented
    - pattern: Subscription fees are a primary cost driver; users report paying $5-15/month per app across 3-8 apps
    - pattern: Tipping models (Earnin) perceived as coercive despite being labeled 'optional'
    - pattern: Debt cycle self-identification is common; users describe 'addiction' framing
    - pattern: Recovery posts (breaking the cycle) consistently highest-engagement content
    - pattern: Average advance amounts $50-350 range; some providers (Ualett) offering larger amounts for gig workers
  demographic_signals:
    - Young adults (18-30) overrepresented based on post content
    - Gig economy workers as primary user cohort
    - Users reporting income $300-800/week range
    - Users report being 1-2 paychecks from financial crisis
```

---

## Curated Posts

```yaml
posts:
- entry_id: REDDIT-0061
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

- entry_id: REDDIT-0062
  title: "I am glad to be done"
  date: 2025-10-08
  score: 118
  type: post
  topics: [BANK_ACCOUNT, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1o1eo5l/i_am_glad_to_be_done/
  text: |
    I went through my bank account and saw how much I’ve gotten (and paid back) to cash advance apps. Please only use these apps temporarily, getting stuck in the loop is miserable. Thankfully I have revoked ACH from all the apps listed and closed all the accounts.

- entry_id: REDDIT-0063
  title: "My journey with cash advances comes to an end."
  date: 2025-07-17
  score: 100
  type: post
  providers: [Albert, Brigit, Cleo, Dave, Earnin, Empower, Klover]
  topics: [DEBT_CYCLE, LEGAL_ACTION, UNAUTHORIZED_DEBIT]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1m27hfb/my_journey_with_cash_advances_comes_to_an_end/
  text: |
    I have been stuck in the never ending cycle of cash advance apps for roughly two years. Two years ago I had a rough month and needed a few bucks to get through. I started with Earnin.. there became my "addiction." It was so easy, and so harmless. I borrowed $200 and paid it back.. well, then I thought maybe I could get more.. and so I spiraled. Empower, Dave, Money Lion, Cleo, Brigit, Klover & Albert. It was wildly out of control. But I always seemed to manage. But the past year, I've made more ...[truncated]

- entry_id: REDDIT-0064
  title: "Newer Cash Advance Apps (2026)"
  date: 2026-01-06
  score: 82
  type: post
  providers: [Albert, Brigit, Cleo, Dave, Earnin, Empower, FloatMe, Gerald, Klover, MoneyLion, Possible Finance, Solo Funds, Varo]
  topics: [DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1q5cic3/newer_cash_advance_apps_2026/
  text: |
    Hello, everyone. Ok, so.. Over the last year, I’ve fallen on hard times and found myself in the never-ending cycle of borrow-payback-borrow with these damn cash advance apps. There were literally times when I had not a dime to my name and I would come to this subreddit hoping to find a new app I could borrow from just to have carfare for work the next day. I’ve borrowed from virtually every app that out there, even failing to pay back and revoking ACH for most of them. It got so bad, I would wai...[truncated]

- entry_id: REDDIT-0065
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

- entry_id: REDDIT-0066
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

- entry_id: REDDIT-0067
  title: "I hate this addiction. This is Klover, MoneyLion, EarnIn & Cleo.. i still have Dave, Tilt, Floatme, & more its sad 😢"
  date: 2026-02-27
  score: 55
  type: post
  providers: [Cleo, Dave, Earnin, FloatMe, Klover, MoneyLion, Tilt]
  topics: [DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rfr1cm/i_hate_this_addiction_this_is_klover_moneylion/

- entry_id: REDDIT-0068
  title: "Finished"
  date: 2026-01-27
  score: 52
  type: post
  providers: [Dave, Earnin]
  topics: [DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1qoq3nx/finished/
  text: |
    I recently got a $2000 loan. I have been stuck in a Dave and Earnin cycle for a year now. I am beyond excited to pay them off and not use them ever again. I just wanted to share my milestone with someone.

- entry_id: REDDIT-0069
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

- entry_id: REDDIT-0070
  title: "I’M FREE FROM THE NEVER ENDING CYCLE."
  date: 2025-02-11
  score: 51
  type: post
  providers: [Earnin, Empower]
  topics: [ACH_REVOCATION, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1imm5mc/im_free_from_the_never_ending_cycle/
  text: |
    I was able to successfully revoke ACH authorization from empower and earnin. I was in this mess for almost a year. Every single check i was borrowing back to make ends meet. I couldn’t take the stress an anxiety and just an inconvenience. It clearly says at the bottom of the email that nothing can be done except I won’t be able to use the app until I pay back the loans.

- entry_id: REDDIT-0071
  title: "You Can Do It"
  date: 2025-05-07
  score: 48
  type: post
  providers: [Albert, Brigit, Cleo, Dave, FloatMe, Gerald, Klover]
  topics: [ACH_REVOCATION, DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1kgvl6r/you_can_do_it/
  text: |
    A few weeks back I was stuck in the cash advance spiral - I needed the advances to get by, but because of paying back the advances I could never get ahead.
    
    Then I saw a post here about ACH revocation and decided to get serious. I sent off 15 emails to the companies I took advances from telling them I wanted out and I logged into Plaid and deleted all of the authorizations tying their service to these various organizations.
    
    Klover still charged me. The Money app still charged me. The rest did n...[truncated]

- entry_id: REDDIT-0072
  title: "Largest cash advance I’ve gotten"
  date: 2025-06-09
  score: 47
  type: post
  providers: [Ualett]
  topics: [GIG_WORKER]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1l7i6lx/largest_cash_advance_ive_gotten/
  text: |
    Ualett is a good option for gig works never heard of it till yesterday, I only make like 300-500 a week on doordash for reference, I’m on a 10 week loan, will pay off in full. Gives me time to finally pay off my credit card and student loan debt for a week.

- entry_id: REDDIT-0073
  title: "Dave may have screwed up and lost themselves money LOL"
  date: 2025-12-17
  score: 46
  type: post
  providers: [Dave]
  topics: [DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1pov6hv/dave_may_have_screwed_up_and_lost_themselves/
  text: |
    I have been stuck in the Dave loop for awhile now. My extra cash has been jumping in the $300-$350 range and as soon as I pay I back within a couple of hours I take it out again. That was true until early last week, after paying back from $350 Dave dropped my extra cash to $50! I have seen where the app goes back up the next day so I told myself I can wait 24 hours and be fine but now almost a week later and my extra cash just jumps between $50 and $125. It has taken some forced sacrifices but I...[truncated]

- entry_id: REDDIT-0074
  title: "Albert has got me f’d up."
  date: 2025-10-28
  score: 44
  type: post
  providers: [Albert]
  topics: [BANK_ACCOUNT, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1oighfj/albert_has_got_me_fd_up/
  text: |
    On Friday They repaid themselves and took their $20 subscription fee cool no worries but a few hours go by And I go to request my $150 back and it’s unavailable. Somehow they were having issues linking my bank account that’s been linked since 2021! And then started to say they couldn’t link my account because another one of my amounts was negative. I was honestly like wtf is going on. This has never happened before. This morning I was finally able to get my advance amount, but 4 days later is ex...[truncated]

- entry_id: REDDIT-0075
  title: "I’m finally free!!!!"
  date: 2026-02-13
  score: 44
  type: post
  topics: [DEBT_CYCLE, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1r3l9ts/im_finally_free/
  text: |
    I was stuck in this cycle of using multiple cash advance apps that basically cleared my paycheck until I borrowed it all again and have been trying to get rid of them one by one for like 2 years. I was lucky to get promoted at work recently and I got my tax return on the same day as my paycheck. The apps basically took my whole return but I’m not even mad because I’m just proud to be FREE from this cycle! I’m deleting the apps and not looking back.

- entry_id: REDDIT-0076
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

- entry_id: REDDIT-0077
  title: "Finally out of the cycle!!!!!"
  date: 2025-11-17
  score: 38
  type: post
  providers: [Brigit, Dave, Klover]
  topics: [BANK_ACCOUNT, COLLECTIONS, DEBT_CYCLE, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1ozl5lz/finally_out_of_the_cycle/
  text: |
    I have been in a horrible cycle with pay day loans and cash advances. I’m finally free. Today is Monday and I get paid on Wednesday. I made it without borrowing from Dave or klover! It’s been months maybe even a year or more since I’ve made it to the next check without borrowing. I still owe money to moneykey, Brigit and uprova but they are no longer able to deduct money from my account due to revoking ahc from uprova and closing my old bank account so moneykwy and Brigit couldn’t access. I have...[truncated]

- entry_id: REDDIT-0078
  title: "PSA for people that got stuck"
  date: 2025-11-24
  score: 37
  type: post
  providers: [Brigit, Earnin, Empower, Possible Finance, Tilt]
  topics: [DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1p5x1am/psa_for_people_that_got_stuck/
  text: |
    Good evening! I am posting this to people that have gotten out of a cycle. If that isn't you, you can stop reading now.
    
    So we all know these apps can really come in handy in a tight situation, but everytime you do that, your paycheck is less and less, and some people, myself included, got into a cycle where you absolutely have to take an advance to see a full paycheck.
    
    I've gotten up to basically do it for my whole paycheck when I was using earnin. Basically my paycheck would come in, it would...[truncated]

- entry_id: REDDIT-0079
  title: "Finally Free"
  date: 2026-02-27
  score: 36
  type: post
  topics: [BANK_ACCOUNT, DEBT_CYCLE, LEGAL_ACTION, PROVIDER_COMPLAINT, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1rftt93/finally_free/
  text: |
    After almost two years of NEVER fully seeing my check and having to rely on the cycle of cash advances, I am FREE! My job payed out from a lawsuit and after every app took back their repayment, I revoked access, unlinked my bank card, and deleted them. While I understand that these apps can be “helpful”, they can also turn quite predatory. An $100 advance turns into a $300 advance, and judging on how deep, you probably downloaded more than one. Now you owe if not HALF your paycheck, the entirety...[truncated]

- entry_id: REDDIT-0080
  title: "I broke the cycle"
  date: 2025-03-13
  score: 35
  type: post
  topics: [ACH_REVOCATION, DEBT_CYCLE, RECOVERY_SUCCESS]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1jae8u9/i_broke_the_cycle/
  text: |
    Hi Guys
    
    Thanks to everyone who talked about the ACH revocation. Was stuck in a vicious cycle for months and finally broke the wheel. Feels so good

- entry_id: REDDIT-0081
  title: "New Cash Advance"
  date: 2026-03-24
  score: 33
  type: post
  topics: [SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1s2di0j/new_cash_advance/
  text: |
    Well as most of you are — I was lookin for another app cause I’m down bad lmao well I found one most people haven’t done because they changed stuff recently.
     
    Upgrade.com!!! 
    
    They used to make you deposit $50 for an advance. Now all you have to do is create an accoun, “pay” the $9 subscription fee,
     (it does not charge you right away so don’t worry) You should get a $50 advance if you just link your bank. Worked perfect for me.
    
    Let me know if you need help or have questions

- entry_id: REDDIT-0082
  title: "I'm out"
  date: 2026-03-31
  score: 31
  type: post
  providers: [Dave, Earnin, MoneyLion, Possible Finance]
  topics: [DEBT_CYCLE, SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1s883ku/im_out/
  text: |
    After recently seeing on my Plaid permissions that some of these apps have had access since 2023, yes that is correct, I knew I needed to end the cycle as I literally can no longer afford to pay these crooks back right now. 
    
    Today I revoked the last ACH permission I had. Well, the last one left is Dave - the impossible behemoth - and they'll get their final payment on Thursday.
    
    I started taking advances from Amscot when I was 22 that got me stuck for a couple years. When I was 27 I took a few ...[truncated]

- entry_id: REDDIT-0083
  title: "trying to get out of this cycle"
  date: 2025-03-08
  score: 31
  type: post
  providers: [Albert, Brigit, Cleo, Dave, Earnin, Empower, FloatMe, MoneyLion]
  topics: [DEBT_CYCLE]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1j6ucza/trying_to_get_out_of_this_cycle/
  text: |
    A few months ago, I was going through some financial struggles and ended up using multiple cash advance apps like Dave, Albert, Brigit, Cleo, EarnIn, Empower, FloatMe, and MoneyLion. Now, every time I get paid, most of my check goes toward paying them back, leaving me with almost nothing—so I end up borrowing again. It feels like a cycle I can’t break. Does anyone know the best way to handle this.

- entry_id: REDDIT-0084
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

- entry_id: REDDIT-0085
  title: "PAYMENT OF TILT’S MONTHLY SUBSCRIPTION FEE IS OPTIONAL"
  date: 2026-04-08
  score: 30
  type: post
  providers: [Tilt]
  topics: [SUBSCRIPTION_FEES]
  url: https://www.reddit.comhttps://www.reddit.com/r/cashadvanceapps/comments/1sg7nvc/payment_of_tilts_monthly_subscription_fee_is/
  text: |
    I know we humans never really read the terms of service before fully agreeing,.. and so do they. This nugget is tucked somewhere towards the middle:
    
      
    ” Access to Tilt Advance requires a subscription, however, you may access Tilt Advance (as well as the Tilt Checking Account) without paying a subscription fee. To do so, please email  [help@tilt.com](mailto:help@tilt.com) and state that you would like your subscription fee waived.”
    
      
    spread the good word ✌️

```