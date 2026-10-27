# Cross-industry and unconventional digital tactics for reaching professional fund buyers (UK and Europe, as of late October 2026)

*Verification status (read first): in this session the shared WebSearch budget was already used up, and the egress proxy refused every outbound web host with HTTP 403, including Wikipedia, Veeva, PMCPA, FCA, Allfunds, ESMA and Reachdesk (checked 27 Oct 2026). WebFetch also failed on DNS. No page could be opened. Every finding below comes from the researcher's existing knowledge (to mid-2026). Each one cites the canonical public location of its source, but no source was re-opened today. Confidence tags: **[H]** = well-established fact, high confidence; **[M]** = believed correct but should be checked before publication. Anything weaker is in the Gaps sections. Where only a homepage is cited, the deep link could not be confirmed. Numbers marked "estimate" are the researcher's own judgement, not sourced data. Excluded on the user's instruction: advertising, sponsored content, events, awards and data products owned by investment, fund or adviser trade media.*

## 1. Pharma/medical HCP marketing: what works, what it achieves, and what has a direct fund-buyer equivalent

### Takeaway
Pharma's most transferable assets are its infrastructure, not its ad formats. They are verified professional identity (NPI in the US, DocCheck-style logins in Europe), pre-approved modular content that lets reps send compliant personalised follow-ups (Veeva Approved Email), closed-loop feedback, education kept separate from promotion (CME), and a distinct "market access" discipline that makes formulary decisions easy. In the UK and EU, point-of-care advertising is much more restricted than in the US, and fund-selection tools look similar. The realistic fund equivalent is presence and data quality inside fund buyers' workflow platforms (Allfunds Connect/Telemetrics, Dynamic Planner risk profiles, FinDatEx templates, CPD libraries) rather than banner ads inside tools.

### Cited Findings

