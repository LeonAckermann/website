@article{ackermann-ohmer-2024-relationship,
    title = "On the Relationship between Skill Neurons and Robustness in Prompt Tuning",
    author = "Ackermann, Leon  and
      Ohmer, Xenia Isabel",
    editor = "Calzolari, Nicoletta  and
      Kan, Min-Yen  and
      Hoste, Veronique  and
      Lenci, Alessandro  and
      Sakti, Sakriani  and
      Xue, Nianwen",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italia",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.1086/",
    pages = "12403--12415",
    abstract = "Prompt Tuning is a popular parameter-efficient finetuning method for pre-trained large language models (PLMs). Based on experiments with RoBERTa, it has been suggested that Prompt Tuning activates specific neurons in the transformer{'}s feed-forward networks, that are highly predictive and selective for the given task. In this paper, we study the robustness of Prompt Tuning in relation to these ``skill neurons'', using RoBERTa and T5. We show that prompts tuned for a specific task are transferable to tasks of the same type but are not very robust to adversarial data. While prompts tuned for RoBERTa yield below-chance performance on adversarial data, prompts tuned for T5 are slightly more robust and retain above-chance performance in two out of three cases. At the same time, we replicate the finding that skill neurons exist in RoBERTa and further show that skill neurons also exist in T5. Interestingly, the skill neurons of T5 determined on non-adversarial data are also among the most predictive neurons on the adversarial data, which is not the case for RoBERTa. We conclude that higher adversarial robustness may be related to a model{'}s ability to consistently activate the relevant skill neurons on adversarial data."
}