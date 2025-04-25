Reviewer Comments:

Reviewer 1
My comments for this modelling paper by Laws et al. is as follows:
1.      The first and foremost query is that there are now multiple RCTs of MSU vs standard care with consistent numbers of the effect of MSU-facilitated early thrombolysis (BEST-MSU Grotta et al.; B_PROUD Ebinger et al.; Turc et al. meta-analysis), earlier thrombolysis prior to MT (BEST-MSU substudy Czap et al.) and MT time savings (Czap et al. 2019; Zhao et al.; Helwig et al.). Most of these were done in a metropolitan setting but I would guess these would broadly still apply to most regions in England. Therefore, I understand modelling the geography of potential MSU locations, but I don’t quite understand the need to use synthesized data for outcomes when real-world data exists for model incorporation? There is quite a discrepancy which definitely needs some further discussion – perhaps my further comments can tease these out a bit.

Response: Thank you for the question. Using modelled (predicted) outcomes based on time to IVT and MT is necessary for three reasons: 1) As we are exploring the impact of the MSUs outside of metropolitan areas response times for the MSU may be significantly longer than in the trials in metropolitan areas (though this may be compensated for by the ability to direct suitable patients directly to a MT-capable centre). 2) We are interested not only in overall benefit, but how that benefit will likely change with geography - to help better understand where MSUs will or will not have most benefit (based on changing times for both IVT and MT). 3) We wish to predict a full mRS profile in order to estimate Utility scores with different treatment options (this is covered in a separate health economics paper). These questions need modelling to answer. we have added a section at the very start of the discussion on this the discussion on this.


2.      Clearly the way that the outcomes are modelled are pivotal to the results and conclusion. Unfortunately, the rationale and basics behind the model are not well described in the manuscript. There is more information in the github link but this is mainly focused on coding and not readily readable by clinician-researchers (and could be deleted or not accessible at a future stage). I would suggest the manuscript body really needs a concise summary of the modelling with key rationales (eg, choosing datasets to decide outcomes) and the rest of modelling can go in a supplemental file that is readable for clinician-researchers.

Response: We have now added a substantial appendix to the paper. We have also put more of an introduction to the outcome modelling in the main paper.


3.      From my current understanding of the modelling, some key comments and questions about outcomes:

a.      I do not understand the population that the authors are trying to model MSUs in. If I am not mistaken it looks like they are trying to model benefit in all hospital-diagnosed strokes in England rather than specifically a “treatment-eligible” population? If I am mistaken, how have they modelled such a treatment-eligible population? If the former, then any MSU-derived benefit for reperfusion therapy would be highly diluted across all stroke patients.

We have modelled the treatment-eligible population. This has been made more clear in the methods. We base the mix of nLVO and LVO (when estimating an overall clinical benefit) on the mix of nLVO and LVO on those currently arriving at hopsital within 4 hours of stroke onset as this population should be similar to the population where a MSU is dispatched.


b.      Assuming linear logs-odd of the IVT time-outcome curve is controversial – do the authors have any validation of this? Most other modelling in stroke (eg, Holodinsky et al. (2018) JAMA Neur) use the Emberson et al. curve directly.


I am happy to confirm that we do use the Emberson 'curve', and we use the same type of modelling as Holodinsky. The Emberson 'curve' of decay in odds of good outcomes becomes linear when the odds ratios are logged (as that was the basis of their logistic model). The supplement now shows the effects over time on mRS scores and in figure S2 it shows how the the good outcomes due to IVT or IMT decline in a non-linear fashion - with the decline being faster in the early time after stroke onset.

c.      Following from the previous point, I do not get a sense where along the Emberson et al. curve that they are modelling the MSU benefit. The main benefit of MSUs is time saving to push patients into the <60 and <90 min onset-to-needle time epochs – see B_PROUD trial (Ebinger et al.) supplementary table 4. This implies that MSUs are probably saving time at the steep part of the IVT curve where the same time saving is probably more valuable than at other time epochs. The importance of this is profound – if you look at Mackey et al. (2023) the outcomes deterioration drop steeply within the first 60 mins of onset and the rest of the time epochs flatten shortly after. This would also argue against a linear logs-odd assumption. Hence I would be very interested to know how the authors have handled this in the model, particularly if they have modelled a significant increase in the “golden hour” (<60 min onset) thrombolysis seen by MSUs worldwide (around 11-fold increase as per Turc et al. meta-analysis).

Response: We agree! As above, by using the log-odds (which is linear in both Emberson and Holodinsky) that will indeed lead to a greater decline in odds of a good outcome in the early period. This effect is built in to the model by using a linear decline in log-odds rather than a linear decline in odds. 


