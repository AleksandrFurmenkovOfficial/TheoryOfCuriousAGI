# TheoryOfCuriousAGI

Knowledge Domain Expansion via Topology Transfer: A Mechanism for Hypothesis Induction or a Built-in Curiosity Mechanism

## A Mechanism for Hypothesis Induction or a Built-in Curiosity Mechanism

The Transformer architecture [1] was a step in the right direction and showed us glimpses of what is to come when achieving full-fledged AGI — an AI capable of all cognitive tasks available to humans.

The next step was the MoE architecture, where for optimization purposes, separate expert networks were extracted from the general weight array [2]. Initially, this step, although made for optimization, led us to a new paradigm — domain experts.

Incorrect architecture results in inefficient data utilization, hinders knowledge generalization, and prevents reaching AGI level and logical reasoning beyond the training data distribution.

To take the next step, I will begin with a problem statement, in which, as is usually the case, the solution is hidden.

## Problem Statement

Suppose we have a person who has been interested in botany since childhood — this is their knowledge domain. They had no books except books on botany, and studied it in isolation from other sciences. This person knows that plants exist, has a concept of a plant as a living organism, concepts of various plant genera, etc. In particular, they know that there are plants such as trees, know typical species, what they look like, where they grow, that there are different species with different needs and properties within certain geographical boundaries (even an isolated domain will inevitably carry redundancy and duplicate some information from potential other domains, such as the knowledge domain of "Geography"). What is important for our example: this botanist-person knows about the existence of parasitic plants that parasitize on trees. They understand the high-level concepts of this domain and the relationships between them, the topology of concepts, and are able to find a topological neighborhood for an arbitrarily given concept of this domain from the domain known to them.

At the same time, throughout their entire life, this person has never heard anything about the knowledge domain of "Biology."

However, if they are asked: "There is a living being — a horse, and it has no roots," — the person will immediately ask: "How does the horse feed?"

How did the person formulate this question? In the domain of botany, there is a connection between the concepts of a plant and feeding through roots.

The person can project the topology of concepts from the knowledge domain "Botany" from the concept "plant" through the parent meta-concept "life" onto the new concept "animal" based on their commonality through the parent concept "life."

Having made a topological projection from one concept to another, the person can begin cognition with the hypothesis that the projection result is most likely valid in the neighborhood of the new concept "animal," and can formulate tests to verify the quality of their projection — ask a question, the answer to which will fix the correctness of part of the projection or weaken it.

Having made a transfer from botany to biology, the person would assume how animals feed — through roots. A logical assumption if you have never seen animals. How would you continue learning about them after finding out there are no roots? First, you would weaken/cut off the concept of roots for an animal based on the interlocutor's answer or the result of observing them, but you would still need a concept implementing the need for nutrition for a living being. If animals are part of the concept "life," then they have nutrition, which means that based on input information, the topological place of roots must be replaced by another homologous concept as a supplier of nutrition. And you can search for this concept in the external world, ask questions, conduct experiments. And you will learn that in animals, the supplier of nutrition is the concept "mouth." You arrived at this by using projection from a known domain to a new concept through the common meta-concept "supplier of nutrition."

Moreover, our botanist can continue cognition by analogy. They will also be able to assume that the concept of parasitism exists in animals, just as it exists in the domain of botany. Simply by projecting topological connections from one domain onto a new entity from the new domain being studied — biology. And they can again conduct verification, confirming or refuting this hypothesis, strengthening or weakening it in the new domain of botany.

For this, the following will be needed:
- build knowledge domains (GWOT MoE [3]?);
- collect domain topology relative to the currently conceptualized concept;
- search for similar topologies in other domains, possibly discovering connections through meta-concepts/parent concepts (plant and animal are both concepts of life);
- fill gaps in some domains through projection from known domains, verifying projection results and either preserving or weakening the connection of the inherited projection;
- dynamically create new knowledge domains if new information generates a unique topology unlike anything known before (GWOT Dynamic MoE?).

As a result, we will obtain a universal model capable of rapid learning using a new type of native conceptual transfer learning.

## Mathematics as a Meta-Conceptual Domain

Of particular interest is the mechanism of mathematical concept formation through topological transfer. Mathematics in this paradigm is not a separate isolated domain, but a meta-conceptual superstructure arising from the generalization of repeating topological patterns across multiple concrete domains.

Consider the concept of "quantity." AI, interacting with different domains — counting apples in botany, sheep in animal husbandry, days in the calendar — discovers an invariant topological structure: discrete elements, the operation of set union, the property of commutativity in union. Projecting these repeating patterns into the meta-domain and cutting off context-dependent properties (apple color, sheep breed), the system derives the abstract concept of natural number and operations on it. Similarly, the concept of "continuous change," observed in plant growth, object movement, temperature change, when projected into the meta-domain, generates concepts of function, limit, derivative.

