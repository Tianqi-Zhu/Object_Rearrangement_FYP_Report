# Object Rearrangement Under Geometric and Commonsense Constraints

## Update on Jan 4th, 2026
added report **"Data-Efficient Preference-Aligned Robotic Shelf Arrangement with Composable Constraint Models"** [here](Zhu_data_efficient_preference_aligned_shelf_arrangement.pdf)

Abstract:
 We study the problem of data-efficient object arrangement on shelves with existing objects, where a robot must propose geometrically feasible and semantically aligned goal configurations for newly introduced items while optionally rearranging existing ones. The task is inherently hierarchical: decisions must be made at the level of shelf layers and compartments before resolving precise local object poses. We propose a unified framework that combines (i) a hierarchical generative model that samples geometrically and physically valid shelf configurations, (ii) composable diffusion or energy-based guidance to enforce constraints and minimize rearrangement effort, and (iii) a semantic alignment module driven by large language models (LLMs) and preference diffusion to capture user habits and commonsense organization principles. Semantic alignment is formalized through a semantic projection and distance defined over configurations, enabling reward-like gradient guidance without requiring dense scalar rewards. We further introduce a continual preference learning mechanism that adapts to evolving user feedback while retaining stability via replay and regularization. Our formulation explicitly accounts for compartment capacity, rearrangement feasibility, and minimal-disruption objective when assigning new objects to shelf compartments. We outline a data generation pipeline and training strategy that leverage synthetic sampling, weak supervision from LLMs, and limited human feedback, achieving strong generalization with minimal data. The proposed approach unifies hierarchical planning, generative modeling, and preference-based learning, offering a scalable and flexible solution for personalized robotic shelf organization.

citation for the updated report:
```
@misc{zhu_preference_arrangement,
  title        = {Data-Efficient Preference-Aligned Robotic Shelf Arrangement with Composable Constraint Models},
  author       = {Zhu, Tianqi},
  year         = {2026},
  howpublished = {\url{https://github.com/Tianqi-Zhu/Object_Rearrangement_FYP_Report/Zhu_data_efficient_preference_aligned_shelf_arrangement.pdf}},
  note         = {GitHub repository, Accessed: 2026-01-04}
}
```
<figure>
<img src="robo_and_shelf.jpeg" alt="shelf arranging robot likes beautiful shelf" width="40%">
<figcaption><em>Shelf arranging robots love beautiful shelves!</em></figcaption>
</figure>

## Update on Jan 6th, 2026 
added report **"Data-Efficient User Preference Acquisition for Shelf Rearrangement via Vision--Language Analysis and Interactive Ranking"** [here](Zhu_data_efficient_user_preference_acquisition.pdf)

Abstract:
Deploying shelf rearrangement models in real homes requires adapting to individual user preferences, yet obtaining such preference data is a major practical challenge.
Directly asking users to generate arrangement demonstrations is tedious and does not scale.
We propose a data-efficient preference acquisition framework that combines (i) analysis of user-provided reference photos using a vision--language model (VLM) and (ii) an interactive ranking interface based on pairwise comparisons and lightweight scoring.
User preferences are inferred as a set of interpretable arrangement patterns, which are then mapped to composable, constraint-specific diffusion models for arrangement goal generation.
This design minimizes user effort while enabling robust personalization and transparent preference modeling.

## Initial Upload of FYP Report
I opted for the self-proposed version of my undergraduate final year project (FYP) and I came up with the topic above almost entirely on my own. I am interested in continue doing research along this line or something relevant.

The main point of the project is to minimize human "hard" coding of various environment specifications etc for robots to place objects in a constrained physical structure, which enables the same system structure to be generalizable to new environments, conditions, with(out) variations on human related parameters.

I am looking for research assistant or PhD student positions. Please contact TianqiZhu at u dot nus dot edu if you have opportunity available.

I am also interested in server resources, robots etc, if i could borrow some from someone to use for a short period.

Thanks for reading. Have a nice day.

The reports contain several parts:
- interim report, on related work and formulation of porblem satisfying several constraints
- final report part one, pattern deduction
- final report part two, on testing VLM's ability for rearrangement goal proposal under geometric and physics constraints


