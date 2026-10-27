# Precision targeting stack: paid platforms and data activation for reaching named fund buyers in the UK and Europe (status at 27 October 2026)

> **Method and limitations (read first).**
>
> - **No full-page reads.** Page retrieval did not work in this session. WebFetch returned DNS errors for every domain tried. The egress proxy returned HTTP 403 for direct requests to linkedin.com, support.google.com, ppc.land and b2linked.com. Every finding below therefore comes from search-engine extracts of the cited pages, not full-page reads.
> - **Unresearched areas.** The session-wide web-search budget also ran out partway through. These areas could not be researched and are listed under Gaps:
>   - programmatic B2B data marketplaces and cookieless IDs;
>   - clean rooms and CRM-to-ad connectors beyond LinkedIn;
>   - personalisation and orchestration vendors (Mutiny, Folloze, Uberflip, Hushly, Vidyard, Sendspark);
>   - job-change tools, Influ2, Lead Forensics and Albacross;
>   - asset-manager ABM case studies.
> - **Background knowledge** appears only in Gaps, labelled *unverified (training knowledge, pre-June 2026)*. It must be checked before use.
> - **Cost and pricing figures** are mostly from vendor or agency blogs, often written by competitors. Treat them as directional.

## 1. LinkedIn Ads (2025–2026 state): targeting facets, formats, EU restrictions, ABM features and costs

### Takeaway
LinkedIn is still the core paid channel that can isolate named fund-buying firms and the roles inside them at scale. Microsoft borrows LinkedIn data, but only in the UK, France and Germany.

In late 2026 LinkedIn's precision is limited by six things:
- a 300-matched-member minimum per campaign;
- Lookalikes are gone, and the replacement (Predictive Audiences) needs a seed of at least 300;
- Audience Expansion now defaults on, because the AI campaign type "Accelerate" was folded into Classic campaigns on 4 August 2026 (single source);
- Thought Leader Ads cannot promote documents or run on lead-gen or website-visit objectives;
- in the EEA and Switzerland, Sponsored Messaging reaches only members who opted in;
- since June 2024, Group-membership targeting has been off for EU members under the DSA.

Vendor datasets put median B2B CPMs at about $57 in the UK and €74 in Western Europe, with finance among the most expensive verticals.

### Cited Findings