d.      It looks to me that the authors are modelling the effect of IVT in the study-defined populations of LVO and non-LVO separately but I am unsure why this is? The meta-analyses of IVT trials clearly were before the MT era so the overall benefit is a composite of both LVO and non-LVO. As demonstrated by BEST-MSU substudy by Czap et al., there is just as much effect with IVT prior to MT patients as in the main BEST-MSU study. Again, most other analyses of this kind model IVT agnostic to LVO status and then add the additional effect of MT according to MT meta-analysis data (like Goyal et al.).


Response: The separation of nLVO and LVO IVT is a necessary step when considering the benefits of both IVT and MT, as the nLVO will only receive IVT, and the MT patients could receive IVT and/or MT. MSUs could change times to IVT and MT differently - for more rural areas IVT may be slowed (due to slower access by the MSU), but time to MT could be speeded (by direct transfer to a MT-capable unit). To understand the potentially complex effects across geography it is necessary to separate out nLVO and LVO and then their treatment options.

e.      I think the 30% LVO rate seems far too high. The authors worked out the total number of hospital-admitted strokes in England and then used a NIHSS dichotomization of 10-11 to determine likely LVO (they justify this through the PRESTO trial but the median NIHSS for LVO in this study was 13). If you look at the BEST-MSU sub-study (Czap et al.), just 19% of enrolled trial patients were LVO, and of these only 75% received EVT. The authors mention a rate of >30% in an early RACE validation study but this was an enriched dataset from Catalonia based on hospital-admitted strokes. I therefore suspect 10-15% LVO rate in a population of hospital-confirmed strokes is more realistic.

Response: There are certainly different possible estimates. A systematic review puts the range at LVO's accounting for approximately 24% to 46% of acute ischemic strokes (https://pmc.ncbi.nlm.nih.gov/articles/PMC6584910/). Our figure is based on arrivals within 4 hours of stroke onset, but seems to be very much within the range reported, using different methods, in systematic review. But as we separate our results for nLVO and LVO, this should allow people to look at our results and see how that would apply with different views of that mix.

Rennert RC, Wali AR, Steinberg JA, Santiago-Dieppa DR, Olson SE, Pannell JS, Khalessi AA. Epidemiology, Natural History, and Clinical Presentation of Large Vessel Ischemic Stroke. Neurosurgery. 2019 Jul 1;85(suppl_1):S4-S8. doi: 10.1093/neuros/nyz042. PMID: 31197329; PMCID: PMC6584910.




f.      Why did the authors choose to model 6-month mRS rather than 3-month mRS? The derivative data from their modelling such as Emberson et al. and Lees et al. are all at 3 months.

This has been corrected this is now set at 3-6 months to reflect Emberson (306 months) and Fransen (3 months). 

g.      I do not understand why the authors have modelled excess mortality on the github attributable to reperfusion therapy when the real-world data has not shown this exists?

Response: Our language was not good! We have adjusted the language. Rather than 'excess' mortality - it is now 'treatment-related mortality' and is the reported or derived risk of treatment-related mortality (e.g. by IVT-induced haemorrhage). This is a fixed quantity that applies across all times of treatment (and adjusts the overall mortality to that seen in the clinical trials). For most patients this will be overcome by the benefit of the treatment.

h.      The authors model no effect for IVT after 6.3 hours according to Emberson et al. curve but the accepted treatment window is <4.5h without CT-perfusion.

Response: The estimate from Emberson is that there is no response at 6.3 hours. 4.5 hours is the statistical cut-off which depends on both estimated time of no effect and the uncertainty around treatment effect size. For modelling we want to use the best estimate of no-effect time (6.3 hours from Emberson), but in clinical practice people want to know the time when you are 'sure' there is still an effect which includes allowance for sampling errors ihn the trials.

i.      Similarly the authors model no effect for MT after 8 hours but there are trials that show benefit of MT up to 24h without CT-perfusion (eg, MR CLEAN LATE trial).