The key distinction of the mathematical meta-domain is the maximum degree of abstraction. It contains pure topological structures, purified of all concrete properties of the original domains. The system can use this meta-domain for instantaneous transfer of mathematical patterns to any new domain where isomorphic topology is discovered. Upon discovering a structure isomorphic to a group in an unfamiliar domain, the system immediately applies the entire apparatus of group theory without the need for retraining.

Thus, mathematical thinking emerges not as a separate ability, but as a natural consequence of the topology consolidation mechanism: discovery of common invariants, their abstraction, and formation of higher-order meta-concepts. This explains the "unreasonable effectiveness of mathematics" — it is effective because it is a distillation of fundamental topological invariants present in multiple concrete domains of reality.

## Knowledge Consolidation

However, even in humans, it often happens that their memory and thinking are fragmented. In one context, they build one chain of reasoning, in another context — another, mutually exclusive one. This is known as "a person says one thing, then another."

A conscious person can fight this only through reflection on their knowledge and thoughts. Why do I think/believe this way? Why in situation A do I think B, and in situation D do I think C? Where do I know this from? Are there contradictions here, am I unbiased in my conclusions?

They can identify contradictions and attempt to eliminate them. Bring their views to a common denominator, remove logical contradictions in their worldview, **consolidate the world model**. For this, there are two operations:

1. **Remove the personal perception component**, recorded in memory, from the final reasoning. "I love Democrats → what Democrats do carries a positive evaluation." However, in fact, there should be no positive evaluation in my logical reasoning, any evaluations should be given to arguments and consequences, not to the author's reputation, which can only be an initial criterion for quick evaluation without thinking. Democrats can also do bad things that should receive their negative evaluations without cognitive distortion due to personal predisposition toward them.

2. **Consolidate the fragmented world model**. It may turn out that in the process of cognition, domain fragments with identical topology were created. The task is to find such topologies and strengthen their connection with the general topology of the meta-model (model of meta concepts), consolidate domain topologies with it. Upon discovering irremovable contradictions, where domain topologies actually diverge due to factual differences between entities, the system should:
   - **and/or dynamically create a new (sub)domain or strengthen the divergence by linking it with the cause of divergence** (or a separate domain), fixing unique topological patterns;
   - **and/or adjust the meta-domain**, expanding its conceptual space to account for identified divergences and preserve common invariants.

Thus, an adaptive hierarchy of knowledge is achieved: domains specialize when necessary, and the meta-level evolves, maintaining consistency of the entire system of representations.

## Conclusion

A conceptual scheme for automatic native construction of a world model by an AI system is proposed, which is inherently curious, builds hypotheses based on the known, and subjects them to verification.

How to implement this in practice? I am convinced that we already have all the necessary computational power and almost all the architectural techniques to create such a system.

**GWOT Dynamic MoE + Recursive Latent Reasoning [4]?**

---

## References

[1] Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., Kaiser, Ł., & Polosukhin, I. (2017). Attention Is All You Need. *arXiv preprint arXiv:1706.03762*. https://arxiv.org/abs/1706.03762

[2] Dai, D., et al. (2024). DeepSeekMoE: Towards Ultimate Expert Specialization in Mixture-of-Experts Language Models. *arXiv preprint arXiv:2401.06066*. https://arxiv.org/abs/2401.06066

[3] Sasaki, M., Takeda, K., Abe, K., & Oizumi, M. (2025). Unsupervised alignment in neuroscience: Introducing a toolbox for Gromov-Wasserstein optimal transport. *Journal of Neuroscience Methods*, 419, 110443. https://doi.org/10.1016/j.jneumeth.2025.110443

[4] Jolicoeur-Martineau, A., et al. (2025). Less is More: Recursive Reasoning with Tiny Networks. *arXiv preprint arXiv:2510.04871*. https://arxiv.org/abs/2510.04871

[5] Kawakita, G., Zeleznikow-Johnston, A., Takeda, K., Tsuchiya, N., & Oizumi, M. (2024). Is my "red" your "red"?: Evaluating structural correspondences between color similarity judgments using unsupervised alignment. *Scientific Reports*, 14(1), 15917. https://doi.org/10.1038/s41598-024-65604-1

---

# Расширение доменов знаний через топологический трансфер

## Механизм индукции гипотез или встроенный механизм любопытства

Архитектура трансформера [1] была шагом в правильном направлении и показала нам проблески того, что грядёт при достижении полноценного AGI — AI, способного на все мыслительные задачи, которые доступны человеку.

Следующим шагом стала архитектура MoE, где с целью оптимизации выделили из общего массива весов отдельные сети экспертов [2]. Изначально этот шаг, хоть и был сделан ради оптимизации, привёл нас к новой парадигме — доменным экспертам.