**Targeting building blocks**
- LinkedIn's "V2" industry taxonomy was rolled out in 2023. It has 434 industries in a hierarchy of 20 top-level groups, and the same codes are used in ad targeting, exports and APIs — [jobspipe.dev](https://jobspipe.dev/blog/linkedin-industries-list).
- The Financial Services branch has 4 second-level and 15 third-level industries — [classification.codes](https://classification.codes/classifications/industry/linkedin). The exact labels (for example "Investment Management") could not be verified; see Gaps.
- 2026 agency ABM guides agree on three practices: target several roles per account rather than single individuals; exclude your own employees and competitors; and add job function and seniority filters on top of company lists. One guide suggests lists of 50–500 accounts — [Vizion](https://www.vizion.com/blog/linkedin-abm-targeting-guide-2026-what-works-what-doesnt-how-to-reach-b2b-buying-committees/); [Single Grain](https://www.singlegrain.com/abm/linkedin-abm-framework-for-targeting-bidding-and-timing/).

**Matched Audiences (company lists, contact lists, CRM sync)**
- **Minimum and recommended audience sizes:**
  - A campaign needs at least 300 audience members to run. LinkedIn recommends "50,000 or more for single image and text ads and over 15,000 for message ads" — [LinkedIn Marketing Solutions](https://business.linkedin.com/advertise/ads/audience).
  - LinkedIn's API documentation says the 300 threshold "ensures that there is enough impression data for the system to properly assess its effectiveness" — [Microsoft Learn: LinkedIn Marketing API](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/getting-started?view=li-lms-2025-01).
  - An older third-party article recommends 300,000+ for Sponsored Content and Sponsored Messaging — [MarketingProfs, 2023](https://www.marketingprofs.com/articles/2023/50624/linkedin-advertising-strategy-tips-benchmarks).
- **How LinkedIn measures match rate:** it is the share of uploaded entries that matched a member account or Page in the past seven days. If a list matched fewer than 300 member accounts, LinkedIn shows "under 5%". Duplicate entries shrink the final audience — [LinkedIn Help: Matched Audiences match rates](https://www.linkedin.com/help/lms/answer/a420595).
- **Typical match rates:**
  - Company lists: **60–90%**. Firms with active LinkedIn Pages match more often, while "small companies, very new companies, or companies with common names may not match" — [ZenABM](https://zenabm.com/blog/linkedin-matched-audiences).
  - Contact lists: typically **30–70%**. Contact targeting only matches members with verified email addresses — [ZenABM](https://zenabm.com/blog/linkedin-contact-targeting); [LinkedIn Help](https://www.linkedin.com/help/lms/answer/a420595).
- **Improving matches:** adding LinkedIn Company Page URLs and website domains alongside company names improves both accuracy and match rate — [B2Linked](https://b2linked.com/blog/best-match-rates-linkedin-ads/); [Vector](https://www.vector.co/compare/improve-your-linkedin-audience-match-rate).
- **Sync time:** LinkedIn can take up to 24 hours to process a synced list, depending on list size — [Gartner support FAQ](https://support.ops.gartner.com/support/solutions/articles/70000640455-linkedin-faqs).
- **CRM connectors:**
  - LeadsBridge builds LinkedIn audiences from Salesforce leads, campaign members and report or list views — [LeadsBridge](https://leadsbridge.com/integrations/salesforce/linkedin-matched-audiences).
  - A Make.com template syncs HubSpot to LinkedIn every 15 minutes. Linking contacts to a company improves matching — [Make](https://make.com/en/integrations/linkedin-matched-audiences).
  - No source confirmed a native Dynamics 365 or LiveRamp sync (see Gaps).
- **ABM pain point:** practitioners openly trade workarounds for the 300-member minimum — [Clay community](https://community.clay.com/x/general/kxegkn1ykbjv/how-to-overcome-linkedin-ads-300-member-minimum-au).

**Predictive Audiences (Lookalikes retired)**
- LinkedIn retired Lookalike Audiences in early 2024. No new lookalikes can be created, and existing ones cannot be edited or refreshed. LinkedIn now points advertisers to Predictive Audiences (built from contact lists, conversions or Lead Gen Form data) and to Audience Expansion — [DestinationCRM](https://www.destinationcrm.com/Articles/CRM-News/CRM-Featured-Articles/LinkedIn-Ends-Lookalike-Audiences-162839.aspx); [Single Grain](https://www.singlegrain.com/blog/n/linkedin-lookalike-audiences/); [Coinbound](https://coinbound.io/linkedin-bids-farewell-to-lookalike-audiences-introduces-new-targeting-tactics/).
- Predictive Audience rules, according to third-party guides — [Edelman](https://www.edelman.com/insights/evolution-linkedin-audience-expansion-tools); [ZenABM](https://zenabm.com/blog/linkedin-ads-minimum-audience-size); [LinkedIn Ads Show ep. 141](https://linkedinads.libsyn.com/linkedin-ads-predictive-audiences-ep-141):
  - The seed must have at least 300 members: contact lists of 300–300,000 rows, or more than 300 converters or Lead Gen Form submitters.
  - Each ad account can hold at most 30, and they cannot be shared across accounts.
  - Audience Expansion cannot be switched on for them.
  - As one guide puts it, "building a lookalike from a 50-account list will not work anymore."

**Audience Expansion, Accelerate (AI campaigns) and LinkedIn Audience Network**
- **Accelerate was retired as a standalone campaign type on 4 August 2026** — [Magnet.co](https://www.magnet.co/posts/audience-expansion-is-on-until-you-say-no). This comes from a single third-party source citing LinkedIn's Help Center and is unverified.
  - Existing Accelerate campaigns keep running, but from 5 January 2027 their run dates cannot be extended and budget cannot be added.
  - Accelerate's creation tools now sit in standard Classic campaigns: audience building, expansion, placements, bidding and "Draft with AI".
  - **Audience Expansion is now switched on automatically wherever it is available.**
- **What Accelerate did:** it used AI to build a whole campaign from the advertiser's website URL, LinkedIn Page and past ads. LinkedIn reported 15% faster campaign creation and 52% lower cost per action than Classic campaigns — [MediaPost](https://www.mediapost.com/publications/article/397611/linkedin-expands-access-to-accelerate-ai-campaig.html); [Social Media Today](https://www.socialmediatoday.com/news/linkedins-making-its-automated-accelerate-campaigns-available-to-all-bra/721174/).
- **LinkedIn Audience Network (LAN):**
  - It tends to underperform for high-value B2B offers, tight budgets and niche targeting, producing "expensive clicks wasted on consumer browsing" — [Opteo](https://opteo.com/docs/en/articles/12269607-disable-audience-network-in-linkedin-ads).
  - A LinkedIn-ads agency advises turning it off by default, warns that it inflates metrics, and says to test it only with a block list — [B2Linked](https://b2linked.com/blog-page/the-hidden-linkedin-ads-setting-that-burns-your-budget).
  - Custom block lists are supported — [ITBusiness](https://www.itbusiness.ca/?p=94660).

**Thought Leader Ads (sponsoring portfolio managers' and others' own posts)**
- **History:** launched in June 2023 for employees' posts. Expanded in March 2024 to any member's post, with that member's permission — [Social Media Today](https://www.socialmediatoday.com/news/linkedin-will-now-enable-brands-to-sponsor-any-organic-post-in-the-app/710255/); [CMSWire](https://www.cmswire.com/the-wire/companies-can-now-promote-member-content-with-linkedin-thought-leader-ads); [JoinValley](https://www.joinvalley.co/blog/linkedin-thought-leader-ads).
- **How it works:**
  - The author approves or declines each sponsorship request and is not paid.
  - The ad carries a "promoted" transparency label.
  - The advertiser needs Super admin, Content admin or Sponsored Content poster rights on its Company Page, but no access to the author's ad account — [JoinValley](https://www.joinvalley.co/blog/linkedin-thought-leader-ads).
  - Sources disagree on whose posts qualify: one says employees plus 1st- and 2nd-degree connections, another says any member who grants permission — [JoinValley](https://www.joinvalley.co/blog/linkedin-thought-leader-ads); [Make Influence](https://www.makeinfluence.com/en/academy/linkedin-creator-marketplace-and-thought-leader-ads-explained).
- **Restrictions** — [B2B Ads](https://b2bads.com/linkedin-thought-leader-ads); [ZenABM TLA guide](https://zenabm.com/blog/linkedin-thought-leader-ads-ultimate-guide); [JoinValley](https://www.joinvalley.co/blog/linkedin-thought-leader-ads):
  - Ineligible post types: celebrations, **documents**, polls, multi-image posts and reshares.
  - Allowed objectives: Brand Awareness and Engagement, plus Video Views for video posts.
  - Not allowed: Lead Generation, Website Visits and Website Conversions.
  - The post runs exactly as written, with no added headline, intro text or call-to-action button.
  - One UK agency recommends website-visit or lead-gen objectives for these ads — [Fill My Funnel](https://www.fillmyfunnel.co.uk/turning-your-ceos-posts-into-thought-leader-ads/). This conflicts with the other sources and is likely wrong.
- **Updates since late 2025:**
  - Late 2025: a Campaign Manager discovery tool finds posts that mention your brand or event from 1st-, 2nd- and 3rd-degree members, with an automated permission request — [Social Media Today](https://www.socialmediatoday.com/news/linkedin-thought-leader-ads-discovery-campaign-manager/804325/).
  - 2026: brands can sponsor non-employees (contractors, advisers and other outside voices), and an event version sponsors member posts that link to LinkedIn Event pages — [TripleDart](https://www.tripledart.com/guides/linkedin-thought-leader-ads-guide); [Postiv](https://postiv.ai/blog/linkedin-thought-leadership-ads).
  - July 2026: new AI creative tools, not confirmed for Thought Leader Ads specifically. September 2026: new LinkedIn guidance on Thought Leader Ads — [HeyOrca monthly LinkedIn roundup](https://www.heyorca.com/blog/linkedin-social-news).
- **Performance claims:** a claim of about 2x higher CTR, attributed to LinkedIn, is widely repeated. Agency claims of 3x or "31.8x" are unverified — [TripleDart](https://www.tripledart.com/guides/linkedin-thought-leader-ads-guide); [Fractional Demand](https://fractionaldemand.com/resources/blog/thought-leader-ads-2026).

**Sponsored Messaging (Message Ads and Conversation Ads): EU, EEA and Switzerland vs the UK**
- **History:** LinkedIn stopped EU-targeted Sponsored Messaging for new campaigns on 15 December 2021 and paused existing ones from January 2022 — [Root Agency](https://rootagency.be/linkedin-disables-sponsored-messages-in-europe-what-linkedin-advertisers-need-to-know/); [Blog du Modérateur](https://www.blogdumoderateur.com/linkedin-arrete-messages-prives-sponsorises-europe/); [Waalaxy](https://blog.waalaxy.com/en/linkedin-sponsored-messages/).
- **Current rule:** LinkedIn's help page says it supports EEA and Switzerland targeting for message and conversation ad sets, but "only members there who opted in to see Sponsored Messaging ads in their inbox will receive them" — [LinkedIn Help: Message ads specifications](https://www.linkedin.com/help/lms/answer/a427509).
- **Practical effect:**
  - The opt-in arrived with a consent prompt in August 2024. Advertisers cannot see how many members have opted in — [DemandSense](https://demandsense.com/blog/linkedin-conversation-ads-vs-message-ads).
  - One agency advises checking what share of a target list sits in the EEA or Switzerland before planning — [Moriah](https://www.moriah.ai/blog/linkedin-marketing/linkedin-message-ads).
  - Another source says Conversation Ads cannot reach EU/EEA members without explicit opt-in. It also claims Message Ads are no longer available for new campaigns, which is unconfirmed — [Stackmatix](https://www.stackmatix.com/blog/linkedin-conversation-ads-best-practices).
- **UK:** none of the sources mentions the UK (see Inferences).

**EU-specific restrictions (DSA, data use)**
- **Group targeting removed for EU users (June 2024).** LinkedIn stopped advertisers building audiences from LinkedIn Group membership for EU users.
  - This followed a European Commission request for information, prompted by a civil-society complaint. The complaint argued that Group membership could reveal special-category data (for example political, religious or trade-union affiliations) protected under GDPR Article 9(1).
  - LinkedIn disagreed but removed the option anyway: "The change is effective now for all new advertising campaigns."
  - Commissioner Breton welcomed the move on 7 June 2024, and the Commission later closed the case.
  - Sources: [PPC Land](https://ppc.land/linkedin-discontinues-group-based-ad-targeting-to-comply-with-dsa/); [Bits of Freedom](https://bitsoffreedom.nl/2024/06/27/linkedin-restricts-ad-targeting-after-our-complaint); [Silicon UK](https://www.silicon.co.uk/e-regulation/surveillance/linkedin-targeting-feature-ad-567261); [iEU Monitoring](https://ieu-monitoring.com/editorial/eu-commissioner-breton-welcomes-announcement-by-linkedin-to-comply-with-dsa-ad-provisions/436027/); [Digital Policy Alert](https://digitalpolicyalert.org/event/20478-closed-european-commission-case-following-linkedin-discontinuation-of-targeted-ads-based-on-sensitive-personal-data).
- **Data sharing with Microsoft (from 3 November 2025).** LinkedIn began sharing more member data with Microsoft group companies for ad personalisation: profile data, feed activity and ad engagement.
  - This applies in the US and most other regions, but **not in the EU, UK or Switzerland** — [Gulf News](https://gulfnews.com/technology/linkedin-privacy-update-microsoft-can-use-your-data-from-nov-3-how-to-stop-it-1.500281615); [Malwarebytes](https://www.malwarebytes.com/blog/news/2025/09/linkedin-will-use-your-data-to-train-its-ai-unless-you-opt-out-now).
  - A separate change, using member data to train AI, covered EU, EEA and Swiss members and reportedly UK members too — [The Register](https://www.theregister.com/2025/10/27/linkedin_ai_profile_scraping).

**ABM features: Buyer Group targeting and the Companies tab**
- **Buyer Group targeting** (reported launch 5 February 2026) — [ABM Agency](https://abmagency.com/linkedin-abm-news-today-updated-ad-targeting-options-for-account-based-campaigns-recency-update/amp/):
  - Instead of combining titles and seniority by hand, advertisers pick a predefined cluster of decision-makers, such as an "IT Buying Committee".
  - Beta claims of cost per lead falling from $145 to $112 and account coverage rising from 65% to 92% are unverified.
  - LinkedIn "identifies clusters of professionals within the same company who are likely involved in purchasing decisions for a given product category". The option appears under target audience as "add buyer groups". The templates are built for typical buying situations, so manual targeting can still win for unusual committees — [Optimize LinkedIn Ads](https://www.optimizelinkedinads.com/blogs/linkedin-buyer-group-targeting-ads-guide).
  - It is described as available to all advertisers globally — [B2Linked ep. 165](https://b2linked.com/blog/ep165); [Vizion](https://www.vizion.com/blog/linkedin-abm-targeting-guide-2026-what-works-what-doesnt-how-to-reach-b2b-buying-committees/).
- **"Companies Hub":** only one source describes it, as a place to upload account lists and see how deeply you have reached each one. Unverified — [LinkBoost](https://www.linkboost.co/blog/linkedin-account-based-marketing-guide-2026/).
- **Company Engagement Report** (launched 2020, free) — [LinkedIn Marketing Blog, 2020](https://business.linkedin.com/marketing-solutions/blog/linkedin-news/2020/company-engagement-reports-on-linkedin-are-here-to-power-up-your); [Social Samosa](https://www.socialsamosa.com/2020/11/linkedin-the-company-engagement-report-b2b-marketers):
  - It scores each account's "Total engagement level": ad engagement plus organic engagement plus website visits, divided by the number of members targeted, and benchmarked across companies.
  - At launch it required an uploaded account list matching more than 300 members.
- **Companies tab:** since 2024 the report sits under Plan > Companies. It needs a connected LinkedIn Page and adds up results by account rather than by campaign — [ZenABM](https://zenabm.com/blog/see-companies-engaging-with-linkedin-ads).

**Video, CTV and BrandLink**
- **BrandLink** places advertisers' videos alongside publisher video content — [Social Samosa](https://www.socialsamosa.com/news-2/linkedin-expands-brandlink-programme-ctv-advertising-11248078); [The Keyword](https://www.thekeyword.co/news/linkedin-ctv-trade-desk-b2b-advertising):
  - It is self-serve in Campaign Manager for selected advertisers.
  - It now includes pre-roll on live events from more than 40 publishers, including Axel Springer, TIME and Times Network.
- **Buying LinkedIn CTV (connected TV) ads:**
  - Directly in Campaign Manager, or programmatically through The Trade Desk, which runs on Microsoft Monetize — [Social Samosa](https://www.socialsamosa.com/news-2/linkedin-expands-brandlink-programme-ctv-advertising-11248078).
  - Through Amazon DSP, since a partnership announced in May 2026 — [Marketing Dive](https://www.marketingdive.com/news/amazon-linkedin-help-advertisers-reach-professionals-via-ctv-ads/819372/); [eMarketer](https://www.emarketer.com/content/linkedin-amazon-ads-give-b2b-marketers-new-path-ctv).
  - LinkedIn job-title targeting also reaches Google DV360 CTV buys, but only in the US — [PPC Land headline](https://ppc.land/linkedin-job-title-targeting-reaches-google-dv360-ctv-buys-in-the-us/).
- **UK availability of CTV is unclear:**
  - One benchmark says UK inventory arrived in 2026; 2 of the 31 accounts it studied targeted the UK — [Kiin](https://kiin.co/research/linkedin-ctv-ads-benchmarks).
  - A Belgian agency says CTV targeting works only in the US and Canada — [Customer Impact](https://www.customerimpact.be/en/blog/linkedin-connected-tv-ads/).

**Cost and performance benchmarks (all vendor or agency data; directional)**
- **By country.** A 2026 dataset of 211 B2B companies across 29 countries gives median CPMs of **UK $56.62**, US $62.67 and Netherlands $50.08 — [ZenABM](https://zenabm.com/blog/linkedin-ads-benchmarks-2026).
- **Netherlands and Western Europe.** Median LinkedIn CPM was **€73.83 in 2025**, up 185% from €25.92 in the previous benchmark — [Merkelijkheid via Searchlab](https://searchlab.nl/statistieken/linkedin-ads-statistieken-2026).
- **UK cost per click.** Typical UK B2B CPCs are £5–£12 for mid-level professionals — [ProfileTree](https://profiletree.com/linkedin-ads-a-guide-to-targeting-professionals/).
- **Financial services.** 2026 blog estimates vary widely — [Datavinity](https://datavinity.com/en/linkedin-ads-benchmarks-2026/); [Postiv](https://postiv.ai/blog/linkedin-advertising-costs); [Ryze](https://www.get-ryze.ai/blog/linkedin-ads-cpc-and-cpl-benchmarks-by-industry-2026); [Benly](https://benly.ai/learn/linkedin-ads/linkedin-ads-benchmarks); [Stackmatix](https://www.stackmatix.com/blog/linkedin-ads-cost); [Meet Lea](https://meet-lea.com/en/blog/linkedin-advertising-costs-roi-benchmarks):
  - CPC from $2.59–6.00 (Datavinity) up to $7.80–15.20.
  - Cost per lead about $90–220.
  - CPM about $35–50.
  - CTR 0.35–0.65%.
  - Finance ranks among the most expensive verticals; the platform-wide average CPC is about $6.50.
- **Funnel benchmarks (2025):**
  - Top of funnel: CTR 0.45–0.9%, CPC $8–15, CPM $50–90 — [Sales-mind](https://sales-mind.ai/en/blog/post/2025-sales-funnel-benchmarks-linkedin).
  - Awareness: median CPM $31; CTR 0.50–0.60% for single-image ads and 0.40% for video — [Nav43](https://nav43.com/blog/2025-linkedin-ads-benchmarks-every-saas-tech-marketer-needs).
- **Dreamdata LinkedIn Ads Benchmarks 2025** (published 8 September 2025; 23 million sessions and 220,000+ customer journeys) — [Dreamdata](https://dreamdata.io/linkedin-ads-b2b-benchmarks):
  - LinkedIn's return on ad spend was 113% ([PPC Land](https://ppc.land/linkedin-emerges-as-top-b2b-platform-with-113-roas-and-211-day-buyer-journeys/)) or 121% ([NetInfluencer](https://www.netinfluencer.com/linkedin-ads-deliver-highest-return-among-major-ad-networks-research-finds/)), against 67% for Google Search and 51% for Meta.
  - B2B buyer journeys averaged 211 days ([PPC Land](https://ppc.land/linkedin-emerges-as-top-b2b-platform-with-113-roas-and-211-day-buyer-journeys/)).
  - LinkedIn took about 39% of total B2B ad spend ([eCommerceNews](https://ecommercenews.co.nz/story/linkedin-emerges-as-top-b2b-ad-channel-with-highest-returns)) and 41% of paid-social budgets in 2025 ([NetInfluencer](https://www.netinfluencer.com/linkedin-ads-deliver-highest-return-among-major-ad-networks-research-finds/)).

**Financial-services and asset-manager examples**
- **LinkedIn's own case-study hub** — [LinkedIn case studies](https://business.linkedin.com/marketing-solutions/success/marketing-case-studies); [LinkedIn Success Hub](https://business.linkedin.com/advertise/customer-stories):
  - "One of the world's largest asset managers" (unnamed) reportedly gained new deposits worth 5,454x the campaign cost. No method is given.
  - J.P. Morgan Asset Management used Sponsored Content and tailored journeys to re-engage financial advisers.
  - BlackRock nurtured a niche alternative-investments audience.
- **GK3 Capital (agency)** — [GK3](https://www.gk3capital.com/insights/how-a-premier-asset-manager-raised-nearly-40m-with-linkedin-advertising); [GK3 guide](https://www.gk3capital.com/insights/linkedin-ads-for-asset-managers?hs_amp=true):
  - A real-estate fund sponsor promoted a Qualified Opportunity Zone eBook to US advisers ahead of a tax deadline, using LinkedIn's pre-filled lead forms. Leads arrived in real time and sales followed up quickly.
  - Another client raised "nearly $40M" with LinkedIn as a main distribution channel. No costs were shown.
- **HomeTree Digital (agency):** a six-month campaign for a multi-affiliate asset manager targeted US financial advisers with lead-form ads, retargeting and weekly reporting. The results were not captured — [HomeTree](https://hometreedigital.com/insights/case-study-linkedin-ads-targeting-financial-advisors/).

### Inferences
- **Core build for a boutique UCITS manager.**
  - Upload a list of 500–3,000 firms, with company name, LinkedIn Page URL and website domain for each.
  - Combine the list with job function, seniority and title filters.
  - Exclude your own staff. Exclude other asset managers' employees except where they are prospects (for example, fund-of-funds teams).
  - At the reported 60–90% company match rate, 3,000 firms would give roughly 1,800–2,700 matched companies.
  - Small IFA practices are the least likely to match. Reach them separately with UK title and industry targeting, testing titles such as financial adviser, chartered financial planner and paraplanner (not verified in LinkedIn's title list).
- **No 1:1 targeting of small firms; build 1:few clusters instead.**
  - A five-person IFA firm cannot be targeted on its own under the 300-member minimum. You need about 60 such firms (300 ÷ 5) pooled in one ad set.
  - The practical unit is a cluster of at least 300 matched members, for example:
    - UK discretionary managers' model portfolio (DFM/MPS) teams;
    - UK platform fund-list teams;
    - Swiss external asset managers;
    - French CGP networks;
    - Italian consulenti networks;
    - German Vermögensverwalter;
    - Spanish EAFs;
    - private-bank fund selectors by country.
  - Clusters also let you localise creative and language for each group, which helps financial-promotion sign-off.
  - Large banks, insurers and platforms with 300+ matched members can be targeted individually.
- **Precision hygiene after the Accelerate change.** Audience Expansion reportedly now defaults on, so check every ad set. Turn off both Audience Expansion and LinkedIn Audience Network for named-account work. Do not rely on Predictive Audiences until there are at least 300 seed converters.
- **Thought Leader Ads as the "people, not logos" layer.**
  - Sponsor portfolio managers' own text, image or video posts to the company-list clusters, using Awareness, Engagement or Video Views objectives.
  - Because these ads cannot carry documents, retarget people who engaged or watched videos with standard Sponsored Content or Document Ads plus Lead Gen Forms. These can gate factsheets or whitepapers; Document Ad gating was not re-checked this session. In the UK, follow with Conversation Ads.
  - The discovery tool can also surface organic posts by clients, gatekeepers or fund raters that mention the fund or an event. Sponsoring them needs the author's approval and a compliance review of third-party content as a financial promotion (flag for the compliance researcher).
- **UK vs EU split for messaging.** The opt-in rule covers the EEA and Switzerland. The UK is outside the EEA, so UK members should still receive Message and Conversation Ads under normal rules. No source confirms this, so check it in Campaign Manager. Treat Sponsored Messaging reach in the EEA and Switzerland as an unpredictable bonus.
- **Group targeting.** EU members can no longer be targeted through fund-selector, CFA-society or adviser-community Groups. Whether UK members can still be targeted this way is unverified. The DSA does not apply in the UK, but LinkedIn may have removed the option more widely.
- **Budget arithmetic** (using the cited medians; senior finance audiences probably cost more):
  - 10,000 targeted members seeing 4 impressions a month is 40,000 impressions.
  - At the $56.62 UK median CPM that costs **about $2,265 a month**; at the €73.83 Western European median, **about €2,953 a month**.
  - A three-month surround sequence on that audience therefore costs roughly $6,800 (UK) or €8,900 (Western Europe) in media, before Thought Leader Ads and retargeting.
  - That is affordable for a boutique, so the real limit is audience size, not budget.
- **GDPR risk flags:**
  - **Low:** targeting on LinkedIn's own member attributes and company lists (company names are not personal data).
  - **Medium:** uploading contact lists (hashed emails). This needs a lawful basis, a privacy-notice disclosure and clean CRM data.
  - **Medium:** retargeting website visitors with the LinkedIn Insight Tag, which needs cookie consent under PECR in the UK and ePrivacy rules in the EU.
  - **Low for the advertiser:** Sponsored Messaging in the EEA and Switzerland, because LinkedIn manages the opt-in.

### Gaps
- LinkedIn help-centre pages could not be opened (proxy 403), so no LinkedIn facts were checked against full text. LinkedIn also publishes a GDPR guide for advertisers that could not be retrieved — [LinkedIn Help: LMS and GDPR](https://www.linkedin.com/help/lms/answer/a1444756/linkedin-marketing-solutions-and-the-general-data-protection-regulation-gdpr-?lang=en).
- **Targeting options to check in Campaign Manager's audience forecaster** (not verified this session):
  - specific Skills entries (for example "Fund Selection", "Portfolio Construction", "Investment Research");
  - Member Interests;
  - standardised titles such as "Paraplanner", "Fund Selector", "Discretionary Fund Manager", "Conseiller en gestion de patrimoine" and "Consulente finanziario";
  - the exact Financial Services industry labels in the V2 taxonomy.
- **Formats not researched (search budget ran out).** *Unverified background (training knowledge, pre-June 2026):*
  - Document Ads allow a preview before gating the rest behind a Lead Gen Form.
  - Lead Gen Forms support hidden fields and CRM or marketing-automation integrations.
  - The Conversions API launched in 2023 and supports server-side and CRM conversion uploads. Integrations were reported to include HubSpot, Salesforce, Dynamics 365, Marketo, LiveRamp and Google Tag Manager server-side.
  - Event Ads promote LinkedIn Events.
  - LinkedIn Live needs eligibility and approval.
- **Minimum daily budget:** not found. *Unverified background:* about $10 a day.
- **Senior-audience costs:** no UK- or EU-specific CPM or CPC benchmark was found for senior fund-selector or investment-management audiences.
- **Buyer Group templates:** it is unknown whether any template covers finance or investment buying committees.
- **Message Ads as a format:** conflicting. Stackmatix says it is retired for new campaigns, while LinkedIn's help still documents it.
- **European case studies:** no UK or European asset-manager LinkedIn case study with numbers was found. The cited examples are US or unnamed.

## 2. Microsoft Advertising: LinkedIn profile targeting, Audience Network, Invest DSP sunset

### Takeaway
Microsoft Ads can add LinkedIn company, industry and job-function data to search ads and to native or display "Audience ads". In Europe this works only for campaigns targeting the UK, France and Germany. The new seniority option (June 2026) excludes those three markets.

Microsoft Audience Network (MSAN) still operates; Microsoft's 2026 product notes call the placement inventory the "Microsoft Advertising Network". Microsoft's demand-side platform, Microsoft Invest (formerly Xandr), shut on 28 February 2026. Microsoft kept its sell-side tools, Curate and Monetize.

### Cited Findings
- **Markets.** Microsoft says LinkedIn Profile Targeting "is available to advertisers located anywhere in the world, [but] it can only be used on campaigns targeting the following markets: United States, United Kingdom, Canada, Australia, France and Germany" — [Microsoft Advertising](https://Advertising.Microsoft.com/en-us/solutions/Audience-targeting/LinkedIn-Profile-Targeting).
- **What you can target.** The 2020 launch added job function, industry and company targeting to Search and Audience campaigns in the US, Canada, UK, Australia, France and Germany — [Microsoft Advertising blog, Sept 2020](https://about.ads.microsoft.com/en-us/blog/post/september-2020/dynamic-remarketing-linkedin-profile-targeting-in-market-are-here); [Search Engine Land](https://searchengineland.com/microsoft-advertising-expands-linkedin-profile-dynamic-remarketing-in-market-audience-targeting-340246). The same LinkedIn data was later offered to Performance Max campaigns in those six markets, as audience *signals* (guidance) rather than strict targeting — [Social Media Today](https://www.socialmediatoday.com/news/microsoft-performance-max-linkedin-data/739335/).
- **Job seniority (added mid-June 2026; sources give 15, 16 or 17 June)** — [PPC Land](https://ppc.land/microsoft-advertising-adds-job-seniority-to-linkedin-profile-targeting/); [Start Some Shift](https://startsomeshift.com/news/microsoft-advertising-linkedin-job-seniority-targeting/); [Business News UK](https://www.business-news.org.uk/microsoft-ads-expands-linkedin-targeting-with-job-seniority-filters/); [Digital Applied](https://www.digitalapplied.com/blog/microsoft-ads-linkedin-job-seniority-targeting-2026-b2b-guide):
  - Available on Search and Audience campaigns, at campaign or ad-group level.
  - 10 seniority levels, each with its own bid adjustment.
  - 29 markets (one source says 23) across the Americas, four EMEA countries and Asia-Pacific. **The UK, Germany and France are not included.**
  - One source reports that job seniority and AI Max for Search became generally available on 31 August 2026. No later market expansion was found.
- **Audience Network in 2026:**
  - **January 2026:** Content Targeting for Audience ads became generally available. Placement targeting runs only on premium Microsoft properties (MSN, Outlook, Microsoft Casual Games and Microsoft Edge). Topic targeting runs by content category, such as Finance — [Microsoft Advertising, January 2026](https://about.ads.microsoft.com/en/blog/post/january-2026/performance-max-updates-and-other-product-news-for-january-2026).
  - **February 2026:** a new preview hub shows how Audience ads "can appear across the Microsoft Advertising Network" — [Microsoft Advertising, February 2026](https://about.ads.microsoft.com/en/blog/post/february-2026/ad-preview-hub-and-other-product-news-for-february-2026).
  - **September 2026:** a third-party roundup still lists the Microsoft Audience Network alongside exclusive search partners (Yahoo, DuckDuckGo, Ecosia), video, retail media, programmatic and gaming — [MEAN CEO](https://blog.mean.ceo/microsoft-advertising-news-september-2026/).
  - An agency calls MSAN "the only native/display inventory where advertisers can target by LinkedIn Company, Industry, Job Function, and Job Seniority" — [MB Adv](https://www.mbadv.agency/microsoft-ads/microsoft-audience-network).
  - No report of MSAN being retired was found. The retirement Microsoft did announce (on 24 November 2025) was of its Microsoft Advertising mobile app, from January 2026 — [Search Engine Land](https://searchengineland.com/microsoft-to-retire-its-advertising-mobile-app-in-early-2026-464970).
- **Microsoft Invest (formerly Xandr) shut on 28 February 2026** — [MediaPost](https://www.mediapost.com/publications/article/409701/microsoft-leans-on-amazon-for-its-demand-side-plat.html); [Search Engine Land](https://searchengineland.com/microsoft-amazon-dsp-preferred-partner-463066); [Social Samosa](https://www.socialsamosa.com/news-2/microsoft-retires-xandr-dsp-9070287); [AI Digital](https://www.aidigital.com/blog/microsoft-sunsets-xandr-what-it-means-for-marketers); [Media in Canada](https://mediaincanada.com/2025/05/23/microsoft-dsp-ai):
  - Announced in May 2025.
  - Microsoft is focusing on three products: the Microsoft Advertising Platform, Monetize (its supply-side platform) and Curate (sell-side curation).
  - Amazon DSP was named the preferred partner for moving campaigns.
  - Microsoft said its "commitment to more private and personalised advertising experiences for a conversational and agentic world is not achievable with the industry's current DSP model."
- **Link to LinkedIn CTV:** LinkedIn's programmatic CTV through The Trade Desk runs on Microsoft Monetize — [Social Samosa](https://www.socialsamosa.com/news-2/linkedin-expands-brandlink-programme-ctv-advertising-11248078).

### Inferences
- **UK, France and Germany: a cheap precision layer.** Microsoft Search and Audience ads can be limited to LinkedIn-identified target companies, industries and job functions, but not seniority in these markets.
  - On search, this captures queries for fund names, ISINs, share classes and sector names from people at named fund-buying firms. It also helps protect your brand and fund-name keywords.
  - On Audience ads (MSN, Outlook, Edge), it adds a low-cost layer of extra exposure. Finance topic targeting can be layered with LinkedIn company targeting; this combination is unconfirmed, so test it.
- **Other European markets: no LinkedIn data on Microsoft.** For Switzerland, Italy, Spain, Luxembourg, Ireland, the Netherlands and the Nordics, Microsoft offers only standard search and audience targeting. Precision there must come from LinkedIn itself.
- **Low data-protection risk.** LinkedIn profile targeting on Microsoft uses data the platforms already hold, with nothing uploaded by the advertiser, so the advertiser's GDPR exposure is low. Microsoft's conversion tracking tag (UET) still needs cookie consent.
- **Programmatic.** The Invest shutdown removes Microsoft's own buying route, so programmatic B2B buying must go through other DSPs (see section 5). Microsoft Curate remains relevant only as a source of curated deals from the sell side.
- **Out of scope.** Copilot and AI-assistant ads belong to another researcher. They matter here only as context, because Microsoft explained the DSP exit in terms of "conversational and agentic" advertising.

### Gaps
- **Costs:** no CPC or CPM benchmarks were found for Microsoft search or Audience ads with LinkedIn profile targeting in the UK, France or Germany, or for financial-services keywords.
- **Unconfirmed status:**
  - whether "Microsoft Advertising Network" is a formal new name for MSAN;
  - whether seniority targeting has reached the UK, France or Germany since June 2026.
- **Not documented in the search results:** minimum audience sizes for LinkedIn profile targeting on Microsoft, and how well LinkedIn company targeting matches small IFA firms.

## 3. Google: Customer Match, custom segments, Demand Gen and YouTube, Performance Max risk, financial-services verification, competitor-fund keywords and cookie status

### Takeaway
Google's B2B precision comes from intent signals (search terms, custom segments and first-party lists), not from firm or job-role data.

For a boutique:
- **Customer Match** (targeting your own uploaded contacts) may be restricted by spend and account-history thresholds. For EEA users it also needs explicit consent signals with every upload.
- **Lookalike segments** need at least 1,000 matched seed contacts, which rules them out for most fund-buyer lists.
- **Financial-services verification** has been compulsory across most EU and EEA markets since 23 July 2026, and in the UK since 2021.
- **Chrome third-party cookies** survive, but Google's Privacy Sandbox advertising tools have been retired.

### Cited Findings
- **Customer Match eligibility:**
  - Google's policy page names "two essential requirements": "a good track record of policy compliance and a good payment record" — [Google Ads Help: Customer Match policy](https://support.google.com/google-ads/answer/6299717?hl=en-GB).
  - Third-party guides still say full targeting needs **at least 90 days of account history and more than USD 50,000 lifetime spend**. Accounts below that can use lists for observation and exclusion, which has been allowed since June 2021 — [Storegrowers](https://www.storegrowers.com/google-customer-match/); [Relevant Audience](https://www.relevantaudience.com/google-ads-en/google-ads-customer-match-guide/); [PPC Land](https://ppc.land/customer-match/).
  - These thresholds do not match the official page's two-requirement summary, so check them before relying on them.
  - List membership expires after 540 days. One guide says a list needs at least 100 members added or updated within 540 days to stay eligible — same sources.
- **EEA consent for Customer Match** — [Google Ads Help: EU user consent policy for Customer Match](https://support.google.com/google-ads/answer/14310715); [DV360 Help](https://support.google.com/displayvideo/answer/14673239?hl=en); [Google Ads Help: enforcement](https://support.google.com/google-ads/answer/14546648):
  - Since March 2024, EEA uploads must set both consent fields, `ad_user_data` and `ad_personalization`, to GRANTED.
  - A missing value is treated as no consent. A DENIED value returns an error.
  - Consent applies to a whole upload job, so users with different consent states need separate jobs.
  - Partners must pass consent through Google Ads API version 15 or later, or advertisers can set it manually in Audience Manager.
  - Data consented before March 2024 can still be used.
- **Consent Mode v2** is still mandatory for EEA and UK traffic on Google Ads, GA4 and DV360 — [SecurePrivacy](https://secureprivacy.ai/blog/google-killed-privacy-sandbox-what-changes-for-cookie-consent-in-2026).
- **Lookalike segments** — [Google Ads Help: Lookalike segments](https://support.google.com/google-ads/answer/13541369); [Google Ads API docs](https://developers.google.com/google-ads/api/docs/remarketing/audience-segments/lookalike-audiences); [Demand Gen audiences overview](https://support.google.com/google-ads/answer/15594567?hl=en-GB):
  - They are built from a seed list (Customer Match uploads, or people who interacted with your website, app or YouTube channel) and expand at Narrow, Balanced or Broad settings.
  - Google documents them as available only in Demand Gen campaigns.
  - Seeds need **at least 1,000 active matched people**. Create the segment 2–3 days before launch.
  - Google advises pairing a lookalike with a high-intent **custom segment built from your 10–15 best-converting search terms**.
  - A newer help article covers "Lookalike segments in Video campaigns", suggesting they now work beyond Demand Gen — [Google Ads Help](https://support.google.com/google-ads/answer/17219920).
  - One agency says that since March 2026 the seed list only guides targeting rather than limiting it. Unverified — [One PPC Agency](https://oneppcagency.co.uk/?p=39453).
- **Financial-services verification** — [PPC Land](https://ppc.land/google-expands-financial-ad-verification-to-24-eu-and-eea-countries/); [Search Engine Land](https://searchengineland.com/google-expands-financial-services-ad-verification-across-24-european-markets-480833); [Google Ads policy: Financial Services Verification](https://support.google.com/adspolicy/answer/12492484); [SEO-Day](https://www.seo-day.de/news/article/google-expands-financial-services-ad-verification-across-24?lang=en):
  - UK verification began on 6 September 2021.
  - In June 2026 Google extended the requirement to 24 EU and EEA countries, bringing the total to 42.
  - Enforcement is phased, with most new markets enforced from **23 July 2026**. Advertisers get **30 days** to verify before their ads are restricted.
  - In Germany, advertisers must prove they are licensed by the relevant regulator or exempt. Most first get a third-party check from the vendor G2.
  - Switzerland is not named in any source.
- **Bidding on competitor fund names: the UK precedent** — [LexisNexis](https://blogs.lexisnexis.co.uk/content/wipit/interflora-v-ms-adwords-are-ok-says-court-of-appeal); [Jones Day](https://jonesday.com/en/insights/2014/11/the-uk-court-of-appeal-orders-a-retrial-in-landmark-keyword-advertising-case); [Humphreys](https://www.humphreys.co.uk/articles/google-adwords-court-of-appeal-remits-interflora-keywords-advertising-trade-mark-case-for-retrial/):
  - In *Interflora v Marks & Spencer* [2014] EWCA Civ 1403, the Court of Appeal allowed M&S's appeal and ordered a retrial.
  - It held that buying a competitor's trade mark as a keyword is "not inherently objectionable".
  - It infringes only where the ad suggests a commercial connection with the mark's owner, or is too vague to rule one out.
- **Chrome and third-party cookies:**
  - Google abandoned its plan to remove third-party cookies in July 2024. In April 2025 it said Chrome would not add a replacement consent prompt.
  - Third-party cookies remain on by default in 2026, with no removal date — [Cookiebot](https://www.cookiebot.com/en/google-third-party-cookies/); [Usercentrics](https://usercentrics.com/knowledge-hub/what-is-google-privacy-sandbox/).
- **Privacy Sandbox retired:**
  - On 17 October 2025 Google retired most Privacy Sandbox advertising technologies, including **Protected Audience and Topics** on Chrome and Android, "in light of their low levels of adoption".
  - It keeps CHIPS and FedCM, maintains Private State Tokens, and is "moving away from the Privacy Sandbox branding" — [Privacy Sandbox blog](https://privacysandbox.google.com/blog/update-on-plans-for-privacy-sandbox-technologies); [BetaNews](https://betanews.com/2025/10/20/google-is-retiring-privacy-sandbox/); [CyberInsider](https://cyberinsider.com/google-quietly-dismantles-core-of-privacy-sandbox-for-chrome/).
  - One secondary guide cites Chrome release notes of 8 September 2026 that list Protected Audience, Attribution Reporting, Shared Storage and Related Website Sets for deprecation and removal — [Groas](https://www.groas.com/post/privacy-sandbox-third-party-cookies-status); [Groas guide](https://groas.com/post/google-privacy-sandbox-cookies-guide-2026).

### Inferences
- **Customer Match: mainly an exclusion tool at first.**
  - A newly verified boutique account is unlikely to meet the reported 90-day and $50,000 thresholds early on.
  - Where it is usable, EEA contacts need recorded consent for advertising use. That is a medium-to-high GDPR and ePrivacy risk for a B2B CRM that relies on legitimate interest.
  - Match rates on work email addresses are probably low (unverified).
  - The 1,000-person seed minimum makes Lookalikes impractical for fund-buyer lists.
- **Search is Google's best precision tool.** Build search campaigns and custom segments from fund-specific queries:
  - fund names, ISINs and share classes;
  - Investment Association or Morningstar sector names (for example "global equity income fund");
  - "UCITS", "SICAV" and "OEIC" combined with strategy names;
  - fund manager names.
- **Turning searches into an audience.** The search-term segments can then target YouTube video and Demand Gen ads at "people who research this kind of fund".
  - URL-based custom segments for fund-data, platform and research-house sites can also be tested. Exclude trade-media domains, to respect the brief.
  - Treat these audiences as probable fund researchers, not named buyers.
- **Verification as an operational step.** Allow at least 30 days to verify in each EU or EEA market before launch, and gather G2 or regulator evidence for Germany. Switzerland's position needs checking.
- **Competitor fund names.** Bidding on them is lawful in the UK in principle, provided the ad text does not imply a connection with the competitor. FCA rules on fair, clear and not misleading promotions and on comparisons still apply (see the compliance researcher).
- **Performance Max.** It mixes inventory with little transparency and expands audiences automatically, which works against named-account precision. Use Search and Video or Demand Gen with tight controls instead. This inference is not sourced this session.

### Gaps
- **Not researched (search budget ran out):**
  - evidence of Performance Max failing for niche B2B advertisers;
  - minimum sizes and serving thresholds for custom segments and YouTube audiences;
  - YouTube placement targeting;
  - Customer Match match rates for business email addresses;
  - Google Ads Data Manager;
  - Google's UK and EEA policy on trade-mark complaints;
  - CPCs for fund-name and adviser searches in the UK and EU.
- **UK and Swiss consent rules:** it is unverified whether Google's EU User Consent Policy and the Customer Match consent rules also cover the UK and Switzerland. *Unverified background:* the policy covers the EEA, UK and Switzerland; check.
- **EU case law.** *Unverified background:* the EU Court of Justice cases *Google France v Louis Vuitton* (2010) and *Interflora* (C-323/09, 2011) set the test the UK Court of Appeal applied, which asks whether the ad confuses buyers about who is behind it. The final outcome of the *Interflora* retrial was not established.

## 4. ABM platforms, intent data and IP-to-company targeting with UK and European strength

### Takeaway
Enterprise ABM (account-based marketing) suites typically cost five figures a year before any media spend. Median contracts are about $55,000–63,000 a year for 6sense and $29,000–65,000 for the Demandbase base platform, according to Vendr procurement data. Demandbase reportedly also requires $5,000–10,000 a month of display advertising.

The market has consolidated: RollWorks is now AdRoll ABM, and Terminus has been absorbed into DemandScience. European-native options are N.Rich (EU data storage, IAB consent framework) and Dealfront/Leadfeeder (from about €79 a month).

IP-to-company matching is weakest exactly where many fund buyers sit: small IFA practices working remotely or hybrid, where vendors report 5–10% match rates. For a list of 500–3,000 accounts dominated by small intermediaries, IP-based ABM advertising should be a secondary layer for larger institutions, not the main tool.

### Cited Findings
- **6sense** — [Landbase](https://www.landbase.com/blog/6sense-pricing); [Factors](https://www.factors.ai/blog/6sense-pricing-and-costs); [MarketBetter](https://marketbetter.ai/blog/6sense-pricing-2026/); [Salesmotion](https://salesmotion.io/blog/6sense-pricing) (mostly competitor blogs):
  - No public prices for paid plans. Tiers are Free, Team, Growth and Enterprise; whether the free tier is still offered is unclear.
  - Medians from Vendr data: about $62,800 a year (range about $11,500–175,000), or $55,200 (range $35,000–130,000+), or $63,200 across 383 purchases.
  - Contracts run 12–24 months, with credits, implementation and overage charges on top.
- **Demandbase** — [Docket](https://docket.io/resources/research/demandbase-pricing); [Landbase](https://www.landbase.com/blog/demandbase-pricing); [MarketBetter](https://marketbetter.ai/blog/demandbase-pricing-breakdown-2026/); [Abmatic](https://blog.abmatic.ai/demandbase-pricing-2026-breakdown):
  - No public prices. Vendr's 2025 median contract was $29,000; Docket estimates $45,000–65,000 a year for the base platform.
  - The full "Demandbase One" product starts at $200,000 a year; an AWS Marketplace 12-month listing shows $215,000.
  - Onboarding costs about $29,000, and each extra user seat $1,200–3,000 a year.
  - **Display advertising minimums are reportedly about $5,000–10,000 a month.**
- **RollWorks, now AdRoll ABM** — [AdRoll](https://www.adroll.com/blog/introducing-adrollabm); [Metadata](https://metadata.io/compare/rollworks-alternatives); [RevenueFlow](https://www.revenueflow.com/blog/rollworks); [PPC Land](https://ppc.land/adroll-unifies-brand-with-ai-assistant-launch-eliminating-rollworks-complexity/):
  - Rebranded within its parent company, NextRoll, around August 2025. rollworks.com now redirects to adroll.com.
  - AdRoll says there are "no changes to your pricing or packaging". Its pricing page shows no figures, only a demo request.
  - Vibhor Kapoor became NextRoll's CEO in February 2026.
- **Terminus, now part of DemandScience** — [Abmatic](https://abmatic.ai/blog/what-happened-to-terminus-abm-2026); [Derrick](https://derrick-app.com/tools/terminus-pricing); [Hey Sid](https://www.heysid.com/resources/best-terminus-alternatives-for-abm); [RevenueFlow](https://www.revenueflow.com/blog/account-based-marketing-platforms):
  - Folded into DemandScience; most sources date the merger to 12 November 2024. One outlier dates it to 2023 — [Influ2](https://www.influ2.com/blog/abm-platforms).
  - The Terminus brand is retired, and terminus.com redirects to demandscience.com.
  - Its features now sit in "ABX by DemandScience", with the advertising product listed as Media Placement & Management. Pricing is by quote only.
- **N.Rich (Finland; focused on Europe)** — [N.Rich](https://nrich.io/abm-platform-for-europe-and-emea); [N.Rich comparisons](https://nrich.io/alternative); [N.Rich vs RollWorks](https://nrich.io/alternative/rollworks); [OMR](https://omr.com/en/reviews/product/n-rich/pricing); [Bitscale](https://bitscale.ai/directory/nrich):
  - Data roles: processor for clients' website and marketing-automation data, and controller for its programmatic advertising data. It collects consent through the IAB Transparency and Consent Framework (TCF), the industry-standard cookie-consent system.
  - European personal data is stored on dedicated servers in France and Germany.
  - It claims intent data in up to 12 European languages, though another of its own pages says 4.
  - It claims to be the only European vendor in Gartner's ABM Magic Quadrant (2023 on one page, 2024 on another).
  - Pricing on request. One third-party price listing appears to be wrong.
- **Jabmo** — [TrustRadius](https://www.trustradius.com/compare-products/jabmo); [G2](https://www.g2.com/products/jabmo/pricing); [Abmatic](https://blog.abmatic.ai/jabmo-alternatives-2026):
  - Detects activity from anonymous visiting companies and runs IP-based advertising, retargeting, website personalisation, analytics and sales enablement.
  - No published pricing and no free trial. A competitor estimates $40,000–150,000, rising above $100,000 a year once lists exceed 500–1,000 accounts.
  - The same competitor says it has no built-in intent data.
- **Dealfront (Leadfeeder plus Echobot)** — [Abmatic](https://blog.abmatic.ai/leadfeeder-pricing); [ZoomInfo](https://pipeline.zoominfo.com/sales/dealfront-pricing); [MarketBetter](https://marketbetter.ai/blog/dealfront-pricing-breakdown-2026/); [Artisan](https://www.artisan.co/blog/leadfeeder-vs-snitcher-which-should-you-choose-in-2026):
  - Leadfeeder's paid plans run from about €79 a month (1,000 companies and 50 credits) to €599 a month on the Scale plan. A free Lite plan covers 100 companies over 7 days. Other sources quote €99 or $99 a month.
  - The full suite (Target, Connect and Datacare) is quote-only, estimated at about $15,000–36,000 a year, or $1,500–3,750 a month.
  - It identifies visiting companies, not people, which comparison sites describe as the GDPR-friendly approach.
  - A competitor describes its data as built on European company registers, with hosting only in the EU.
- **Madison Logic** — [Madison Logic](https://www.madisonlogic.com/); [ML Insights](https://www.madisonlogic.com/solutions/ml-insights/); [ML press release](https://www.madisonlogic.com/press-release/ml-intent-dashboard/); [Demand Gen Report](https://www.demandgenreport.com/industry-news/news-brief/madison-logic-unveils-new-account-buying-group-intelligence-capabilities/50916/); [Abmatic](https://abmatic.ai/blog/madison-logic-strengths-and-weaknesses-2026); [GlobeNewswire, 2014](https://www.globenewswire.com/news-release/2014/02/13/1227920/0/en/Madison-Logic-Offers-Marketers-Better-Targeting-in-Europe-by-Signing-Intent-Data-Partnership-Deal-in-France.html):
  - Runs LinkedIn ads prioritised by intent, "creating custom matched audiences with market-leading intent data".
  - Customers with a live media campaign get its buyer-intent data (ML Insights) at no extra charge.
  - Its Intent Dashboard (launched 5 November 2025) sorts insights by region, industry and company size. It also offers account and buying-group intelligence.
  - Its intent data mainly comes from activity across its own content network.
  - Its network of European partners dates back to 2014.
- **Bombora (intent data)** — [Bitscale](https://bitscale.ai/blogs/bombora-review); [Subger](https://subger.com/en/service/bombora); [APIs.io](https://apis.io/providers/bombora/); [Derrick](https://derrick-app.com/fr/tools/bombora); [Truto](https://truto.one/blog/connect-bombora-to-chatgpt-track-b2b-intent-manage-account-lists/):
  - Its topic list includes a financial-services category, but sources disagree on its size: 4,000+, 13,000+ or 18,000+ topics.
  - Requests for niche topics need confirmation of process and timing. A topic-listing API can search by name, theme or category.
  - **No source confirmed fund-specific topics** such as ETFs, mutual funds, ESG investing or dividend investing.
- **How accurate IP-to-company matching is with hybrid work (vendor estimates, mostly US):**
  - Overall company-level match rates are about 30–65% of B2B website traffic ([Unify](https://www.unifygtm.com/explore/website-visitor-identification-how-it-works); [Coffee](https://coffee.ai/articles/b2b-visitor-identification-tools-2026)), or 30–40% ([Markettailor](https://markettailor.io/blog/visitor-identification-company-tracking)).
  - People working from home on domestic broadband show up as their internet provider, not their employer ([LeadBoxer](https://www.leadboxer.com/learn/ip-to-company-lookup-identify-website-visitors)).
  - Expected match rates by segment: **50–65% for enterprise offices, 30–45% for small-business offices, 10–20% for remote enterprise staff and 5–10% for remote small-business staff** ([MarketBetter](https://marketbetter.ai/blog/best-website-visitor-identification-tools-2026/)).
  - Matching more aggressively reduces precision ([HappierLeads](https://happierleads.com/blog/reverse-ip-lookup-accuracy-benchmark-2026)), and "confidently wrong matches can be worse than no match" ([Abmatic](https://abmatic.ai/blog/reverse-ip-lookup-dying-agent-era-2026)).
  - Identifying individual people works for only about 5–20% of US traffic and needs identity-matching databases ([Coffee](https://coffee.ai/articles/b2b-visitor-identification-tools-2026)).

### Inferences
- **Do enterprise suites suit 500–3,000 accounts at boutique scale?**
  - Using the cited estimates, a Demandbase-style programme could cost **about $118,000–214,000 in the first year**: a $29,000–65,000 licence, $60,000–120,000 of display minimums and about $29,000 of onboarding.
  - 6sense medians of about $55,000–63,000 come before any media spend.
  - Both look disproportionate for a boutique unless the list is concentrated in large institutions (banks, private banks, insurers, platforms and large DFMs). There, IP matching works better and multi-person buying groups justify the cost.
- **A better-fit European stack:**
  - LinkedIn's built-in ABM features (company lists, Companies tab, Buyer Groups) as the core.
  - Dealfront or Leadfeeder for identifying visiting companies and alerting sales, at roughly €1,000–7,000 a year for Leadfeeder plans.
  - Optionally, N.Rich for account-based display advertising, using its EU data storage and TCF consent.
- **IFA practices.** With only 5–10% of remote small-business traffic matched, IP-based targeting and identification will miss most IFA firms. It is also more likely to attribute visits wrongly, for example from shared offices or networks. Reach them through member attributes on LinkedIn and search intent instead.
- **Large institutions.** Corporate VPN traffic may appear to come from one central location; a Swiss private bank's traffic might all exit in Zurich, for example. That helps identify the account but can distort country-level targeting. This inference is not sourced.
- **Intent data for fund selection is probably thin.** Fund research happens largely inside closed tools and platforms, which are unlikely to feed intent data co-operatives (inference).
  - Check Bombora's topic coverage through its topic API before buying.
  - Weight your own first-party signals, such as factsheet downloads and webinar attendance, above third-party intent.
- **GDPR flags:**
  - **Low to medium:** identifying larger firms at company level.
  - **Medium:** identifying sole-trader or very small IFA firms, where the company effectively identifies a person.
  - **High in the UK and EU:** identifying individual people, or person-based ads. Another researcher covers the legal detail.

### Gaps
- **Not researched (search budget ran out):**
  - Influ2 (person-based B2B ads);
  - Lead Forensics (UK) and Albacross (Sweden);
  - Metadata.io;
  - account-level CTV offerings from 6sense, Demandbase, Madison Logic and others;
  - 6sense's and Demandbase's claims about European data coverage and quality;
  - Bombora's coverage in Europe, the Middle East and Africa;
  - ABM case studies from asset managers or wealth firms.
- **Pricing evidence:** all of it comes from third-party blogs, mostly written by competitors. No vendor quotes were obtained.
- **IP accuracy:** no independent European measurement was found. All figures are vendors' own and US-focused.

## 5. Programmatic B2B audience data, curation and cookieless identity in Europe

### Takeaway
This area was only partly researched. Three structural changes are confirmed:
- **Microsoft has left the DSP business.** Invest shut on 28 February 2026, with Amazon DSP as the preferred route for moving campaigns. Curate and Monetize remain.
- **LinkedIn's professional data now reaches CTV programmatically.** This runs through The Trade Desk (using Microsoft Monetize supply) and Amazon DSP, and through DV360 in the US only.
- **Consent, not browser policy, is the binding constraint.** Chrome third-party cookies remain, but Privacy Sandbox's advertising tools are retired. EU and UK consent requirements (the IAB consent framework and Google's Consent Mode v2) are what limit targeting.

B2B data marketplaces, adoption of EUID and ID5 (cookieless identifiers) and curation platforms could not be checked this session.

### Cited Findings
- **Microsoft Invest:** shut on 28 February 2026. Microsoft kept the Microsoft Advertising Platform, Monetize and Curate, and named Amazon DSP as its preferred transition partner — [MediaPost](https://www.mediapost.com/publications/article/409701/microsoft-leans-on-amazon-for-its-demand-side-plat.html); [Search Engine Land](https://searchengineland.com/microsoft-amazon-dsp-preferred-partner-463066); [Xenoss](https://xenoss.io/blog/microsoft-sunsets-invest-dsp-signals-a-new-era-of-walled-garden-ai-advertising).
- **LinkedIn CTV programmatic routes:**
  - The Trade Desk, using Microsoft Monetize — [Social Samosa](https://www.socialsamosa.com/news-2/linkedin-expands-brandlink-programme-ctv-advertising-11248078); [The Keyword](https://www.thekeyword.co/news/linkedin-ctv-trade-desk-b2b-advertising).
  - Amazon DSP, since May 2026 — [Marketing Dive](https://www.marketingdive.com/news/amazon-linkedin-help-advertisers-reach-professionals-via-ctv-ads/819372/).
  - Google DV360 CTV, in the US only — [PPC Land headline](https://ppc.land/linkedin-job-title-targeting-reaches-google-dv360-ctv-buys-in-the-us/).
- **Cookies:** Chrome third-party cookies stay on by default with no removal date, and the Privacy Sandbox advertising tools were retired in October 2025 — [Cookiebot](https://www.cookiebot.com/en/google-third-party-cookies/); [Privacy Sandbox blog](https://privacysandbox.google.com/blog/update-on-plans-for-privacy-sandbox-technologies).
- **Consent:** Consent Mode v2 is still mandatory for EEA and UK traffic on Google Ads, GA4 and DV360 — [SecurePrivacy](https://secureprivacy.ai/blog/google-killed-privacy-sandbox-what-changes-for-cookie-consent-in-2026).
- **A European-native option:** N.Rich runs programmatic ads as data controller, collects consent through the IAB TCF and stores EU data in France and Germany — [N.Rich](https://nrich.io/abm-platform-for-europe-and-emea).

### Inferences
- **Cookie-based B2B segments still work where Chrome users have consented.** This covers firmographic and intent segments derived from IP addresses or cookies, such as the Dun & Bradstreet, Bombora or Madison Logic data named in the brief (not verified this session). Safari and Firefox users, and EU or UK users who decline consent, fall outside them. This matters most for audiences who read on mobile.
- **At boutique budgets, programmatic is a supporting layer.** The likely routes are an agency's seat on a major DSP, or a B2B-specialist or European-native platform such as N.Rich. Prefer curated or private deals with business and financial publishers that are *not* investment trade media, to respect the brief.
- **Account-level CTV for fund buyers is still experimental in Europe.** Reports conflict on whether LinkedIn CTV is available in the UK, and programmatic CTV reach depends on access to The Trade Desk or Amazon DSP.

### Gaps
- **Not researched this session (search budget ran out).** *Unverified background (training knowledge, pre-June 2026):*
  - **The Trade Desk data marketplace:** carries third-party B2B segments from Dun & Bradstreet (which bought Eyeota in 2021), Bombora, LiveRamp and Experian. These B2B segments are less available in Europe than in the US.
  - **Cookieless identifiers:** UID2 has a European counterpart, EUID, designed around GDPR consent. ID5 is a widely used European identifier. How widely either is adopted in 2026 is unknown.
  - **Curated deals:** offered by Index Exchange Marketplaces, Magnite, PubMatic, Microsoft Curate, Equativ and Permutive. Their fit for B2B finance audiences is unverified.
  - **DSPs used in Europe:** DV360, Amazon DSP, Adform and StackAdapt, the last popular with B2B advertisers because of its B2B data partners. Minimum spends are unverified.
  - **Apple:** App Tracking Transparency (iOS 14.5, 2021) restricts tracking in apps. Safari's Intelligent Tracking Prevention and Link Tracking Protection limit cookies and click IDs. The effect on desktop B2B targeting is probably modest, but no 2026 evidence was gathered.
- **Costs:** no European CPMs for programmatic campaigns using B2B data were found.

## 6. CRM activation and clean rooms: matching asset-manager CRM data to platforms, sales-triggered sequences, visitor identification and document-engagement signals

### Takeaway
In 2026 a UCITS manager can connect its CRM to advertising through four main routes:
- **LinkedIn:** CRM lists synced through connectors. Middleware can sync every 15 minutes, but LinkedIn takes up to 24 hours to process a list, and an audience needs 300 matched members before it serves.
- **Google:** Customer Match, which needs explicit EEA consent signals with every upload and may be restricted by spend thresholds.
- **Website:** company-level visitor identification (Dealfront/Leadfeeder) feeding sales alerts and company lists.
- **Microsoft:** LinkedIn company targeting, with nothing uploaded.

Clean rooms and the linking of document-engagement data (for example DocSend) to ad audiences could not be checked this session.

### Cited Findings
- **LinkedIn timing and thresholds:** processing takes up to 24 hours ([Gartner FAQ](https://support.ops.gartner.com/support/solutions/articles/70000640455-linkedin-faqs)), and an audience needs 300 matched members to serve ([LinkedIn](https://business.linkedin.com/advertise/ads/audience)).
- **LinkedIn connectors:**
  - LeadsBridge builds audiences from Salesforce leads, campaign members and report or list views — [LeadsBridge](https://leadsbridge.com/integrations/salesforce/linkedin-matched-audiences).
  - A Make.com template syncs HubSpot every 15 minutes — [Make](https://make.com/en/integrations/linkedin-matched-audiences).
- **Madison Logic** builds custom LinkedIn audiences from its intent data — [Madison Logic](https://www.madisonlogic.com/).
- **Google Customer Match in the EEA** — [Google Ads Help](https://support.google.com/google-ads/answer/14310715); [DV360 Help](https://support.google.com/displayvideo/answer/14673239?hl=en):
  - Both consent fields must be set to GRANTED, and consent applies per upload job.
  - Partner uploads need API version 15 or later; alternatively, consent can be set manually in Audience Manager.
  - If someone withdraws consent, remove them from the audience or replace the file.
- **Company-level visitor identification:**
  - Dealfront and Leadfeeder identify visiting companies rather than people, with hosting in the EU — [ZoomInfo comparison](https://pipeline.zoominfo.com/sales/dealfront-pricing); [Artisan](https://www.artisan.co/blog/leadfeeder-vs-snitcher-which-should-you-choose-in-2026).
  - N.Rich processes clients' website and marketing-automation data as a processor — [N.Rich](https://nrich.io/abm-platform-for-europe-and-emea).
- **LinkedIn Companies tab:** shows engagement by account for uploaded lists, combining ads, organic posts and website visits — [ZenABM](https://zenabm.com/blog/see-companies-engaging-with-linkedin-ads).
- **Speed of sales follow-up:** in GK3's asset-manager example, leads from lead forms arrived "in real time" and sales "followed up quickly" — [GK3](https://www.gk3capital.com/insights/how-a-premier-asset-manager-raised-nearly-40m-with-linkedin-advertising).

### Inferences
- **Sales-triggered ad sequences work as pooled, rolling audiences, not per-person triggers.**
  - Build CRM-driven lists such as:
    - contacts with a meeting booked in the next 14 days;
    - factsheet downloaders in the last 30 days;
    - webinar registrants and attendees;
    - new contacts added to open opportunities.
  - Sync them to LinkedIn, and to Google only where EEA consent exists.
  - Pool them across teams and countries until each passes 300 matched members.
  - Then run a short sequence: portfolio manager Thought Leader posts, then the relevant Document Ad, then a UK-only Conversation Ad invitation.
  - Because LinkedIn can take up to 24 hours to process a list, add contacts at least 2–3 days before the meeting.
- **A lower-risk alternative: trigger at firm level.** When a CRM account reaches a set stage, add the firm to a "hot accounts" company list combined with the relevant job functions.
  - This needs no personal-data upload, because company names are not personal data.
  - It works only for firms large enough to reach 300 members on their own, or when several firms are pooled.
- **Visitor identification:**
  - Company-level tools (Dealfront/Leadfeeder) can feed a weekly "visited our fund pages" company list back into LinkedIn and into sales alerts.
  - Avoid tools that try to identify individual visitors. They are US-focused, identify only 5–20% of people, and are high-risk for UK and EU traffic.
- **GDPR and PECR flags:**
  - **Medium:** uploading contacts to LinkedIn.
  - **Medium to high:** EEA Customer Match, which needs consent signals.
  - **Medium:** website retargeting tags, which need cookie consent.
  - **Low:** company lists.

### Gaps
- **Not researched (search budget ran out):**
  - LinkedIn's own CRM integrations (Salesforce, Dynamics 365 Customer Insights, HubSpot) and the LinkedIn Conversions API;
  - Google Ads Data Manager connectors;
  - LiveRamp (its RampID identifier and clean rooms) and InfoSum. *Unverified background:* WPP acquired InfoSum in 2025;
  - any LinkedIn clean-room offering;
  - engagement data from DocSend, Seismic LiveDocs, Showpad and Highspot feeding the CRM and ad audiences;
  - "reverse ETL" tools (Hightouch, Census) that push warehouse data into ad audiences.
- **Results:** no asset-manager example of CRM-triggered advertising with results was found.

## 7. Advanced orchestration: sequential and surround ABM, 1:few personalisation, buying-committee mapping, meeting-based and job-change triggers

### Takeaway
The verified building blocks for orchestrated, multi-channel account-based programmes in late 2026 are:
- **LinkedIn:** company-list clusters; Buyer Group templates (February 2026); Thought Leader Ads from portfolio managers and third parties (with the author's approval); the Companies tab for account engagement; and Conversation Ads in the UK only.
- **Microsoft:** LinkedIn company targeting on search and native ads in the UK, France and Germany.
- **Google:** capturing search intent.
- **Website:** company-level visitor identification.

Dreamdata measured an average B2B buyer journey of 211 days, which favours always-on sequences over short bursts. Personalisation and video vendors (Mutiny, Folloze, Uberflip, Hushly, Vidyard, Sendspark), job-change tools and documented asset-manager results could not be checked this session.

### Cited Findings
- **LinkedIn Buyer Group targeting:** predefined clusters of the people at one company likely to be involved in a purchase, with templates built for typical buying situations. Reported launch 5 February 2026 — [Optimize LinkedIn Ads](https://www.optimizelinkedinads.com/blogs/linkedin-buyer-group-targeting-ads-guide); [ABM Agency](https://abmagency.com/linkedin-abm-news-today-updated-ad-targeting-options-for-account-based-campaigns-recency-update/amp/).
- **Madison Logic** offers "account and buying group intelligence" — [Demand Gen Report](https://www.demandgenreport.com/industry-news/news-brief/madison-logic-unveils-new-account-buying-group-intelligence-capabilities/50916/).
- **Thought Leader Ads discovery and event versions** let brands sponsor posts that mention the brand or an event, including posts by non-employees — [Social Media Today](https://www.socialmediatoday.com/news/linkedin-thought-leader-ads-discovery-campaign-manager/804325/); [HeyOrca](https://www.heyorca.com/blog/linkedin-social-news).
- **Buyer journeys** averaged 211 days, and LinkedIn had the highest measured return on ad spend among the major networks — [PPC Land on Dreamdata 2025](https://ppc.land/linkedin-emerges-as-top-b2b-platform-with-113-roas-and-211-day-buyer-journeys/).
- **LinkedIn Companies tab** scores engagement by account across ads, organic posts and website visits — [ZenABM](https://zenabm.com/blog/see-companies-engaging-with-linkedin-ads).
- **Practitioner advice:** target several roles in each account, and add job function and seniority filters to account lists — [Vizion](https://www.vizion.com/blog/linkedin-abm-targeting-guide-2026-what-works-what-doesnt-how-to-reach-b2b-buying-committees/).

### Inferences
- **A three-tier plan for a boutique, UK-headquartered UCITS manager.** This combines the capabilities cited above, with costs as in sections 1–4.
  - **Tier 1: about 50–150 strategic institutions** (UK DFMs and platforms, private banks, Swiss external-asset-manager platforms, insurers' unit-linked desks, fund-of-funds teams):
    - LinkedIn company-list ad sets by institution type and country, with Buyer Group or manual function and seniority filters.
    - Portfolio manager Thought Leader Ads as the opener.
    - Document Ads plus Lead Gen Forms for strategy papers.
    - UK Conversation Ads inviting buyers to meet the fund manager.
    - Microsoft LinkedIn company targeting on search and native ads in the UK, France and Germany.
    - Optional account-level display through N.Rich or Dealfront.
    - Companies-tab scores reviewed weekly with sales.
  - **Tier 2: about 1,000–3,000 UK IFA and paraplanner firms, plus continental adviser networks:**
    - Target by member attributes (title, function, industry, location and language) rather than IP address.
    - Google and Microsoft search on fund names, ISINs and sectors.
    - Website retargeting where visitors have consented.
    - Pooled CRM-triggered lists of at least 300 matched members.
  - **Tier 3: influencers** (fund research and ratings houses):
    - Small company-list clusters for portfolio manager Thought Leader content. Expect delivery limits, because these firms may have fewer than 300 members.
- **Ads to the people in next week's meeting.** This works only through a pooled list of everyone with an upcoming meeting (see section 6), or at firm level for large institutions. Targeting one meeting's attendees individually needs person-based ad vendors, which are high-risk in the UK and EU and were not checked this session.
- **Job-change triggers** (for example a new head of fund research):
  - Add the new person's firm and job function to a "new decision-maker" cluster, and prompt sales to make contact.
  - Using LinkedIn's own targeting rather than uploading personal data keeps the risk low to medium.
- **Personalise per cluster, not per account.** Build one landing page or microsite for each cluster and language (for example "Swiss external asset managers", "French CGPs", "UK model portfolio services"), not one per account. That keeps financial-promotion approvals manageable. This follows the brief's compliance logic rather than a sourced finding.
- **UK vs EU and Switzerland differences** (drawn from the findings above):

| Feature | UK | EU/EEA | Switzerland |
|---|---|---|---|
| LinkedIn Sponsored Messaging | Not covered by the opt-in rule (inferred; verify) | Opted-in members only ([LinkedIn Help](https://www.linkedin.com/help/lms/answer/a427509)) | Opted-in members only ([LinkedIn Help](https://www.linkedin.com/help/lms/answer/a427509)) |
| LinkedIn Group targeting | Unverified | Off since June 2024 under the DSA ([PPC Land](https://ppc.land/linkedin-discontinues-group-based-ad-targeting-to-comply-with-dsa/)) | Unverified |
| LinkedIn sharing ad data with Microsoft (from 3 November 2025) | Not applied ([Gulf News](https://gulfnews.com/technology/linkedin-privacy-update-microsoft-can-use-your-data-from-nov-3-how-to-stop-it-1.500281615)) | Not applied | Not applied |
| Microsoft LinkedIn profile targeting | Yes ([Microsoft](https://Advertising.Microsoft.com/en-us/solutions/Audience-targeting/LinkedIn-Profile-Targeting)) | France and Germany only | No |
| Microsoft job-seniority targeting (June 2026) | No ([PPC Land](https://ppc.land/microsoft-advertising-adds-job-seniority-to-linkedin-profile-targeting/)) | Not in France or Germany | No |
| Google financial-services verification | Since September 2021 | Most markets from 23 July 2026 ([Search Engine Land](https://searchengineland.com/google-expands-financial-services-ad-verification-across-24-european-markets-480833)) | Not named |
| Google Customer Match consent signals | Unverified | Required since March 2024 ([Google](https://support.google.com/google-ads/answer/14310715)) | Unverified |
| LinkedIn CTV | Conflicting reports (2026 according to [Kiin](https://kiin.co/research/linkedin-ctv-ads-benchmarks)) | Unverified | Unverified |

### Gaps
- **Not researched (search budget ran out):**
  - personalised landing pages and microsites: Mutiny, Folloze, Uberflip and Hushly (current product status and pricing);
  - personalised video: Vidyard and Sendspark;
  - job-change alerts: UserGems, Champify and LinkedIn Sales Navigator alerts;
  - person-based ads: Influ2;
  - documented results from asset managers or similar financial-services marketers.
- **Uplift:** no source measured the uplift from sequential or multi-channel "surround" programmes aimed at fund buyers.