Response: : We are*modelling the average effect decline as reported in the meta-analyses. There will no doubt be some patients who can still benefit, as there are patients who lose benefit faster. But in a recent observational study we found that in real-world data the average beneficial effect of thrombectomy reduced to zero by about 7 hours (see page 35 of https://zenodo.org/records/13310710)  

4.      A number of comments regarding the Introduction:

a.      The authors mention the Fatima et al. and Chen et al. meta-analyses of MSU but seem to have excluded Turc et al. which is the most rigorous meta-analysis of MSU efficacy to date – main findings here are of 31 mins median difference MSU vs standard ambulances and improved 90-day mRS of aOR 1.64, in addition to higher thrombolysis and 11-fold increase in “golden hour” thrombolysis.

Response: Thank you - that's very useful to include in the introduction, which we've now done.


b.      The authors write “In order to predict the benefit of MSUs in a broader geographic area Holodinsky et al. [14] used modelling to predict the benefit from IVT as the proportion of patients with an outcome of mRS 0-2 when using MSUs to cover larger distances (up to 4.5 hours travel for the MSU)” – I think this has been written in a somewhat misleading way. This paper modelled the specific situation of suspected large vessel occlusion patients coming directly to an EVT center through use of a severity-based triage tool (eg, LAMS) versus MSU, rather than modelling MSU-facilitated IVT in general. The modelling relies on the assumption that time to MT is the predominant driver of efficacy and the additional effect of MSU is by earlier bridging IVT prior to MT. For fairness, there is contrary data the Czap et al. paper which the authors mention briefly but do not the report the main finding of significantly improved 90-day outcomes (OR 2.6). There is also a RCT from Germany Helwig et al. comparing MSU vs LAMS triage showing significant improved triage accuracy with MSU.

Response: Thanks you. We certainly do not intend to be misleading - we're trying to show the potential benefit of MSUs can come from either earlier on-scene IVT or better direction to MT-centres. But we have adjusted the intro to modify our wording and include these points (including being clearer about Jess Holodinky's paper). We now also reference the full czap paper and the improved outcomes. We now also cite the Helwig article.


References:
Czap, A. L., Alexandrov, A. W., Nour, M., Yamal, J. M., Wang, M. X., Jacob, A. P., . . . Grotta, J. C. (2024). Impact of Mobile Stroke Units on Patients With Large Vessel Occlusion Acute Ischemic Stroke: A Prespecified BEST-MSU Substudy. Stroke-Vascular and Interventional Neurology, 4(1). doi:ARTN e001095 10.1161/SVIN.123.001095
Czap, A. L., Grotta, J. C., Parker, S. A., Yamal, J. M., Bowry, R., Sheth, S. A., . . . Jagolino-Cole, A. L. (2019). Emergency Department Door-to-Puncture Time Since 2014. Stroke, 50(7), 1774-1780. doi:10.1161/STROKEAHA.119.025106
Grotta, J. C., Yamal, J. M., Parker, S. A., Rajan, S. S., Gonzales, N. R., Jones, W. J., . . . Bowry, R. (2021). Prospective, Multicenter, Controlled Trial of Mobile Stroke Units. N Engl J Med, 385(11), 971-981. doi:10.1056/NEJMoa2103879
Helwig, S. A., Ragoschke-Schumm, A., Schwindling, L., Kettner, M., Roumia, S., Kulikovski, J., . . . Fassbender, K. (2019). Prehospital Stroke Management Optimized by Use of Clinical Scoring vs Mobile Stroke Unit for Triage of Patients With Stroke: A Randomized Clinical Trial. JAMA neurology, 76(12), 1484-1492. doi:10.1001/jamaneurol.2019.2829
Holodinsky, J. K., Williamson, T. S., Demchuk, A. M., Zhao, H., Zhu, L., Francis, M. J., . . . Kamal, N. (2018). Modeling Stroke Patient Transport for All Patients With Suspected Large-Vessel Occlusion. JAMA Neurol, 75(12), 1477-1486. doi:10.1001/jamaneurol.2018.2424
Turc, G., Hadziahmetovic, M., Walter, S., Churilov, L., Larsen, K., Grotta, J. C., . . . Audebert, H. J. (2022). Comparison of Mobile Stroke Unit With Usual Care for Acute Ischemic Stroke Management: A Systematic Review and Meta-analysis. JAMA Neurol, 79(3), 281-290. doi:10.1001/jamaneurol.2021.5321
Zhao, H., Coote, S., Easton, D., Langenberg, F., Stephenson, M., Smith, K., . . . Davis, S. M. (2020). Melbourne Mobile Stroke Unit and Reperfusion Therapy: Greater Clinical Impact of Thrombectomy Than Thrombolysis. Stroke, 51(3), 922-930. doi:10.1161/STROKEAHA.119.027843


Reviewer 2
Thank you for the opportunity to review this very interesting paper on modelling MSU use in England.  The paper generally reads well and adds significantly to current evidence base.
My main comments are in order of reading and grouped into more major and minor issues:

More major:
(1)     The use of NIHSS to determine LVO status is indirect and a limitation that needs to be mentioned in the discussion.  There are other studies assessing % LVOs in hospital admissions series based on imaging and it would be useful to cross reference one of these in addition to the RACE pre-hospital prediction of LVO, which is also indirect.

Response: There are certainly different possible estimates. A systematic review puts the range at LVO's accounting for approximately 24% to 46% of acute ischemic strokes (https://pmc.ncbi.nlm.nih.gov/articles/PMC6584910/). Our figure is based on arrivals within 4 hours of stroke onset, but seems to be very much within the range reported, using different methods, in systematic review. But as we separate our results for nLVO and LVO, this should allow people to look at our results and see how that would apply with different views of that mix. We have added uncertatinty about the mix of nLVO and LVO to the discussion.

