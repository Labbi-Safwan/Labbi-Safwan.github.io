---
title: "Federated UCBVI: Communication-Efficient Federated Regret Minimization with Heterogeneous Agents"
collection: publications
category: conference
permalink: /publication/FedUCBVI
excerpt: 'We propose FedUCBVI, a federated optimistic value-iteration algorithm for reinforcement learning, and show that it enables multiple agents to learn efficiently from heterogeneous environments while reducing communication and retaining strong regret guarantees.'
date: 2025
venue: 'Proceedings of The 28th International Conference on Artificial Intelligence and Statistics, PMLR 258:1315-1323'
#slidesurl: 'https://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://proceedings.mlr.press/v258/labbi25a.html'
#bibtexurl: 'https://academicpages.github.io/files/bibtex1.bib'
#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
In this paper, we present the Federated Upper Confidence Bound Value Iteration algorithm
(\textsc{Fed-UCBVI}), a novel extension of the UCBVI algorithm
\citep{azar2017minimax} tailored for the federated learning framework. We prove that the
regret of \textsc{Fed-UCBVI} scales as
\[
\widetilde{O}\!\left(\sqrt{H^3 |\mathcal{S}| |\mathcal{A}| T / M}\right),
\]
with a small additional term due to heterogeneity, where $|\mathcal{S}|$ is the number of
states, $|\mathcal{A}|$ is the number of actions, $H$ is the episode length, $M$ is the
number of agents, and $T$ is the number of episodes. Notably, in the single-agent setting,
this upper bound matches the minimax lower bound up to polylogarithmic factors, while in
the multi-agent scenario, \textsc{Fed-UCBVI} has linear speed-up. To conduct our analysis,
we introduce a new measure of heterogeneity, which may hold independent theoretical
interest. Furthermore, we show that, unlike existing federated reinforcement learning
approaches, \textsc{Fed-UCBVI}'s communication complexity only marginally increases with
the number of agents.