#### Source industry: identity, registries and HCP-verified media
- [H] Every US healthcare provider who bills has a unique 10-digit National Provider Identifier (NPI), searchable in the public NPPES registry. US HCP ad-tech builds "NPI-level" audiences by matching NPIs to logins and devices. This is the US-specific infrastructure that makes HCP programmatic possible. — [CMS NPPES NPI Registry](https://npiregistry.cms.hhs.gov/)
- [M] DeepIntent (founded 2016) is a healthcare-only demand-side platform offering NPI-level HCP planning and targeting, with campaign outcomes measured against prescription and claims data. — [DeepIntent](https://www.deepintent.com/)
- [M] PulsePoint (acquired by WebMD/Internet Brands, 2021) sells "HCP365", NPI-level targeting of HCPs across programmatic inventory. It now sits within WebMD's healthcare marketing business. — [PulsePoint](https://www.pulsepoint.com/)
- [M] Doceree (founded 2019) runs an HCP-only programmatic network that serves messages inside physician platforms (e-prescribing, EHR/practice software, telehealth and medical sites) to verified HCPs, including "point-of-care" formats. — [Doceree](https://doceree.com/)
- [M] OptimizeRx (Nasdaq: OPRX) places brand, savings and patient-support messages inside EHR and e-prescribing workflows. Its Dynamic Audience Activation Platform (DAAP) uses real-world-data triggers to message an HCP when a patient matching clinical criteria appears. It acquired Medicx Health in 2023 to add consumer reach. — [OptimizeRx](https://www.optimizerx.com/)
- [M] Doximity, a US professional network for physicians, reports that over 80% of US physicians are members. Most of its revenue comes from pharma marketing and hiring solutions. It is the clearest example of a profession-specific network monetised by advertisers. — [Doximity investor relations](https://investors.doximity.com/)
- [H] Medscape (WebMD) combines clinical news, accredited CME, case challenges and quizzes for HCPs. It is the archetypal HCP portal funded by pharma advertising and education grants. — [Medscape](https://www.medscape.com/)
- [H] Germany's Heilmittelwerbegesetz (HWG) restricts advertising of prescription medicines to "Fachkreise" (healthcare professionals). Pharma websites therefore put professional content behind verified logins, and DocCheck Login is the de facto HCP authentication layer in German-speaking markets. — [HWG (gesetze-im-internet.de)](https://www.gesetze-im-internet.de/heilmwerbg/); [DocCheck](https://www.doccheck.com/)
- [M] Doctors.net.uk (owned by Japan's M3 group) is a UK doctor-only network funded largely by pharma communications. — [Doctors.net.uk](https://www.doctors.net.uk/)
- [M] In the UK, prescribing decision-support software in GP systems (e.g., FDB's OptimiseRx, which is unrelated to the US OptimizeRx, and Optum's ScriptSwitch) is deployed by NHS commissioners to steer cost-effective prescribing. UK point-of-care messaging is therefore largely payer-controlled rather than bought by pharma. — [FDB UK](https://www.fdbhealth.co.uk/)

#### Source industry: rep-triggered email, omnichannel orchestration and closed loop
- [H] Veeva CRM "Approved Email": reps can send only emails assembled from templates and content fragments pre-approved through medical-legal-regulatory (MLR) review. Sends and opens are logged against the HCP record, and HCP consent is captured in CRM. Veeva "CLM" (closed-loop marketing) records which detail-aid slides an HCP viewed and for how long, so field reactions feed back to brand teams. Veeva has been moving customers from its Salesforce-based CRM to its own Vault CRM platform since 2025. — [Veeva Systems](https://www.veeva.com/)
- [M] Veeva Vault PromoMats manages promotional content and MLR review. Industry practice has shifted to "modular content": pre-approved claims and modules recombined into many personalised assets without re-reviewing every permutation. — [Veeva Vault PromoMats](https://www.veeva.com/products/vault-promomats/)
- [M] Veeva Link (Key People) maps KOLs and digital opinion leaders from publications, congress activity and social media. Veeva Crossix (acquired 2019) measures campaign impact using privacy-safe health data. — [Veeva Systems](https://www.veeva.com/)
- [M] Competing orchestration stacks include IQVIA OCE (Orchestrated Customer Engagement) and Salesforce Life Sciences Cloud (launched 2024–25). Aktana supplies AI "next-best-action" suggestions to pharma field teams, telling a rep which HCP to contact, through which channel and with what content. — [IQVIA](https://www.iqvia.com/); [Salesforce](https://www.salesforce.com/); [Aktana](https://www.aktana.com/)
- [M] ZS's AccessMonitor has tracked a long-term decline in US physicians' accessibility to sales reps. That decline is the structural reason pharma moved budget into digital, rep-triggered and remote channels. — [ZS Associates](https://www.zs.com/)
- [H] Medical science liaisons (MSLs) sit in medical affairs, not sales. They conduct non-promotional scientific exchange with KOLs, which is legally and organisationally separate from promotion. — [Medical Science Liaison Society](https://www.themsls.org/)
- [M] US "market access" teams use the AMCP Format for Formulary Submissions, a standardised evidence dossier that makes payer and formulary reviews quicker. Winning formulary listing is treated as a discipline separate from promotion to prescribers. — [AMCP](https://www.amcp.org/)

#### Source industry: codes, CME and KOL rules
- [H] UK: the ABPI Code of Practice (current 2024 Code, in force from 1 July 2024) is administered by the PMCPA. Prescription-only medicines may be promoted only to HCPs and other relevant decision makers. Promotional material must be formally certified before use. Transfers of value to HCPs are disclosed publicly via Disclosure UK. The PMCPA publishes guidance on digital and social media activity. — [PMCPA](https://www.pmcpa.org.uk/); [ABPI](https://www.abpi.org.uk/)
- [M] Under the ABPI Code, certification requires two signatories, one of whom must be a UK-registered medical practitioner or pharmacist (or, for some material, another appropriately qualified person). — [PMCPA](https://www.pmcpa.org.uk/)
- [H] The EFPIA Code of Practice binds EU national industry associations. It covers interactions with HCPs and healthcare organisations, including annual public disclosure of transfers of value (since 2016). — [EFPIA Code](https://www.efpia.eu/relationships-code/the-efpia-code/)
- [H] The US ACCME "Standards for Integrity and Independence in Accredited Continuing Education" (December 2020) bar ineligible companies (pharma and devices) from controlling accredited education content. Any commercial support must come through written grant agreements, and promotion must be kept apart from accredited education. — [ACCME](https://accme.org/)
- [M] In Europe, the UEMS's EACCME accredits live and e-learning CME under comparable independence rules. — [UEMS](https://www.uems.eu/)

#### Fund-industry equivalents (registries, workflow platforms, CPD, inducement rules)
- [H] UK registry: the FCA Financial Services Register is a public register of authorised firms, each with a Firm Reference Number (FRN), and of individuals. These are senior managers and, via the FCA Directory under SM&CR, certified client-facing staff such as investment advisers. It is the nearest UK equivalent of the NPI registry, but it has no ad-tech identity graph attached. — [FCA Register](https://register.fca.org.uk/)
- [H] Continental registries usable for account-list building: France's ORIAS (registers CIFs/CGPs and other intermediaries); Italy's OCF (Albo unico dei consulenti finanziari); Spain's CNMV (investment firms including EAFs); Germany's DIHK Vermittlerregister (§34f financial-investment intermediaries and §34h fee-based advisers). — [ORIAS](https://www.orias.fr/); [OCF](https://www.organismocf.it/); [CNMV](https://www.cnmv.es/); [Vermittlerregister](https://www.vermittlerregister.info/)
- [H] Switzerland: under FinIA (in force 2020, transition to end-2022), independent asset managers need FINMA authorisation and are supervised by approved supervisory organisations. FINMA publishes lists of authorised institutions. FinSA requires client advisers of non-prudentially-supervised firms to be entered in an advisers' register. — [FINMA](https://www.finma.ch/)
- [H] US equivalent for comparison: FINRA BrokerCheck and SEC IAPD are public adviser registries. [M] US asset managers routinely license adviser databases derived from these filings and match them to digital audiences; Europe has no comparable mature market. — [FINRA BrokerCheck](https://brokercheck.finra.org/); [SEC IAPD](https://adviserinfo.sec.gov/)
- [H] Allfunds (Madrid; listed on Euronext Amsterdam since 2021) is Europe's largest B2B fund distribution platform, used by bank, private-bank and wealth-manager fund selectors. Allfunds Connect is its digital research and selection environment for fund selectors. — [Allfunds](https://allfunds.com/)
- [M] Allfunds sells fund houses "Telemetrics", analytics on how distributors' fund selectors interact with a house's funds on Allfunds Connect (views, searches, downloads), alongside digital marketing and data services. This is the closest European analogue to pharma's point-of-care and closed-loop data. (Allfunds is a platform, not trade media.) — [Allfunds](https://allfunds.com/)
- [M] Other European B2B fund platforms that sit in fund selectors' workflow: MFEX (acquired by Euroclear in 2021) and Clearstream Fund Centre (formerly UBS's Fondcenter, acquired 2021). — [MFEX](https://www.mfex.com/); [Clearstream](https://www.clearstream.com/)
- [M] UK: Dynamic Planner (risk profiling, asset allocation and fund research software widely used by advisers) offers fund managers a paid service to have funds and MPS risk-profiled and mapped to its risk levels. Profiled funds can then be found by advisers inside the software when matching portfolios to client risk profiles. This is the closest UK equivalent of being "in the EHR at the moment of prescribing". — [Dynamic Planner](https://www.dynamicplanner.com/)
- [M] UK: Defaqto (Diamond Ratings and the Engage adviser research software) is owned by Fintel plc (formerly SimplyBiz Group). Fintel also sells "distribution channel" services that give product providers access to its network of member advice firms. — [Defaqto](https://www.defaqto.com/); [Fintel](https://www.wearefintel.com/)
- [M] UK: Invesco acquired the adviser back-office/CRM software Intelliflo in 2020, a rare example of an asset manager owning adviser workflow software. — [Intelliflo](https://www.intelliflo.com/)
- [H] FinDatEx publishes the standard data templates distributors use for product governance and sustainability: EMT (European MiFID Template), EPT (European PRIIPs Template) and EET (European ESG Template). Complete, timely templates are a precondition for being selectable on many European platforms and buy lists. — [FinDatEx](https://findatex.eu/)
- [H] UK CPD (the CME equivalent): retail investment advisers must complete at least 35 hours of CPD a year, at least 21 of them structured, and hold an annual Statement of Professional Standing from an accredited body (e.g., CII/PFS, CISI, LIBF). — [FCA Handbook, TC sourcebook](https://www.handbook.fca.org.uk/handbook/TC/)
- [H] The EU Insurance Distribution Directive requires at least 15 hours of professional training a year for insurance distributors. That covers insurers' unit-linked and insurance-based investment product distribution, and the many French and Italian advisers who also distribute insurance. — [Directive (EU) 2016/97, EUR-Lex](https://eur-lex.europa.eu/eli/dir/2016/97/oj)
- [M] EFPA certifications (EIP, EFA, EFP) carry annual CPD requirements run by national affiliates (e.g., EFPA Italia, EFPA España), and asset managers commonly provide EFPA-accredited training sessions in Italy and Spain. — [EFPA Europe](https://www.efpa-europe.org/)
- [H] MiFID II inducement rules (the equivalent of pharma's hospitality and transfer-of-value rules): firms giving independent advice or portfolio management may accept only "acceptable minor non-monetary benefits". These include generic information about a financial instrument, participation in conferences, seminars and training on a specific instrument's benefits and features, and hospitality of a reasonable de minimis value. — [Delegated Directive (EU) 2017/593, Art. 12](https://eur-lex.europa.eu/eli/dir_del/2017/593/oj); [FCA COBS 2.3A](https://www.handbook.fca.org.uk/handbook/COBS/2/3A.html)
- [H] The same provisions treat third-party written material commissioned and paid for by a corporate issuer as an acceptable minor non-monetary benefit, provided the relationship is clearly disclosed and the material is made available at the same time to any firm wishing to receive it or to the general public. This is the legal basis for issuer-paid investment-company research (see Section 4). — [Delegated Directive (EU) 2017/593, Art. 12](https://eur-lex.europa.eu/eli/dir_del/2017/593/oj); [FCA COBS 2.3A](https://www.handbook.fca.org.uk/handbook/COBS/2/3A.html)
- [M] Sales-enablement tools already used across asset management provide the "Approved Email plus CLM" mechanics. Seismic LiveSend shares tracked content and shows which recipient opened which pages; Highspot and DocSend offer similar tracking. — [Seismic](https://seismic.com/); [Highspot](https://www.highspot.com/); [DocSend](https://www.docsend.com/)
- [M] AI-assisted compliance pre-review for financial marketing now exists (e.g., Saifr, which originated at Fidelity Labs). It is the asset-management counterpart of pharma's MLR tooling. — [Saifr](https://saifr.ai/)

### Inferences
Transfer "playbook cards". Feasibility is for a boutique-to-mid-sized UK manager; costs are the researcher's estimates, not sourced.

- **P1. Verified-professional identity layer (NPI/DocCheck → FRN and registry verification).**
  - *Source mechanism:* NPI-matched audiences in the US; DocCheck-gated professional content in Germany.
  - *Fund equivalent:* a professional hub whose sign-up asks for the firm's FRN (UK) or registry number (ORIAS, OCF, CNMV, Vermittlerregister, FINMA list) and checks it automatically against the public register. Paraplanners and DFM analysts are often not individually registered, so verify them by firm FRN plus a work-email domain.
  - *Payoff:* the result is a verified first-party audience that can be used for LinkedIn Matched Audiences (contact and company lists), consented email and on-site personalisation. It also becomes a defensible "professional investors only" gate for the content behind it.
  - *Feasibility:* high. Estimate £15–40k to build plus upkeep.
  - *Risks:* GDPR transparency when register data is reused (Art. 14 notices); register terms of use; PECR/UWG email rules; geo-gating by fund registration status per country.
- **P2. "Point-of-selection" presence (EHR point-of-care → fund-selection workflow).**
  - *Context:* in the UK and EU, in-tool display advertising is rare, much as in European EHRs. The pharma lesson that does transfer is to be present, correctly mapped and data-complete inside the tools where the choice is made.
  - *Fund equivalent:* Dynamic Planner risk profiling (UK advisers), Defaqto ratings/Engage, Allfunds Connect plus Telemetrics (EU bank and private-bank selectors), MFEX, Clearstream Fund Centre, and complete FinDatEx EMT/EPT/EET files.
  - *Feasibility:* high for data hygiene and risk profiling (modest fees); medium for Telemetrics-type analytics (platform fees, likely mid-five figures, unverified).
  - *Risks:* paying for ratings or profiles must be disclosed and must not compromise independence; UK platform payment rules (see the compliance researcher).
  - *Answers the brief's question:* ads inside fund-research tools are largely not available. The realistic equivalent is paid profiling, listings and analytics.
- **P3. Rep-triggered digital follow-up (Veeva Approved Email → "salesperson-triggered, compliance-pre-approved" sequences).**
  - *How it would work:* build a library of pre-approved modules (fund one-liners, risk warnings, monthly-refreshed charts, PM quotes, CPD invitations) in Seismic, Salesforce or HubSpot. Within 24 hours of a meeting, the salesperson assembles a follow-up from those modules and sends it from their own address. Opens are tracked. At the same time, the firm's buying group (company plus job titles) is retargeted on LinkedIn for 2–6 weeks.
  - *Fund equivalent:* this is the most directly transferable pharma tactic and is cheap, because it uses existing CRM and sales-enablement tools.
  - *Feasibility:* very high. Low cost, plus upfront compliance time.
  - *Risks:* approval of modules and their combinations; record-keeping. UK PECR treats sole-trader and some partnership IFAs as individual subscribers, so they need consent. Germany's UWG requires consent even for B2B email. For EU recipients, ESMA marketing-communication requirements apply.
- **P4. Closed-loop marketing → instrument every deck, factsheet, webinar and email.**
  - *How it would work:* log what each fund buyer viewed and asked in CRM. Hold a monthly "questions fund buyers asked" review, and let the most-asked questions set next month's content.
  - *Feasibility:* high. Low cost.
- **P5. CME model → accredited, independent CPD.**
  - *What to build:* CPD modules on topics next to the strategies, for example dividend-sustainability analysis, energy-transition supply chains, income design for decumulation, and evidencing fair value in income portfolios under Consumer Duty.
  - *Design rules:* use an independent faculty (academics, sector experts); get external CPD accreditation (UK CPD bodies, EFPA in Italy and Spain, IDD-eligible hours); keep the fund out of the module, with any product follow-up offered separately on an opt-in basis, as under ACCME.
  - *Distribution:* the firm's own hub, LinkedIn Document Ads and Lead Gen Forms, and professional associations rather than trade media (e.g., PIMFA, CISI, PFS regional groups, EFPA affiliates, ANASF, CNCGP/ANACOFI, ASEAFI, VuV, VSV/ASG).
  - *Feasibility:* high. Estimate £5–20k per module.
  - *Risks:* the content must genuinely be education (training is an allowed minor non-monetary benefit); each CPD body's rules; any mention of the fund turns the module into a promotion.
- **P6. KOL/DOL programme → a "trusted voices" map.**
  - *Rule:* do not pay practising fund selectors or advisers to promote funds. That is an inducement and a conflict of interest, and it is stricter than pharma, where HCP fees are permitted but disclosed.
  - *What to do instead:* map whom fund buyers follow (LinkedIn engagement, association speakers, podcast guests) and pay independent experts who do not advise (economists, energy analysts, dividend historians, academics, compliance trainers) to co-create content, with disclosure.
  - *MSL equivalent:* an "investment specialist / PM office hours" service for technical, non-sales exchange. UK and EU rules offer no non-promotional safe harbour like pharma's medical information, so treat it as promotion.
  - *Feasibility:* medium.
  - *Risks:* the FCA's social-media and influencer guidance (FG24/1, see Section 2) and disclosure.
- **P7. Next-best-action orchestration (Aktana/OCE → simple CRM rules).**
  - *Signals:* Telemetrics views, document opens, webinar attendance, LinkedIn company-level engagement, manager changes at competitor funds (public news), and each account's review-calendar dates. Each signal should trigger a specific salesperson task.
  - *Feasibility:* medium; it needs a clean CRM. Low to moderate cost.
  - *Risks:* GDPR and ePrivacy consent for tracking individuals.
- **P8. Market-access discipline (AMCP dossier → a "buy-list access kit").**
  - *Pharma model:* pharma separates payer and formulary access from promotion and makes reviews easy with standard dossiers.
  - *Fund equivalent:* a verified-hub due-diligence pack containing pre-filled DDQs, complete EMT/EPT/EET files, manufacturer-to-distributor fair-value information, holdings transparency, capacity and team-stability data, and SFDR/ESG data. Add a named access manager for research houses and platform fund-list teams, and a service level (e.g., any DDQ in five working days).
  - *Rationale:* this builds "physical availability" (see Section 5) at low cost. It is rarely marketed as a proposition.
  - *Feasibility:* very high.
- **Overall:** P3, P4, P5 and P8 give a boutique the best value. P1 and P2 are enabling infrastructure. P6 and P7 need careful compliance design.

### Gaps
- All pharma vendor benchmarks are missing because no page could be opened this session: Doceree engagement rates, OptimizeRx and DeepIntent script-lift/ROI figures, Veeva Pulse email open rates, and IQVIA/Indegene channel-mix data. No numbers are reported rather than recalled loosely. The common industry claim that rep-sent email gets far higher open rates than HQ-sent email is directional only.
- It is unverified whether Doceree, DeepIntent or PulsePoint operate HCP-verified programmatic at scale in the UK and EU under GDPR.
- It is unverified whether FE Analytics, Morningstar Direct/Adviser Workstation, Synaptic, Defaqto Engage, Dynamic Planner, Intelliflo, Harvest's Quantalys/O2S (France), Fida (Italy) or VDOS (Spain) sell in-tool advertising or sponsored placements. FE fundinfo also owns the media site Trustnet, which falls under the trade-media exclusion.
- Pricing is unknown for Allfunds Telemetrics, Dynamic Planner fund profiling and Fintel distribution-channel packages.
- The legal position on reusing FCA Register or Directory data (and EU registers) for marketing lists, and UK platform rules on payments from fund managers, belong to the regulatory researcher.
- Audience sizes are unverified: roughly 4,500–5,000 UK advice firms and 25,000–28,000 advisers (FCA data, recalled), and the number of EU fund selectors. Both matter for LinkedIn minimum-audience and frequency planning.

## 2. Enterprise B2B tech: account-based everything, buying groups, dark social, community, free tools, gifting, advocacy, creators, humour and CTV, and the 95:5 rule for periodic fund reviewers

### Takeaway
B2B tech faces an audience like fund buyers: small, mostly out of market at any moment, and researching largely out of sight through peers, private channels and self-serve content. The winning pattern combines three things:
- account-based targeting of whole buying groups;
- an always-on, distinctive, emotionally resonant brand presence that builds memory before the roughly 5% "in-market" window opens;
- distribution amplified by people (employees, creators, communities, physical mail).

For fund buyers who review periodically, this means a low-intensity, memory-building baseline across the defined account universe, plus activation timed to review calendars and trigger events. LinkedIn serves as the identity layer. TV/CTV is mostly unrealistic for a boutique.

### Cited Findings

#### Effectiveness research specific to B2B
- [H] **The 95:5 rule.** Prof. John Dawes of the Ehrenberg-Bass Institute, writing for the LinkedIn B2B Institute in 2021, showed that if business buyers switch provider about every five years, only about 20% are in market in a year and about 5% in a quarter. Roughly 95% of the people an ad reaches are therefore not buying now, so advertising's main job is to build memories that pay off at future purchase occasions. — [LinkedIn B2B Institute, "The 95-5 Rule"](https://business.linkedin.com/marketing-solutions/b2b-institute/b2b-research/trends/95-5-rule); [Ehrenberg-Bass Institute](https://marketingscience.info/)
- [H] **Brand-to-activation split.** Les Binet and Peter Field, *The 5 Principles of Growth in B2B Marketing* (2019, LinkedIn B2B Institute, using the IPA Effectiveness Databank), put the optimum B2B split at about 46% brand-building and 54% activation. The B2C optimum in *The Long and the Short of It* (IPA, 2013) is about 60:40. [M] The report also argues that emotional and "fame" effects drive long-term B2B growth, and that broad reach and excess share of voice (share of voice above share of market) predict growth. — [LinkedIn B2B Institute](https://business.linkedin.com/marketing-solutions/b2b-institute); [IPA](https://ipa.co.uk/)
- [H] **Time with suppliers.** Gartner found B2B buyers spend about 17% of total buying time meeting potential suppliers, split across all vendors they consider. Buying groups for complex purchases typically involve 6–10 decision makers. — [Gartner, B2B buying journey](https://www.gartner.com/en/sales/insights/b2b-buying-journey)
- [M] **Rep-free preference.** Gartner's 2023 sales survey reported that about 75% of B2B buyers prefer a rep-free buying experience, and that 44% of millennial buyers prefer no rep interaction at all. — [Gartner newsroom](https://www.gartner.com/en/newsroom)
- [M] **Shortlists form early.** 6sense's Buyer Experience Reports (2023–2024) found buyers are typically about 70% through their process before engaging sellers, and that in roughly four out of five cases they already have a preferred vendor at first contact. — [6sense](https://6sense.com/)
- [M] **Personal value.** CEB (now Gartner) and Google's *From Promotion to Emotion* (2013) found B2B buyers more emotionally connected to suppliers than consumers are to consumer brands. "Personal value" (career safety, confidence, pride) had about twice the impact of "business value" on purchase intent. — [Think with Google](https://www.thinkwithgoogle.com/)
- [M] **Thought leadership.** The annual Edelman–LinkedIn *B2B Thought Leadership Impact Report* consistently finds decision makers trust good thought leadership more than product marketing for judging a supplier's capabilities. It also reaches "hidden buyers", influential members of the buying group who never engage with sales. — [Edelman](https://www.edelman.com/)

#### Account-based targeting, buying groups and identity
- [H] The main ABM and intent vendors are 6sense, Demandbase and RollWorks (account identification, intent, orchestration) and Bombora, whose "Company Surge" intent data comes from a co-op of B2B publisher sites. Their data is strongest for tech and US firms. — [6sense](https://6sense.com/); [Demandbase](https://www.demandbase.com/); [RollWorks](https://www.rollworks.com/); [Bombora](https://bombora.com/)
- [M] An ITSMA (now Momentum ITSMA) survey (2014) found 84% of marketers said ABM delivered higher ROI than other marketing approaches. — [Momentum ITSMA](https://momentumitsma.com/)
- [M] Forrester's revised B2B Revenue Waterfall (2021) moved measurement from individual leads to buying groups and opportunities. — [Forrester](https://www.forrester.com/)
- [H] LinkedIn passed 1 billion members in 2023. Campaigns need a targetable audience of at least 300 members. Matched Audiences accept uploaded company lists and contact lists. Lead Gen Forms prefill members' profile data. — [LinkedIn Marketing Solutions](https://business.linkedin.com/marketing-solutions)
- [M] European GDPR-oriented B2B contact and intent data vendors include Cognism (London) and Dealfront (formed 2022 from Echobot and Leadfeeder). — [Cognism](https://www.cognism.com/); [Dealfront](https://www.dealfront.com/)

#### Dark social and word of mouth
- [H] Alexis Madrigal coined "dark social" in *The Atlantic* (October 2012) for sharing through private channels (email, messaging) that analytics cannot see. — [The Atlantic](https://www.theatlantic.com/technology/archive/2012/10/dark-social-we-have-the-whole-history-of-the-web-wrong/263523/)
- [M] B2B practitioners, notably Refine Labs (Chris Walker), popularised "self-reported attribution": a free-text "How did you hear about us?" field that captures influence from dark social, podcasts and peers which software attribution misses. — [Refine Labs](https://www.refinelabs.com/)

#### Community-led growth and free tools
- [M] Examples of community-led B2B growth: Salesforce's Trailblazer Community (users helping users, which drives adoption and certification); dbt Labs' large practitioner Slack community; and Pavilion (formerly Revenue Collective), a paid membership community for revenue leaders. Typical platforms are Slack, Circle, Discourse, Bevy and WhatsApp Communities. — [Salesforce Trailblazer Community](https://trailhead.salesforce.com/); [dbt Labs](https://www.getdbt.com/); [Pavilion](https://www.joinpavilion.com/)
- [M] HubSpot's free Website Grader (launched around 2007) is the standard example of a free tool used as marketing. Gabriel Weinberg and Justin Mares's *Traction* (2014) named "engineering as marketing" as one of 19 traction channels. — [HubSpot Website Grader](https://website.grader.com/); [Traction](https://www.tractionbook.com/)

#### Gifting, programmatic direct mail and personalised microsites
- [H] Reachdesk (founded in London), Sendoso, PFL and Postal integrate with Salesforce and HubSpot. They trigger physical or e-gifts and direct mail from CRM events, track delivery, add QR codes or personalised URLs, and attribute pipeline. — [Reachdesk](https://reachdesk.com/); [Sendoso](https://www.sendoso.com/); [PFL](https://www.pfl.com/); [Postal](https://www.postal.com/)
- [M] Account-specific web experiences: Mutiny (AI personalisation and account-specific pages), Folloze, Uberflip and PathFactory (curated content hubs per account). — [Mutiny](https://www.mutinyhq.com/); [Folloze](https://www.folloze.com/); [Uberflip](https://www.uberflip.com/); [PathFactory](https://www.pathfactory.com/)
- [H] UK JICMAIL measures how addressed mail, business mail and door drops are kept, re-read and acted on, including the lifespan and frequency of interaction. — [JICMAIL](https://www.jicmail.org.uk/)
- [M] Royal Mail MarketReach and Millward Brown's 2009 neuroscience study with Bangor University found physical mail produced stronger emotional processing and memory encoding than on-screen equivalents. — [Royal Mail MarketReach](https://www.marketreach.co.uk/)
- [H] UK rules for physical outreach:
  - Postal marketing to named business contacts can rely on legitimate interests, with an opt-out.
  - PECR's email consent requirement does not apply to "corporate subscribers" (companies, LLPs, Scottish partnerships, public bodies).
  - It does apply to sole traders and other partnerships, which describes many small IFA firms.
  - Gifts and hospitality fall under the Bribery Act 2010, including the section 7 "failure to prevent" offence and its adequate-procedures defence.
  — [ICO, business-to-business marketing](https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-communications/business-to-business-marketing/); [Bribery Act 2010](https://www.legislation.gov.uk/ukpga/2010/23/contents)
- [H] Germany is stricter than the UK: §7(2) no. 2 UWG requires prior express consent for email advertising to any recipient, businesses included. Continental B2B email programmes therefore need opt-in capture, for example through a verified hub or webinar registration. — [UWG §7 (gesetze-im-internet.de)](https://www.gesetze-im-internet.de/uwg_2004/__7.html)

#### Employee advocacy and creators
- [M] Employee-advocacy platforms include Haiilo (formed from the Smarp and COYO merger) and DSMN8 (UK), alongside LinkedIn's own "My Company" tab. LinkedIn has said employees typically have about 10 times as many connections as their company page has followers. — [Haiilo](https://haiilo.com/); [DSMN8](https://dsmn8.com/); [LinkedIn Marketing Solutions](https://business.linkedin.com/marketing-solutions)
- [H] The FCA's FG24/1, *Finalised guidance on financial promotions on social media* (March 2024), says:
  - a social-media post can be a financial promotion whatever the channel or poster;
  - firms are responsible for promotions they communicate or approve;
  - staff posting about their firm's products on personal accounts may be communicating financial promotions;
  - paid influencers promoting financial products must comply with the s21 FSMA restriction.
  — [FCA FG24/1](https://www.fca.org.uk/publications/finalised-guidance/fg24-1-finalised-guidance-financial-promotions-social-media)
- [M] LinkedIn's creator and advocacy tools:
  - Thought Leader Ads launched in 2023 for boosting employees' posts; in 2024 they were extended to any member's post with permission (customers, partners, creators).
  - BrandLink (2024) lets advertisers sponsor video from LinkedIn creators and premium publishers, with pre-roll ads.
  - "Creator mode" was retired in 2024, making newsletters, LinkedIn Live and follow tools available to everyone.
  — [LinkedIn Marketing Solutions](https://business.linkedin.com/marketing-solutions)

#### Humour, distinctive assets and TV/CTV
- [H] Jenni Romaniuk's *Building Distinctive Brand Assets* (2018) argues that colours, characters, logos and sonic cues work as memory triggers only when they are both well known and unique to the brand. — [Ehrenberg-Bass Institute](https://marketingscience.info/)
- [M] Workday's first Super Bowl ad, "Rock Star" (February 2023), cast Ozzy Osbourne, Joan Jett, Billy Idol, Paul Stanley and Gary Clark Jr. to mock corporate overuse of "rock star". It shows a pure B2B brand using comedy on the largest TV stage. — [Workday newsroom](https://newsroom.workday.com/)
- [M] Mailchimp's "Did You Mean Mailchimp?" (2019, Droga5) built an award-winning campaign out of deliberate mis-namings (MailShrimp, KaleLimp and others), showing humour paired with a distinctive brand asset. — [Mailchimp](https://mailchimp.com/)
- [M] Asset-management brand platforms show the category can do brand work: Baillie Gifford's long-running "Actual Investors" platform (print, TV, podcasts) and Ninety One's 2020 rebrand from Investec Asset Management. — [Baillie Gifford](https://www.bailliegifford.com/); [Ninety One](https://ninetyone.com/)
- [H] Thinkbox, the UK commercial-TV marketing body, publishes effectiveness evidence for TV and broadcaster video on demand (BVOD) and tracks advertiser categories. — [Thinkbox](https://www.thinkbox.tv/)

### Inferences
- **B1. Account-based "fund-buyer universe" with buying-group mapping.**
  - *Tier the accounts:*
    - Tier 1, about 50–150 gatekeeper firms: DFM and MPS teams, network investment committees, private banks, platform fund-list teams, multi-managers, family offices, and research houses (inform only, never incentivise).
    - Tier 2, about 500–1,500 advice firms with their own investment committees or centralised investment propositions.
    - Tier 3, the long tail reached by job title.
    - Europe: bank and private-bank selector desks, Swiss independent asset managers (FINMA list), French CGPs (ORIAS), Spanish EAFs (CNMV), German Vermögensverwalter (VuV) and broker pools.
  - *Map each buying group:* CIO or head of research, fund analysts, MPS portfolio managers, investment-committee members, product-governance and compliance staff (who own target-market and fair-value reviews), paraplanners (who do the research and suitability work), client-facing advisers, and platform fund-list analysts.
  - *Delivery:* LinkedIn company-list Matched Audiences crossed with job functions, staying above the 300-member minimum, plus salesperson coverage of Tier 1.
  - *Intent data:* third-party intent co-ops (e.g., Bombora) are probably thin for UK and EU fund buyers. First-party signals (Allfunds Telemetrics, verified-hub behaviour, factsheet downloads) are worth more.
  - *Feasibility:* high. Spend estimate for a boutique: £5–25k a month on LinkedIn.
  - *Risks:* GDPR lawful basis for contact uploads; target only countries where the fund is registered or notified.
- **B2. Design for dark social.**
  - *How fund buyers share:* via WhatsApp, Teams, email and investment-committee packs.
  - *Build assets made to be forwarded:* a "chart of the month" PDF in distinctive house style; one-page summaries ready for an investment committee; 60–90-second explainers. Each carries its professional-only labelling and risk wording, so it stays compliant after forwarding.
  - *Measure:* add self-reported attribution to every sign-up form and salesperson note, and track branded search and direct traffic.
  - *Feasibility:* high. Low cost.
  - *Risk:* forwarded material reaching retail investors.
- **B3. Community-led growth.** An owned Slack or Circle community needs critical mass and moderation that most boutiques cannot sustain.
  - *More realistic for a boutique:* partner with professional bodies (PIMFA, CISI branches, PFS regional groups, CFA societies, EFPA chapters, ANASF, CNCGP/ANACOFI, ASEAFI, VuV, VSV/ASG) to supply content and speakers for their communities.
  - *Or:* build a small "community of practice" around a data product (see Section 4), e.g., quarterly round tables for users of an income-resilience tracker.
  - *WhatsApp caution:* record-keeping and "off-channel" risk. US regulators levied about $1.8bn of off-channel fines in September 2022 alone (SEC $1.1bn plus CFTC about $710m) [M] ([SEC press release 2022-174](https://www.sec.gov/news/press-release/2022-174)), so keep communities on archived platforms.
- **B4. Product-led growth through free tools.** Highly relevant; developed in Section 4.
- **B5. ABM gifting and programmatic direct mail.**
  - *What to send:* MiFID inducement rules and buyers' gift registers make luxury gifts a liability, so send "information-gifts" instead. Examples: a well-produced printed annual (e.g., a dividend atlas or energy-transition yearbook), a desk-worthy data poster, a book by the PM.
  - *How to deliver:* trigger sends from CRM through Reachdesk or Sendoso after meetings or ahead of a known review window. A QR code leads to an account-specific microsite (Mutiny, Folloze, Uberflip). The same accounts are retargeted on LinkedIn and then followed up by a salesperson.
  - *Feasibility:* high. Estimate £30–80 per pack all-in, for 200–1,000 named people.
  - *Risks:* de minimis and inducement tests, the Bribery Act, recipients' gift policies, GDPR legitimate-interest assessment and opt-outs, and EU customs/VAT friction after Brexit.
- **B6. Employee advocacy at boutique scale.** Five to fifteen credible voices (PMs, analysts, product specialists) beat a corporate page.
  - *How:* use Haiilo or DSMN8, or simply LinkedIn's My Company tab, and boost the best posts with Thought Leader Ads aimed at buying groups.
  - *Feasibility:* high. Estimate £5–20k a year for a platform, plus ad spend.
  - *Risks:* FG24/1. Pre-approve product-related posts, keep an archive, and write a personal-account policy.
- **B7. B2B creator partnerships, adapted.** Partner with educators and specialists who do not advise clients (technical-paraplanning trainers, retirement-income researchers, economists, energy analysts) through co-hosted LinkedIn Lives, sponsored newsletter issues, disclosed paid partnerships and Thought Leader Ad boosts.
  - *Do not pay practising advisers or fund selectors.* This is the key difference from B2B tech, because it creates inducement and conflict problems.
  - *Feasibility:* medium.
  - *Risks:* s21 approval and disclosure under FG24/1, and ESMA marketing-communication rules for EU audiences.
- **B8. Distinctive assets and (careful) humour.** Fund marketing is visually uniform (blue palettes, mountains, compasses), which leaves room for distinctive assets: a recurring character or colour, one chart style, a sonic signature for audio and video, and named recurring formats (e.g., "The Monday Dividend", "One Chart on the Transition").
  - *Humour:* aim it at industry quirks (jargon, meeting fatigue), never at risk or returns.
  - *Feasibility:* medium-high. Estimate £30–100k for a creative platform.
  - *Risk:* balanced presentation of risk; content reaching retail.
- **B9. TV/CTV.** For an audience of tens of thousands of professionals across the UK and Europe, linear TV mostly wastes money, and B2B-targeted CTV is immature and expensive in Europe.
  - *Better:* video made first for LinkedIn and YouTube with B2B targeting, plus an owned podcast (not a trade-media one).
  - *Exception:* BVOD becomes justifiable only for a mid-sized manager that also wants a retail brand, with advisers reached as a side effect.
  - *Feasibility:* low for a boutique.
- **95:5 applied to fund buyers.**
  - *Why most selectors are out of market:* many funds stay on buy lists and in model portfolios for years, so at any moment a selector is usually not shopping for a given sector slot.
  - *When they come into market:*
    - scheduled points (quarterly MPS rebalances, annual buy-list or panel reviews, annual value and fair-value assessments);
    - triggers (a manager departure, style drift, a drawdown, a fund merger or closure, a new client need such as decumulation income, an energy or rates shock, a regulatory change).
  - *What to do:*
    - keep a continuous, low-frequency presence across the whole account universe (about 1–2 exposures a week per person plus a monthly email and a quarterly physical touch, all estimates);
    - aim to be the default name for two or three category entry points;
    - concentrate bursts on known review windows;
    - add trigger-based activation (see Sections 4 and 5).

### Gaps
- No vendor benchmark could be retrieved this session for: Reachdesk/Sendoso/PFL response or meeting rates, Mutiny conversion uplift, Haiilo/DSMN8 reach multipliers, the click-through of Thought Leader Ads versus standard ads, or JICMAIL business-mail figures.
- Unverified: whether LinkedIn CTV inventory and BrandLink are generally available to UK and EU advertisers as of late 2026, and the current status of the LinkedIn B2B Institute's research programme.
- No documented case of an asset manager running a successful owned community for fund buyers was found (search was unavailable).
- No data on how UK and EU fund buyers share material privately (WhatsApp, Teams, investment-committee packs), on actual LinkedIn reach among paraplanners and continental fund selectors, or on typical buy-list holding periods and review frequencies. Primary research (a short survey or interviews) would close these.

## 3. Professional services, private banking and luxury: proprietary research and indices, benchmarking, clienteling, and lessons from marketing to wealth managers' own clients

### Takeaway
The best professional-services marketing assets work as PR, advertising and sales tools at once: an annual or quarterly proprietary report, index or ranking with a recognisable name. The strongest of them, such as the Knight Frank Wealth Report, are built partly from surveys of the intermediaries themselves, so the audience helps make the asset. For a boutique equity-income or thematic manager, a narrow, frequent, data-led index, plus "clienteling" of each gatekeeper's review calendar and content that makes the gatekeeper look good to clients and investment committees, transfers better than imitating big-bank wealth reports.

### Cited Findings
- [H] **Knight Frank Wealth Report.** Published annually since 2007. It combines wealth-population data with an "Attitudes Survey" of private bankers, wealth advisers and family offices, the Prime International Residential Index (PIRI 100), and the Knight Frank Luxury Investment Index (KFLII), which tracks collectables such as art, wine, watches, classic cars, whisky and handbags. Intermediaries are both sources and audience. — [Knight Frank, The Wealth Report](https://www.knightfrank.com/wealthreport)
- [H] **UBS Global Wealth Report.** UBS has published it since 2023, after taking over Credit Suisse, continuing the Credit Suisse Global Wealth Report series that began in 2010. Global media cite it every year for millionaire counts and wealth distribution. — [UBS Global Wealth Report](https://www.ubs.com/global/en/wealthmanagement/insights/global-wealth-report.html)
- [M] UBS also publishes a Global Family Office Report (a survey of family offices, which are part of this brief's audience) and Billionaire Ambitions (earlier editions with PwC). — [UBS](https://www.ubs.com/)
- [H] **UBS Global Investment Returns Yearbook.** Compiled by Elroy Dimson, Paul Marsh and Mike Staunton and formerly the Credit Suisse Yearbook, it provides long-run asset-return history and is cited for years after each edition. It is an "evergreen" reference asset. — [UBS](https://www.ubs.com/)
- [M] **Capgemini World Wealth Report.** Published since 1997 (originally with Merrill Lynch). It covers HNWI population and wealth and includes surveys of HNWIs and wealth-management executives. — [Capgemini World Wealth Report](https://www.capgemini.com/insights/research-library/world-wealth-report/)
- [H] **Henley Passport Index.** Henley & Partners has ranked passports by visa-free access, using IATA data, since 2006. A residence- and citizenship-advisory firm turned it into a recurring global PR asset. Henley also publishes the Private Wealth Migration Report. — [Henley Passport Index](https://www.henleyglobal.com/passport-index)
- [M] **Asset-management precedents for proprietary data assets:**
  - Janus Henderson Global Dividend Index: quarterly analysis of dividends paid by about 1,200 of the largest listed companies, running since the mid-2010s. Its direct relevance to equity income means a boutique must differentiate rather than copy it.
  - Computershare (formerly Link Group) UK Dividend Monitor: quarterly.
  - Natixis Global Survey of Fund Selectors: an annual survey of professional fund buyers, proof that a manager can make fund selectors the subject of its research.
  - Schroders Global Investor Insights survey.
  - J.P. Morgan Asset Management's quarterly Guide to the Markets chart book, a staple adviser reference.
  - BlackRock Investment Institute's Geopolitical Risk Dashboard: an interactive tracker updated regularly.
  - Fidelity International's annual Analyst Survey, built from its in-house analysts' views.
  — [Janus Henderson](https://www.janushenderson.com/); [Computershare UK](https://www.computershare.com/uk); [Natixis IM](https://www.im.natixis.com/); [Schroders](https://www.schroders.com/); [J.P. Morgan AM](https://am.jpmorgan.com/); [BlackRock Geopolitical Risk Dashboard](https://www.blackrock.com/corporate/insights/blackrock-investment-institute/interactive-charts/geopolitical-risk-dashboard); [Fidelity International](https://www.fidelityinternational.com/)
- [H] Howard Marks's memos to Oaktree clients (since 1990) show a named, idiosyncratic, long-running PM letter becoming a firm's main brand asset. [M] Warren Buffett has said a Marks memo is the first thing he opens in his mail. — [Oaktree, Memos](https://www.oaktreecapital.com/insights/memos)
- [H] In B2B tech, Gartner's Magic Quadrant shows how a third-party evaluation framework becomes a buying shortcut that vendors then amplify in their own marketing. — [Gartner](https://www.gartner.com/)
- [M] Benchmarking research as marketing: PwC's Annual Global CEO Survey (since 1998) gives a professional-services firm an annual reason to contact C-suite clients. In the UK adviser market, independent research consultancies publish benchmark studies, some with provider sponsorship: NextWealth (financial-advice business benchmarks and managed-money research), the lang cat (adviser-market studies) and Fundscape (platform-market data). — [PwC](https://www.pwc.com/); [NextWealth](https://www.nextwealth.co.uk/); [the lang cat](https://www.langcatfinancial.co.uk/); [Fundscape](https://www.fundscape.co.uk/)
- [M] **Clienteling in luxury retail.** Clienteling apps (e.g., Salesforce, Tulip) give store associates each client's purchase history, preferences and important dates so they can make personal outreach. — [Salesforce](https://www.salesforce.com/); [Tulip](https://tulip.com/)
- [M] **Clienteling in wealth management.** Morgan Stanley Wealth Management rolled out "Next Best Action" in 2018, a machine-learning system suggesting timely, personalised client contacts to its roughly 15,000 financial advisers. It followed with the generative-AI tools "AI @ Morgan Stanley Assistant" (2023) and "Debrief" (2024), built with OpenAI. — [Morgan Stanley](https://www.morganstanley.com/)
- [H] **UK Consumer Duty.** In force from 31 July 2023 for open products, it includes a "consumer understanding" outcome and requires manufacturers and distributors to share information along the distribution chain (PRIN 2A). Gatekeepers therefore value material that helps them evidence client understanding and fair value. — [FCA Consumer Duty](https://www.fca.org.uk/firms/consumer-duty)
- [H] UK authorised fund managers must publish an annual Assessment of Value for each fund (COLL 6.6.20R, since 2019). This creates a recurring, scheduled moment when fund buyers re-examine value. — [FCA Handbook, COLL 6.6](https://www.handbook.fca.org.uk/handbook/COLL/6/6.html)
- [M] Asset managers in the US supply "client-ready" material that advisers use with their own clients, such as J.P. Morgan's Guide to Retirement and Vanguard's "Adviser's Alpha" research quantifying the value of advice. The model is content that makes the intermediary look good. — [J.P. Morgan AM](https://am.jpmorgan.com/); [Vanguard](https://www.vanguard.com/)

### Inferences
- **S1. A boutique flagship index or report.** Copy the Knight Frank structure (survey of intermediaries + proprietary index + rankings) at boutique scale. The value is in being narrower and more frequent than the big-bank reports.
  - *Candidate assets:* (a) a "Dividend Resilience Index" (cuts, raises, cover and payout sustainability for UK, European or global income stocks; it must be clearly differentiated from Janus Henderson's index); (b) an energy-transition capex and earnings tracker; (c) a quarterly "Fund Selector Pulse" of three to five questions that gives salespeople a reason to call.
  - *Distribution:* LinkedIn chart ads to buying groups, mainstream business-press PR (general titles only, not adviser or fund trade media), salesperson follow-ups and print copies in direct mail.
  - *Feasibility:* medium-high. Estimate £40–150k a year for data, survey, design and PR.
  - *Risks:* methodological credibility; data-licensing costs; keeping survey thank-yous de minimis (a charity donation, say); any product mention turns it into a financial promotion.
- **S2. Benchmarking as a service.** Offer fund-buyer firms an anonymised peer benchmark, for example on the income yield, sector concentration or energy-transition exposure of MPS ranges, built from public factsheets or submitted data.
  - *Partner option:* independent research consultancies (NextWealth, the lang cat). Their status against the "no trade media" rule needs a quick check by the user.
  - *Feasibility:* medium.
  - *Risks:* data accuracy; fairness in comparative claims.
- **S3. Clienteling for gatekeepers.** Keep a per-account profile: review calendar (MPS rebalance dates, investment-committee meetings, buy-list review months), preferred formats, constraints (ESG exclusions, liquidity), topics of interest and relationship history. Feed it into next-best-action prompts and time content to each firm's calendar.
  - *Borrow from luxury:* small, invitation-only PM round tables, framed as training and kept within MiFID de minimis hospitality.
  - *Feasibility:* high. Low cost. Probably the highest-ROI idea in this section.
- **S4. Make the gatekeeper look good.** This applies the CEB/Google "personal value" finding and mirrors pharma's patient-education leaflets.
  - *What to supply:* comprehension-tested client-understanding explainers that support Consumer Duty evidence; "investment-committee-ready" summary packs for DFMs; rapid "what to tell clients when oil drops 20%" briefings.
  - *Feasibility:* high.
  - *Risk:* anything intended for retail end-clients is a retail financial promotion and needs full retail-standard approval. Keep professional-only and client-facing versions strictly separate.
- **S5. An evergreen data book** (on the Dimson–Marsh–Staunton yearbook model), e.g., a long-run dividends or energy-transition data book refreshed annually in print and PDF. It sits on desks for years and builds mental availability (see Section 5). Feasibility: medium.
- **S6. A named PM letter** (on the Howard Marks model), carried as a LinkedIn newsletter and email (see Section 4). Feasibility: high, provided the PM can write distinctively.

### Gaps
- Documented outcomes (media mentions, leads, assets gathered) for the Knight Frank, UBS, Henley, Janus Henderson and Natixis assets could not be retrieved, so no PR benchmarks are given.
- Typical response rates, sample sizes and costs for fund-selector surveys in the UK and Europe are unknown.
- Unverified whether NextWealth, the lang cat and Fundscape take asset-manager sponsorship in 2026. Some run events and publish content, so the user should decide whether they fall under the trade-media exclusion.
- No published ROI was found for wealth-management clienteling or next-best-action tools (e.g., Morgan Stanley's).

## 4. Unconventional finance-specific ideas: free tools, paid research, PM office hours, triggered creative, year-in-review, gamified CPD, mail plus retargeting, newsletters with Thought Leader Ads, and puzzles

### Takeaway
Of these ideas, the most promising for B2B fund buyers are:
- a genuinely useful free data tool tied to the strategy's expertise, such as a dividend-resilience screener or an energy-transition tracker built on openly licensed data;
- a PM-voiced LinkedIn newsletter amplified with Thought Leader Ads to account lists;
- bookable "PM office hours";
- market-triggered creative switched from a pre-approved library.

Issuer-paid research works neatly for investment trusts but has no clean open-ended-fund equivalent. Personalised year-in-review content and puzzle campaigns are cheap, distinctive brand-builders as long as they stay away from performance claims. Gamified CPD is credible if it is built on spaced-repetition evidence rather than gimmicks.

### Cited Findings

#### Free interactive tools and data products as marketing
- [H] BlackRock Investment Institute runs an interactive Geopolitical Risk Dashboard tracking the likelihood and market attention of top geopolitical risks. It is a recurring reason for professionals to revisit and cite BlackRock. — [BlackRock Geopolitical Risk Dashboard](https://www.blackrock.com/corporate/insights/blackrock-investment-institute/interactive-charts/geopolitical-risk-dashboard)
- [M] Schroders' Climate Progress Dashboard (launched in the late 2010s) tracks indicators of climate action and translates them into an implied long-term temperature rise. It is an asset-manager-branded thematic tracker. — [Schroders](https://www.schroders.com/)
- [M] Natixis Investment Managers' Portfolio Research and Consulting Group offers advisers free portfolio analysis ("Portfolio Clarity") and publishes aggregate insight from thousands of adviser portfolios it has reviewed. The free analysis doubles as lead generation and as content. — [Natixis IM](https://www.im.natixis.com/)
- [M] BlackRock offers advisers portfolio-analytics and portfolio-consultation tools; Morningstar's Portfolio X-Ray is a long-standing free analysis tool. Both are "product-led" entry points to a relationship. — [BlackRock](https://www.blackrock.com/); [Morningstar UK](https://www.morningstar.co.uk/)
- [M] Data sources for a thematic tool:
  - Ember, an independent energy think tank, publishes open electricity-transition data (e.g., its Global Electricity Review) under a Creative Commons licence that permits reuse with attribution.
  - IEA data is a mix of free and paid licences.
  - BloombergNEF is subscription-only.
  — [Ember](https://ember-energy.org/); [IEA](https://www.iea.org/); [BloombergNEF](https://about.bnef.com/)

#### Paid-for independent research
- [H] Edison Group (London, founded 2003) produces issuer-sponsored research, including on investment companies. It is disclosed as paid for by the issuer and made freely available, which fits the MiFID issuer-paid research exemption cited in Section 1. — [Edison Group](https://www.edisongroup.com/)
- [M] Kepler Trust Intelligence (Kepler Partners LLP) publishes research on investment trusts for professional and private investors. Research on a given trust is commissioned and paid for by that trust and labelled as such. — [Kepler Trust Intelligence](https://www.trustintelligence.co.uk/)
- [M] Hardman & Co (London) provides issuer-paid research on listed companies and investment companies, plus investor events. — [Hardman & Co](https://www.hardmanandco.com/)
- [M] Marten & Co (founded 2013) produces issuer-paid research on investment companies and publishes under the QuotedData brand. QuotedData also operates as an investment-trust news outlet, so it is borderline under the trade-media exclusion. — [QuotedData / Marten & Co](https://quoteddata.com/)
- [M] Open-ended funds have no direct "issuer-paid research" market. The nearest equivalents are research and ratings firms where any payment comes after an independent assessment, for licensing the rating or for marketing services: FundCalibre (consumer-facing; run by Chelsea Financial Services), RSMR, Square Mile and Defaqto. — [FundCalibre](https://www.fundcalibre.com/); [RSMR](https://www.rsmr.co.uk/); [Square Mile](https://www.squaremileresearch.com/); [Defaqto](https://www.defaqto.com/)

#### Bookable access, triggered creative and data-driven formats
- [H] Scheduling tools (Calendly, Chili Piper) plug into web forms and CRM so a prospect can book a slot straight from an ad or landing page. LinkedIn Lead Gen Forms can pass data to CRM and marketing-automation tools. — [Calendly](https://calendly.com/); [Chili Piper](https://www.chilipiper.com/); [LinkedIn Marketing Solutions](https://business.linkedin.com/marketing-solutions)
- [M] Dynamic creative optimisation (DCO) tools take live data feeds (weather, scores, prices, inventory) and change ad copy or imagery automatically. Examples include Google Display & Video 360 / Studio dynamic feeds, Bannerflow, Celtra and Flashtalking (Mediaocean). — [Google Marketing Platform](https://marketingplatform.google.com/); [Bannerflow](https://www.bannerflow.com/); [Celtra](https://www.celtra.com/); [Flashtalking](https://www.flashtalking.com/)
- [M] LinkedIn's Marketing API supports programmatic campaign and creative management, so pre-built campaigns can be paused or activated from external rules (e.g., a market move) through custom code or automation vendors. — [LinkedIn Marketing API documentation](https://learn.microsoft.com/en-us/linkedin/marketing/)
- [H] UK rules on past performance in financial promotions (COBS 4.6) and the EU's ESMA marketing-communication guidelines restrict how performance figures may be shown: standard periods, sources, warnings and consistency with legal documents. Triggered creative should therefore switch market context and messaging, not fund performance. — [FCA Handbook, COBS 4.6](https://www.handbook.fca.org.uk/handbook/COBS/4/6.html); [Regulation (EU) 2019/1156, EUR-Lex](https://eur-lex.europa.eu/eli/reg/2019/1156/oj)
- [H] Cross-border registration constrains any pan-European digital campaign. A UCITS may be marketed in another EEA state only after its home regulator notifies the host state (UCITS Directive, Art. 93). Since Brexit, UK-authorised funds (OEICs) count as non-EU AIFs in the EU. They can be marketed to professional investors only through each country's national private-placement regime, where one exists (AIFMD, Art. 42). Ads, tools and office-hours invitations must therefore be geo-fenced by each fund's registration status. — [UCITS Directive 2009/65/EC](https://eur-lex.europa.eu/eli/dir/2009/65/oj); [AIFMD 2011/61/EU](https://eur-lex.europa.eu/eli/dir/2011/61/oj)
- [M] Switzerland: offering foreign funds to qualified investors who are not regulated institutions generally requires a Swiss representative and paying agent under the Collective Investment Schemes Act (CISA), and FinSA client-adviser registration applies to some intermediaries. — [FINMA](https://www.finma.ch/)

#### Year-in-review, gamification and learning science
- [H] Spotify Wrapped, launched in 2016, set the template for personalised, shareable year-in-review content, and many apps and B2B software firms have copied it. — [Spotify Newsroom](https://newsroom.spotify.com/)
- [M] Qstream, a spaced-repetition microlearning platform used by pharma sales teams among others, is based on Dr B. Price Kerfoot's research at Harvard. Randomised trials (e.g., Kerfoot et al., *Medical Education*, 2007; Kerfoot & Baker, *Annals of Surgery*, 2012, a spaced-education "game" for continuing medical education) found spaced, question-based and competitive formats improved knowledge retention among medical students and physicians. — [Qstream](https://qstream.com/)

#### LinkedIn newsletters
- [M] On LinkedIn, newsletter subscribers are notified, in-app and by email, when each new issue is published. Members and company pages can both publish newsletters, which builds an owned, opted-in audience inside the platform. — [LinkedIn Help](https://www.linkedin.com/help/linkedin)

#### Puzzles, ARGs and games used by financial and security employers
- [H] In 1942 the *Daily Telegraph* crossword was used to identify potential codebreakers for Bletchley Park, the founding example of a puzzle used for recruitment. — [Bletchley Park](https://bletchleypark.org.uk/)
- [M] GCHQ ran the online recruitment puzzle "Can You Crack It?" (2011) and has issued Christmas-card puzzles since 2015 (first via its then director). Both drew mass participation and global media coverage. — [GCHQ](https://www.gchq.gov.uk/)
- [H] Jane Street publishes a monthly puzzle with a public list of correct solvers, a long-running recruitment and brand device. [M] It also invented the trading card game "Figgie" and released it publicly. — [Jane Street Puzzles](https://www.janestreet.com/puzzles/); [Figgie](https://www.figgie.com/)
- [M] Two Sigma ran "Halite", an AI-programming competition (from 2016), as a recruitment and brand tool. IMC (Prosperity) and Optiver run trading challenges aimed at students. — [Halite](https://halite.io/); [IMC](https://www.imc.com/); [Optiver](https://optiver.com/)

### Inferences
Each idea is judged for B2B fund-buyer relevance. Costs are the researcher's estimates.

- **U1. A free interactive tool or data product.** Relevance: high. Feasibility: medium.
  - *Options:*
    - (a) a dividend-resilience screener showing cover, free-cash-flow payout, balance-sheet strength and growth streaks for a global income universe;
    - (b) an energy-transition tracker of renewables additions, EV share, grid capex and battery costs, built mainly on Ember's openly licensed data plus company filings, with fortnightly PM commentary and an "export this chart for your investment committee" button;
    - (c) an MPS income X-ray using non-personal model-portfolio inputs.
  - *Why it works:* it creates repeat visits, which is mental availability (Section 5), and gives salespeople a reason to call.
  - *Promotion:* LinkedIn account-list ads, salesperson sharing and search, with light FRN verification for advanced features.
  - *Cost:* £40–150k to build plus £20–60k a year for data and upkeep.
  - *Risks:*
    - market-data redistribution licences (security-level data from FactSet, LSEG, Bloomberg or index providers can be expensive);
    - if the tool outputs stock-level views, it may count as an "investment recommendation" under the Market Abuse Regulation, with disclosure duties;
    - keep it generic and public so it stays outside MiFID research and inducement concerns;
    - any reference to the fund inside the tool is a promotion.
- **U2. Paid-for independent research.** Relevance: high for investment trusts (the Edison/Kepler/Hardman/Marten model works as-is if the manager runs a trust); low to medium for OEICs and UCITS.
  - *Open-ended alternatives:*
    - (a) pursue independent ratings from firms that cannot be paid for the verdict;
    - (b) fund disclosed academic or independent research on the asset class itself, such as long-run dividend-growth returns or transition capex cycles, mirroring pharma's independent research grants;
    - (c) commission explicitly labelled "paid-for" strategy notes, though selectors may discount them.
  - *Cost:* £10–40k per paper.
  - *Risks:* perceived bias; labelling; whether the issuer-paid exemption covers a UCITS ManCo (see Gaps).
- **U3. "PM office hours" bookable from ads.** Relevance: high. Feasibility: high, since PM time is the only real constraint.
  - *Format:* a Thought Leader Ad from the PM, e.g., "Every other Thursday I hold 20-minute office hours for fund selectors — bring your hardest question on dividend cuts." It links to a verified booking page (Calendly or Chili Piper, with firm and FRN check) offering capped places in 1:1 or small-group (5–8) video sessions. The P3 follow-up sequence runs afterwards.
  - *Why it works:* a boutique's PMs are more reachable than a mega-manager's, so access is a selling point. Capped places also add scarcity, as in luxury marketing. This is the MSL "scientific exchange" idea adapted, but treated as promotion.
  - *Risks:* real-time promotion rules and exemptions for investment professionals (see compliance researcher); MAR, so never discuss non-public portfolio changes; only invite people in countries where the fund is registered; keep records.
- **U4. Event- or market-triggered creative.** Relevance: high, because market moves are exactly when advisers' clients call and selectors re-check sector exposures.
  - *Set-up:* define triggers in advance, for example:
    - Brent moving ±8% in a week;
    - a 10-year gilt or Bund move of 30bp or more;
    - a sector index falling 10% from its peak;
    - a major dividend-cut announcement;
    - a carbon-price shock.
  - *Creative:* pre-approve three to five variants per trigger, each with PM commentary and a pre-written explainer.
  - *Activation:* within 24 hours, either manually ("war-room" sign-off) or through LinkedIn API automation, running 5–10 days against account lists.
  - *Feasibility:* medium. Estimate £10–30k to set up, plus media per trigger.
  - *Risks:* no live performance figures; avoid market-timing implications and fear framing; keep the risk/benefit balance required by ESMA; consistent with fund documents.
- **U5. A personalised year-in-review for client firms ("Wrapped for fund buyers").** Relevance: medium-high for retention and memory among accounts that already engage.
  - *Content:* each December, a personalised digest for each engaged firm: meetings held, office-hours sessions and CPD hours completed, research the team used, and "the questions your team asked that shaped our 2026 content". An optional shareable card ("our team completed 12 CPD hours with X") is posted only if the firm chooses.
  - *Avoid:* personalised performance or dividend figures. These raise COBS 4.6 and accuracy issues, and platform nominee structures often hide which adviser firm holds the fund.
  - *Feasibility:* medium; it depends on CRM data quality. Estimate £10–30k.
  - *Risks:* GDPR transparency (engagement tracking must have been disclosed) and a "creepiness" test.
- **U6. Gamified, spaced-repetition CPD.** Relevance: medium-high, because UK advisers need 35 CPD hours a year (21 structured), the IDD requires 15 hours, and EFPA holders have their own CPD duties. Feasibility: high.
  - *Format:* eight questions over four weeks by email or app (Qstream-style), with a firm-versus-firm leaderboard (e.g., DFM teams) and a structured-CPD certificate on completion.
  - *Prizes:* charity donations only, never personal prizes (inducement risk).
  - *Evidence:* the Kerfoot randomised trials in medical education support the method.
  - *Cost:* £5–25k.
  - *Risks:* CPD-body standards; keep the fund out of the content.
- **U7. Personalised direct mail plus digital retargeting.** Relevance: high for Tier 1 and 2 accounts. Feasibility: high.
  - *Format:* print and post the flagship report (S1), personalised "for the [Firm] investment committee". Add a QR code to an account microsite, LinkedIn retargeting of the buying group and a salesperson call within seven days.
  - *Risks:* as for B5.
- **U8. A LinkedIn newsletter amplified with Thought Leader Ads.** Relevance: high. Feasibility: high. Cost: PM time plus about £2–10k a month in boosts.
  - *Format:* the PM, not the corporate page, writes a fortnightly newsletter in a distinctive voice with a recurring format (the Howard Marks model). Subscribers get email notifications. Boost the best issues as Thought Leader Ads to account lists.
  - *Risks:*
    - key-person dependency (the audience follows the PM), so co-author with a colleague and invite readers onto the firm's own email list;
    - each issue that mentions the fund is a financial promotion needing pre-approval (FG24/1, ESMA).
- **U9. A puzzle or ARG campaign for fund buyers.** Relevance: medium as a brand and distinctiveness play; the audience is analytical and December is a quiet, low-share-of-voice period.
  - *Format:* an annual "year-end puzzle" or cryptic themed on markets, energy and dividends. Trail it on LinkedIn and send a printed card to Tier 1 and 2 accounts. Publish a list of solvers with their permission, and donate to charity per solver.
  - *Feasibility:* high. Estimate £5–20k.
  - *Risks:* low compliance risk if there are no product claims and no valuable prizes; tone must not trivialise investing.
- **U10. Extra idea: a "manager-change response kit".** When a well-known manager leaves a competitor fund in the same sector (public news), many selectors must review that holding.
  - *Response:* have a due-diligence pack ready (P8), alert salespeople, and run a short burst to the sector's buyer universe.
  - *Never* name or disparage the competitor; keep comparative claims fair.
  - *Feasibility:* high.
- **U11. Extra idea: multilingual versions** (DE, FR, IT, ES) of the tool, newsletter digest and CPD for continental selectors. Boutiques rarely do this, so it could stand out. Cost is translation plus per-country compliance review; only use it where the fund is registered (UCITS notification, or national private-placement rules for UK OEICs, which count as AIFs in the EU after Brexit).

### Gaps
- Not verified this session: concrete examples of asset managers running Wrapped-style year-in-review, ad-bookable PM office hours, or market-triggered creative for professional audiences; and finance-industry puzzles aimed at clients rather than recruits. The ideas are judged on mechanism, not documented results.
- Data-licensing costs for screeners (FactSet, LSEG, Bloomberg, MSCI/FTSE redistribution) are unknown.
- Unverified: whether LinkedIn Thought Leader Ads can boost newsletters or articles (as opposed to posts) in late 2026, and whether LinkedIn gives newsletter authors subscriber email addresses (believed not).
- Regulatory questions for the compliance researcher: whether the MiFID issuer-paid-research exemption can apply to research commissioned by a UCITS ManCo; MAR investment-recommendation exposure for stock-level screeners; and real-time promotion rules for office hours.

## 5. Behavioural science and effectiveness: brand-building versus activation, mental availability and category entry points, and staying front of mind for the fund-review cycle

### Takeaway
B2B effectiveness research points the same way from several directions:
- split investment roughly 46:54 between brand-building and activation;
- reach the whole category of potential buyers, not just those in market;
- use emotion, personal value and distinctive assets;
- tie the brand to a few category entry points (CEPs) so it comes to mind in buying situations;
- make buying easy ("physical availability").

For fund buyers, "front of mind at review time" means four things:
- a continuous, low-weight, distinctive presence across the whole account universe;
- consistent links to two or three fund-buyer CEPs;
- activation bursts timed to scheduled review windows and to trigger events;
- frictionless due diligence.

Progress should be measured with a small fund-buyer brand tracker and leading indicators, not only leads.

### Cited Findings
- [H] Les Binet and Peter Field's *The Long and the Short of It* (IPA, 2013) shows brand-building (long-term, emotional, broad reach) and sales activation (short-term, rational, targeted) work differently. Activation effects decay quickly while brand effects compound, and the B2C optimum split is about 60:40. — [IPA](https://ipa.co.uk/)
- [H] For B2B, Binet and Field (2019, with the LinkedIn B2B Institute) put the optimum at about 46:54 brand:activation. [M] They also found B2B brand effects take longer to show, given longer purchase cycles, and that emotional and fame-driven campaigns outperform the rational, feature-led approach most B2B marketers default to. — [LinkedIn B2B Institute](https://business.linkedin.com/marketing-solutions/b2b-institute)
- [H] Byron Sharp's *How Brands Grow* (Ehrenberg-Bass, 2010) argues brands grow mainly through penetration, i.e., more buyers. That depends on mental availability (being thought of in buying situations) and physical availability (being easy to find and buy). The book recommends continuous presence over sporadic bursts and documents the "double jeopardy" law. — [Ehrenberg-Bass Institute](https://marketingscience.info/)
- [H] Jenni Romaniuk (*How Brands Grow Part 2*, 2015, with Sharp; *Better Brand Health*, 2022) defines category entry points as the needs, occasions and situations that cue buyers' memories at the moment of choice. Mental availability is measured by how many CEPs a brand is linked to, relative to competitors. — [Ehrenberg-Bass Institute](https://marketingscience.info/)
- [H] The 95:5 rule (Dawes, 2021): only about 5% of B2B buyers are in market in a given quarter, so most advertising must build memories for later rather than harvest demand now. — [LinkedIn B2B Institute, "The 95-5 Rule"](https://business.linkedin.com/marketing-solutions/b2b-institute/b2b-research/trends/95-5-rule)
- [M] The LinkedIn B2B Institute and Ehrenberg-Bass published guidance (around 2021–22) on applying CEPs and mental availability to B2B. It recommends researching buying situations rather than personas and building distinctive assets. — [LinkedIn B2B Institute](https://business.linkedin.com/marketing-solutions/b2b-institute)
- [M] The B2B Effectiveness Code (2023), from the LinkedIn B2B Institute with Cannes Lions and WARC, is a framework for classifying B2B creative effectiveness by the type of effect achieved. — [Cannes Lions](https://www.canneslions.com/); [WARC](https://www.warc.com/)
- [M] Tversky and Kahneman's "availability heuristic" (1973) holds that people judge likelihood and relevance by how easily examples come to mind. It is the cognitive basis of mental availability for time-pressed fund selectors. — [Tversky & Kahneman (1973), *Cognitive Psychology*](https://doi.org/10.1016/0010-0285(73)90033-9)
- [M] Personal value (career safety, confidence) weighs about twice as heavily as business value in B2B purchase intent (CEB/Google, 2013). B2B buyers also spend only about 17% of buying time with suppliers (Gartner). Most of a fund buyer's impression is therefore formed without the salesperson present. — [Think with Google](https://www.thinkwithgoogle.com/); [Gartner](https://www.gartner.com/en/sales/insights/b2b-buying-journey)
- [H] Fund buyers face scheduled, regulator-driven review moments:
  - UK authorised fund managers' annual Assessments of Value (COLL 6.6.20R);
  - Consumer Duty fair-value assessments by manufacturers and distributors (PRIN 2A);
  - periodic product-governance reviews by distributors under the FCA PROD sourcebook and the MiFID II product-governance rules.
  These are predictable windows when fund buyers come into market. — [FCA Handbook, COLL 6.6](https://www.handbook.fca.org.uk/handbook/COLL/6/6.html); [FCA Consumer Duty](https://www.fca.org.uk/firms/consumer-duty); [FCA Handbook, PROD](https://www.handbook.fca.org.uk/handbook/PROD/)

### Inferences
- **Define the category and all its buyers first.** Examples: "global equity income for UK DFM/MPS teams and adviser investment propositions", or "energy and transition equities for European bank selectors". List every potential buying firm (Section 1, P1; Section 2, B1) and plan to reach all of them every quarter, not just those that look "in market".
- **Make the split explicit.** For a boutique, a workable starting point is about 40–50% of non-staff marketing spend on memory-building (always-on distinctive content and ads to the whole universe) and 50–60% on activation (triggered campaigns, office hours, CPD, due-diligence packs, sales enablement). Long holding periods and rare switching argue against a pure lead-generation programme. The split should then be tuned with tracking data.
- **Use a fund-buyer CEP map.** These are hypotheses to validate with 15–20 interviews or a short survey before committing creative:
  - "when I need more portfolio income without adding duration or credit risk";
  - "when a client in decumulation wants rising income";
  - "when an income fund on our list cuts its dividend or loses its manager";
  - "when clients ask about oil, energy prices or the energy transition";
  - "when we rebalance after a sector sell-off";
  - "when we need diversification away from concentrated US mega-cap exposure";
  - "when we want transition exposure that still pays dividends";
  - "Assessment-of-Value or fair-value review season".
  Own two or three CEPs and repeat the same phrasing and assets everywhere: ads, factsheets, decks, mailers, the PM newsletter.
- **Distinctive assets:** choose one or two (a colour plus a chart style, a named index, a recurring PM format) and keep them for years. Fund marketing's visual sameness makes this cheap differentiation.
- **Physical availability for funds** means being on platforms and buy lists, risk-profiled (e.g., Dynamic Planner), on Allfunds, rated where possible, with complete EMT/EPT/EET data and due diligence that can be done in days (P8). It is the "ease of buying" half of the Ehrenberg-Bass model and usually under-marketed.
- **Continuity and timing:**
  - Keep always-on at low weight, e.g., roughly 1–3 LinkedIn exposures a week per targeted member (estimate), with creative variety inside fixed assets.
  - Add bursts around quarter-ends (MPS rebalances), the months when Assessments of Value are published and fair-value reviews happen, each account's known buy-list review month (Section 3, S3) and trigger events (Section 4, U4 and U10).
- **Emotion and personal value:** speak to the selector's career and investment-committee stakes. Examples: "evidence your committee will accept", "the fund you won't have to explain away in a drawdown", "make your fair-value review easier". All must remain fair, clear, not misleading and balanced.
- **Measurement for a small audience:**
  - An annual or semi-annual fund-buyer brand tracker of 100–200 respondents (estimate £15–40k) covering unprompted and prompted awareness, which managers come to mind for each CEP, and consideration.
  - Leading indicators: the share of the account universe reached, share of branded search, newsletter subscribers from target accounts, due-diligence and DDQ requests, meeting acceptance rates, buy-list additions, and platform or Allfunds flow and engagement data.
  - Judge over 12–24 months, not by campaign.

### Gaps
- No effectiveness study specific to B2B fund marketing (brand versus activation in asset-management distribution) was found or could be searched. Whether IPA Databank has relevant asset-management B2B cases is unknown.
- Binet and Field's *Effectiveness in Context* (IPA, 2018) gives category-specific splits, but the financial-services figures could not be recalled reliably, so none are given.
- Fund-buyer CEPs, buy-list holding periods and review frequencies across UK and continental segments have not been researched and need primary research.
- Claims that most B2B ads score poorly on emotional response (e.g., System1 testing with the B2B Institute) could not be verified and are excluded.