Неправильная архитектура упирается в неэффективное использование данных, препятствует генерализации знаний и выходу на уровень AGI и логические рассуждения за распределением обучающих данных.

Чтобы сделать следующий шаг, я начну с постановки задачи, в которой, как это обычно и бывает, скрыто решение.

## Постановка задачи

Допустим, у нас есть человек, который с детства интересуется ботаникой — это его домен знаний. У него не было никаких книг, кроме книг по ботанике, и он изучил её изолированно от других наук. Этот человек знает, что существуют растения, у него есть концепт растения как живого организма, концепты различных родов растений и т. д. В частности, он знает, что есть такие растения как деревья, знает типовые виды, как они выглядят, где растут, что бывают разные виды с различными потребностями и свойствами в рамках определённых географических границ (даже изолированный домен так или иначе будет нести избыточность и дублировать часть информации из потенциальных иных доменов, как, например, домен знаний «География»). Что важно для нашего примера: этот человек-ботаник знает о существовании растений-паразитов, паразитирующих на деревьях. Он понимает высокоуровневые концепты этого домена и отношения между ними, топологию концептов и способен из известного ему домена найти топологическую окрестность для произвольно заданного концепта этого домена.

При этом за всю жизнь этот человек никогда ничего не слышал о домене знаний «Биология».

Однако если его спросят: «Есть такое живое существо — лошадь, и у неё нет корней», — то человек тут же спросит: «А как лошадь питается?»

Как человек сформулировал этот вопрос? В домене ботаники существует связь между концептами растения и питания корнями. 

Человек может спроецировать топологию концептов домена знаний «Ботаника» с концепта «растение» через родительский мета-концепт «жизнь» на новый концепт «животное» на основании их общности по родительскому концепту «жизнь». 

Сделав топологическую проекцию с одного концепта на другой, человек может начать познание с гипотезы, что результат проекции наиболее вероятно валиден в окрестности нового концепта «животное», и может сформулировать тесты для проверки качества своей проекции — задать вопрос, ответ на который зафиксирует верность части проекции или ослабит её. 

Сделав перенос из ботаники в биологию, человек предположил бы как питаются животные, — корнями. Логичное предположение, если вы никогда не видели животных. Как бы вы стали узнавать о них дальше, узнав, что корней нет? Во-первых, вы бы ослабили/отрезали концепт корня для животного на основе ответа собеседника, или результата наблюдения за ними, но вам по-прежнему был бы нужен концепт, реализующий потребность в питании для живого. Если животные — часть концепта «жизнь», то питание у них есть, значит, на основе входной информации топологическое место корня должно быть замещено иным гомологичным концептом как поставщиком питания. И вы можете искать этот концепт во внешнем мире, задавать вопросы, ставить опыты. И узнаете, что у животных поставщик питания — концепт «рот». Вы пришли к этому, использовав проекцию с известного домена на новый концепт через общий мета-концепт «поставщик питания».

Более того, наш ботаник может продолжить познание по аналогии. Он также сможет предположить, что концепт паразитизма существует и у животных, подобно тому как он существует в домене ботаники. Просто спроецировав топологические связи из одного домена на новую сущность из нового изучаемого домена — биологии. И он вновь может провести проверку, подтвердив или опровергнув эту гипотезу, закрепив её или ослабив в новом домене ботаники.

Для этого понадобится:
- строить домены знаний (GWOT MoE [3]?);
- собирать топологию домена относительно осмысляемого в данный момент концепта;
- искать подобные топологии в других доменах, возможно обнаруживая связь через мета-концепты/концепты-родители (растение и животное — оба являются концептами жизни);
- заполнять пробелы в одних доменах через проекцию из известных доменов, производя проверку результатов проекции и либо сохраняя, либо ослабляя связь унаследованной проекции;
- динамически создавать новые домены знаний, если новая информация порождает уникальную топологию, не похожую ни на что известное ранее (GWOT Dynamic MoE?).

Как результат мы получим универсальную модель, способную быстро обучаться, используя новый тип нативного концептуального трансфер-лёрнинга.

## Математика как мета-концептный домен

Особый интерес представляет механизм формирования математических концептов через топологический трансфер. Математика в этой парадигме — не отдельный изолированный домен, а мета-концептная надстройка, возникающая из обобщения повторяющихся топологических паттернов across множества конкретных доменов.

Рассмотрим концепт «количество». AI, взаимодействуя с разными доменами — считая яблоки в ботанике, овец в животноводстве, дни в календаре — обнаруживает инвариантную топологическую структуру: дискретные элементы, операцию объединения множеств, свойство коммутативности при объединении. Проецируя эти повторяющиеся паттерны в мета-домен и отсекая контекстно-зависимые свойства (цвет яблок, порода овец), система выводит абстрактный концепт натурального числа и операций над ним. Аналогично, концепт «непрерывного изменения», наблюдаемый в росте растений, движении объектов, изменении температуры, при проекции в мета-домен порождает концепты функции, предела, производной.