(2)     My understanding is that CTA in MSUs can be quite tricky – is this routinely part of MSUs? Please comment on this earlier and more extensively than in current discussion.

Response: Thank you. We have bolstered the discussion on this point to reflect that CT-A has not always been used in MSU care, but is increasingly being adopted to improve MT workflows.


(3)     Why were perfusion imaging selected candidates excluded?  This is fairly standard practice now.  Please justify under methods going beyond the current brief mention in the discussion.

Reponse - Thank we have added more to the discussion. We currently don't have sufficient clinical trial data to confidently model how MSUs miught affect this group, where onset-to-treatment times are not strongly linked to outcomes

(4)     The time frames for transfer related ‘net MT delays’ are listed as 30, 60, 90.  Are these based on existing registry data?  We certainly have some small hospitals that can take a lot longer than 90 minutes for ‘door in door out time.’  Can you add somewhere where these times frames came from?  Really quite relevant to all time frame estimates.  Apologies if I overlooked this if already mentioned.

Response: We have added to the discussion. In a stroke registry Froehler reported that transfer-related delays were on average 75 minutes + travel time. We have explored the range 30-90 minutes + travel time. This was also agreed in co-production workshops involving representation from stroke consultants, ambulance staff and patients and public. We are likely biasing this investigation to assuming that transfer-related delays would more likely improve rather than worsen as MT becomes more established. But we acknowledge that in some instances delays could be longer, which we have added to the discussion.

(5)     Discussion: in the para on clinician propensity to treat – this could also be mimicked by equipping regional hospitals with telestroke services and it would be worth mentioning this as another usual care service improvement opportunity. If telestroke already in place throughout England then the argument that MSU clinicians are more motivated would be less convincing.


Response: Yes, that certainly is alternative and has been added to the dicussion, along with other possible methods to improve pre-hopsital care,



(6)     I think you could spend a bit more time on hybrid models in the discussion. You very briefly mention stroke scales and telemedicine stating evidence of patient benefit is limited.  However, as far as I am aware, there is also no data showing that MSU triage for bypass improves patient outcome, certainly not in remote areas.  Therefore, I feel that paramedic stroke scales and especially telemedicine (aka ‘mini-MSU’) deserve more emphasis in the discussion. This is especially important given your observation that for patients further from CSC the LVO bypass appears to be the main driver of MSU benefit which really comes down to LVO diagnosis or rather predicting MT intervention, which can be quite reliably achieved via telemedicine as shown in studies such as Scot et al https://eur03.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.neurology.org%2Fdoi%2F10.1212%2FWNL.0000000000201104&data=05%7C02%7Cm.allen%40exeter.ac.uk%7C2a50295ac0c74945add908dd5ae30db9%7C912a5d77fb984eeeaf321334d8f04a53%7C0%7C0%7C638766653406450171%7CUnknown%7CTWFpbGZsb3d8eyJFbXB0eU1hcGkiOnRydWUsIlYiOiIwLjAuMDAwMCIsIlAiOiJXaW4zMiIsIkFOIjoiTWFpbCIsIldUIjoyfQ%3D%3D%7C0%7C%7C%7C&sdata=p6sCYwWhrcxiWuKg1uSI3wb1OVEMksxNLNg1bKwz9ZI%3D&reserved=0.

Response - that has now been strenghtened in the discussion - especially your point that these other systems may offer particular advantage for people further away from a MSU base. Your point of the potential advantage of a hybrid system is well-taken.

Minor:
(1)     The manuscript is quite long and I wondered if some sections could be shortened and streamlined.

Response: It is quite long - we have moved some methods to what is now a much more extensive appendix on methodology.

(2)     Please define  Lower Super Output areas briefly in the abstract e.g. (~1500 people)

Response - have done (in the methods)

(3)     The writing is unclear in a few places.  I list some examples below from abstract and introduction, but suggest you carefully review the entire manuscript once more:
(a) First sentence in abstract is missing a word. Third sentence is difficult to follow.  Can this be split into two or at least the order? E.g. MSUs are XYZ and have been proposed as away…
(b)     Second to last sentence repeated use of the word ‘more.’
(c)     Introduction first sentence second paragraph the first comma should be replaced by an ‘and.’ Last sentence that paragraph I’d move the ‘only’ before ‘suitable.’  Introduction 5th paragraph second sentence there is an ‘in’ missing before ‘the proportion.’

Thank you for those points. They are corrected and we will read through again.


(4)     I am not 100% sure about Figures 3 and 4.  These are very busy.  Could this information be presented instead in the form of a table or forest plot? Might be easier to read as well allowing larger fonts which are currently quite small.  Just a suggestion.

Response - thank you. It is a lot of information, but we feel grouping it by variable hopefully is easier than combining everything in a Forest Plot.
