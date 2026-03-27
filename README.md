# Object Rearrangement Under Geometric and Commonsense Constraints

## Added my google doc links, originally sent to my FYP advisor for update
- Google doc one: https://docs.google.com/document/d/1vQ6TnDqs57LIIg0wrAfPz3NKcF2j7TZjyt1pOM3lEwk/edit?usp=sharing
- Google doc two: https://docs.google.com/document/d/1bNGfMg2cU19ufobZZW97ff-PVwAQd5qv/edit?usp=sharing&ouid=106964031147266588184&rtpof=true&sd=true
- Dear visitors to this page, would appreciate your valuable comments if any.
```
## citation for google doc1
@misc{2023LitResearchRobo,
  author = {Zhu, Tianqi},
  title = {Literature research and discussion on robot reasoning with foundation models, NUS CP4101 update doc},
  year = {2023},
  url = {https://docs.google.com/document/d/1vQ6TnDqs57LIIg0wrAfPz3NKcF2j7TZjyt1pOM3lEwk/edit?usp=sharing},
  note = {Google Doc with link on Github}
}
## citation for google doc2
@misc{2024ObjectRearrangement,
  author = {Zhu, Tianqi},
  title = {Object rearrangement under geometric and commonsense constraints, NUS CP4101 update doc},
  year = {2024},
  url = {https://docs.google.com/document/d/1vQ6TnDqs57LIIg0wrAfPz3NKcF2j7TZjyt1pOM3lEwk/edit?usp=sharing](https://docs.google.com/document/d/1bNGfMg2cU19ufobZZW97ff-PVwAQd5qv/edit?usp=sharing&ouid=106964031147266588184&rtpof=true&sd=true},
  note = {Google Doc with link on Github}
}
```

## Added the data submitted together with my FYP final report on May 7th, 2024
- [result_llm.zip](https://github.com/Tianqi-Zhu/Object_Rearrangement_FYP_Report/blob/main/Result_llm.zip)

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
## Update on Jan 6th, 2026 
added report **"Data-Efficient User Preference Acquisition for Shelf Rearrangement via Vision-Language Analysis and Interactive Ranking"** [here](Zhu_data_efficient_user_preference_acquisition.pdf)

Abstract:
Personalized object arrangement in domestic environments requires understanding subjective user preferences that are often implicit
and difficult to articulate. Existing approaches typically rely on user-generated demonstrations or curated datasets, which are costly
to collect and do not scale well to real-world deployment. We present a data-efficient, human-centered pipeline for adapting shelf
rearrangement models to individual users by learning preferences through natural interactions. The system acquires preference signals
from user-provided reference photos and interactive ranking of shelf images, and uses a vision–language model to infer interpretable
arrangement patterns such as spacing, grouping, and spatial bias. User preferences are represented as weighted, composable constraints
that guide generative arrangement models. To improve adaptation efficiency over time, the system leverages a growing cross-user
preference database to refine which examples are presented to new users and to warm-start preference inference. In addition, the
pipeline supports adaptive discovery of new arrangement patterns when existing categories fail to explain user behavior. Together,
these components enable transparent, scalable, and low-effort personalization of object arrangement goals suitable for deployment in
household robotic and assistive systems.

```
@misc{zhu_preference_acquisition,
  title        = {Data-Efficient User Preference Acquisition for Shelf Rearrangement via Vision--Language Analysis and Interactive Ranking},
  author       = {Zhu, Tianqi},
  year         = {2026},
  howpublished = {\url{https://github.com/Tianqi-Zhu/Object_Rearrangement_FYP_Report/Zhu_data_efficient_user_preference_acquisition.pdf}},
  note         = {GitHub repository, Accessed: 2026-01-06}
}
```
<figure>
<img src="robo_and_shelf.jpeg" alt="shelf arranging robot likes beautiful shelf" width="40%">
<figcaption><em>Shelf arranging robots love beautiful shelves!</em></figcaption>
</figure>

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

## Useful Related Work
- [Compositional Diffusion-Based Continuous Constraint Solvers (CoRL 2023)](https://diffusion-ccsp.github.io/)
- [Energy-based Models are Zero-Shot Planners for Compositional Scene Rearrangement (RSS 2023)](https://rss2023.github.io/rss2023-website/program/papers/030/)
- [MyHouse, MyRules: Learning Tidying Preferences with Graph Neural Networks (CoRL 2021)](https://proceedings.mlr.press/v164/kapelyukh22a/kapelyukh22a.pdf)
- [TarGF: Learning Target Gradient Field to Rearrange Objects without Explicit Goal Specification (NeurIPS 2022)](https://proceedings.neurips.cc/paper_files/paper/2022/hash/cf5a019ae9c11b4be88213ce3f85d85c-Abstract-Conference.html)
- [LEGO-Net: Learning Regular Rearrangements of Objects in Rooms (CVPR 2023)](https://openaccess.thecvf.com/content/CVPR2023/html/Wei_LEGO-Net_Learning_Regular_Rearrangements_of_Objects_in_Rooms_CVPR_2023_paper.html)