Ключевое отличие математического мета-домена — максимальная степень абстракции. Он содержит чистые топологические структуры, очищенные от всех конкретных свойств исходных доменов. Система может использовать этот мета-домен для мгновенного переноса математических закономерностей в любой новый домен, где обнаруживается изоморфная топология. Обнаружив в незнакомом домене структуру, изоморфную группе, система немедленно применяет весь аппарат теории групп без необходимости повторного обучения.

Таким образом, математическое мышление возникает не как отдельная способность, а как естественное следствие механизма консолидации топологий: обнаружение общих инвариантов, их абстрагирование и формирование мета-концептов высшего порядка. Это объясняет «непостижимую эффективность математики» — она эффективна потому, что является дистилляцией фундаментальных топологических инвариантов, присутствующих во множестве конкретных доменов реальности.

## Консолидация знаний

Однако и у человека часто так бывает, что его память и мышление фрагментарны. В одном контексте он строит одни цепочки рассуждений, в другом контексте — другие, причём взаимоисключающие. Известно это как «человек говорит то одно, то другое». 

Осознанный человек может с этим бороться только посредством рефлексии над своими знаниями и мыслями. А почему я так думаю/так считаю? Почему в ситуации А я думаю Б, а в ситуации Д я думаю С? А откуда я это знаю? Нет ли тут противоречий, беспристрастен ли я в своих выводах?

Он может выявить противоречия и попытаться их устранить. Привести свои взгляды к общему знаменателю, убрать логические противоречия в картине мира, **консолидировать модель мира**. Для этого есть две операции:

1. **Убрать компоненту личного восприятия**, записанную в памяти, из итогового рассуждения. «Я люблю демократов → то, что делают демократы, несёт позитивную оценку». Однако по факту позитивной оценки в моих логических рассуждениях быть не должно, какие-либо оценки должны даваться аргументам и следствиям, а не репутации автора, которая может быть лишь изначальным критерием для быстрой оценки не задумываясь. Демократы тоже могут делать плохие вещи, которые должны получать свои негативные оценки без когнитивного искажения за счёт личной предрасположенности у ним.  

2. **Консолидировать фрагментарную модель мира**. Так может оказаться, что в процессе познания были созданы фрагменты доменов с одинаковой топологией. Задача найти такие топологии и усилить их связь с общей топологией мета-модели (модели мета концепций), консолидировать топологии доменов с ней. При обнаружении неустранимых противоречий, где доменные топологии действительно расходятся ввиду фактических различий между сущностями, система должна:
   - **и/или динамически создавать новый (суб)домен или усилить расхождение связав его с причной расхождения** (или отдельный домен), фиксирующий уникальные топологические паттерны;
   - **и/или скорректировать мета-домен**, расширяя его концептуальное пространство для учёта выявленных расхождений и сохранения общих инвариантов.

Таким образом достигается адаптивная иерархия знаний: домены специализируются при необходимости, а мета-уровень эволюционирует, сохраняя согласованность всей системы представлений.

## Заключение

Предложена концептуальная схема автоматического нативного построения модели мира AI-системой, которая по сути своей любопытна, строит гипотезы на основе известного и подвергает их проверке.

Как это реализовать на практике? Я убеждён, что у нас уже есть все необходимые вычислительные мощности и почти все архитектурные приёмы для создания такой системы.

**GWOT Dynamic MoE + Recursive Latent Reasoning [4]?**

---

## Литература

[1] Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., Kaiser, Ł., & Polosukhin, I. (2017). Attention Is All You Need. *arXiv preprint arXiv:1706.03762*. https://arxiv.org/abs/1706.03762

[2] Dai, D., et al. (2024). DeepSeekMoE: Towards Ultimate Expert Specialization in Mixture-of-Experts Language Models. *arXiv preprint arXiv:2401.06066*. https://arxiv.org/abs/2401.06066

[3] Sasaki, M., Takeda, K., Abe, K., & Oizumi, M. (2025). Unsupervised alignment in neuroscience: Introducing a toolbox for Gromov-Wasserstein optimal transport. *Journal of Neuroscience Methods*, 419, 110443. https://doi.org/10.1016/j.jneumeth.2025.110443

[4] Jolicoeur-Martineau, A., et al. (2025). Less is More: Recursive Reasoning with Tiny Networks. *arXiv preprint arXiv:2510.04871*. https://arxiv.org/abs/2510.04871

[5] Kawakita, G., Zeleznikow-Johnston, A., Takeda, K., Tsuchiya, N., & Oizumi, M. (2024). Is my "red" your "red"?: Evaluating structural correspondences between color similarity judgments using unsupervised alignment. *Scientific Reports*, 14(1), 15917. https://doi.org/10.1038/s41598-024-65604-1

