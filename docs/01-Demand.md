---
book_filename: "1) Consumer demand"
title: 'Chapter 1: Consumer demand'
subtitle: Lecture notes for Econ 641
author: "Sebastien pouliot"
date: "Fall 2018"

documentclass: book
link-citations: yes
bibliography: References.bib
site: bookdown::bookdown_site
subparagraph: yes #Otherwise cannot use the titlesec package
geometry: "letterpaper, tmargin=1.0in, bmargin=1.1in, lmargin=1.15in, rmargin=1.15in, headheight=0in, headsep=0in, footskip=0.5in"
biblio-style: apalike
---

\setcounter{section}{2}

# Consumer demand

\noindent
Economists have long been interested in estimating the demand for goods. Many reasons motivate estimation of demand, including: 1) Predicting consumption to changes in tax, prices, quality; 2) Describing demand; 3) Forecasting; 4) Policy analysis; 5) Welfare studies; 6) Testing consumer theory. Interest in demand is not unique to scholars. The Economics Research Service (ERS) of the United States Department of Agriculture (USDA) invests significant effort into estimating demand for food commodity to conduct policy analysis. Private firms may also estimate demand to improve the marketing of their products or develop pricing strategies.


## Econometric problems in estimating demand
\noindent
Empirical results are conditioned by choices made by the econometrician. In general, parameter estimates and test results are conditioned by choices regarding the type of data, the functional forms, dependent variable and restrictions on the parameters. There is no getting around making choices when estimating an econometric model; this is true not only when estimating a system of demand but for any econometric estimation. Estimates are sometimes (very) sensitive to these choices which then makes credible inference difficult. A meta-analysis collects data to show how estimates vary according to methodology or type of data. An example of meta-analysis is @Gallet2010 who looks at estimates of the demand for meat.

@Leamer1983 warns that economists rarely have access to experiments and that identification is difficult. The data generating process is unknown and results may be sensitive to functional form choices. @Alston1991 make similar comments and note that inferences in studies of demand are fragile to specification choices.

<!-- \textcite{Leamer1983} had a major influence on the approach taken by economists to help with the identification of parameters. Economists now perform sensitivity analysis, have access to better data and rely on natural experiments and structural equations to obtain more credible estimates \autocite{Angrist2010}. Non-parametric inference and vector-error correction models have also improved the reliability of economic estimates. However, \textcite{Leamer2010} is not convinced. Other authors offer different perspectives \autocite{Keane2010,Nevo2010, Sims2010, Stock2010}.\footnote{The second issue in 2010 if the \emph{Journal of Economic Perspectives} offers a good summary regarding identification issues in economics. It discusses identification techniques in several fields of economics. A recent issue of the \emph{Journal of Economic Perspectives} revisits some of the material in the 2010 issues. See \autocite{AtheyImbens2017, LowMeghir2017, StockWatson2017, MullainathanSpiess2017, Powell2017, AngristPischke2017}. Both issues are worth reading.} -->

<!-- When estimating a model of demand, or any other empirical model, an economist must seek data that allow the identification of the parameters of interest, allow to test hypotheses or allow for meaningful predictions. The quality of the data is often an issue. In collecting data for demand estimation, an econometrician must consider that not all parameters may by precisely estimated given the data at hand. -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--   \item Time series data: -->
<!--     \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=5mm,label=-] -->
<!--           \item Elasticities (income and price); -->
<!--           \item Change in taste; -->
<!--           \item Functional forms tests; -->
<!--     \end{enumerate} -->
<!--   \item Cross-section data: -->
<!--     \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=5mm,label=-] -->
<!--           \item Income elasticities (price difficult); -->
<!--           \item Food at home vs. food away from home; -->
<!--           \item Demographic/socioeconomics factors; -->
<!--           \item Food stamps. -->
<!--     \end{enumerate} -->
<!--   \item Panel data -->
<!--       \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=5mm,label=-] -->
<!--           \item ... -->
<!--       \end{enumerate} -->
<!-- \end{enumerate} -->
<!-- It is possible to estimate income and price elasticities from time series data because these two variables change over time. However, in a cross-section, consumers face the same (or very similar) prices, which makes the estimation of price elasticities very difficult. The level of aggregation may also limit the usefulness of a dataset. For example, it is difficult to estimate the effects of demographics in a time series of US aggregate consumption of food. Disaggregated data that contain household consumption along with household characteristics will perform better. -->

<!-- I invite you to have a look at \textcite{Goodwin2015}. In his presidential address to the AAEA, Barry Goodwin discusses many empirical issues you must keep in mind in empirical estimation and policy analysis. -->

<!-- \subsubsection{Specification issues} -->
<!-- \noindent -->
<!-- Most demand models are based on economic theory and therefore impose restrictions derived from consumer theory. True restrictions increase precision and increase power for hypothesis tests. Incorrect restrictions cause biased estimates. Of course we want to impose \emph{true} restrictions but do we know for sure that the economic theory that we work with is correct? How can we test economic theory if any test is sensitive to the choice of functional forms and the choice of data? -->

<!-- A careful estimation of demand acknowledges and discusses limitations imposed by its approach. In particular, some of the specification issues that must be considered when estimating a model of demand include: -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--   \item Theoretical plausibility: Are the restrictions on consumer behavior acceptable? -->
<!--   \item Functional forms: Are the functional forms of the econometric model the same as the data generating process and do these functional forms bias estimates? Are non-parametric estimation techniques more appropriate? Danger of over-fitting. -->
<!--   \item Identification: Are prices and quantities both endogenous? What assumption allows to identify demand parameters from supply parameters? -->
<!--   \item Ceteris Paribus: What control variables should be included? How many control variables are correlated with the regressor of interest? -->
<!--   \item Error specification: Autocorrelation, heteroscedasticity? -->
<!--   \item Static theory vs. dynamic estimation: How do you handle and interpret dynamic variables (such as a time trend) when consumer theory is static? Are variables stationary? -->
<!--   \item Aggregation: Does consumer theory hold for aggregated data?  Aggregation is often imposed by the data collection process. -->
<!--   \item Separability: We cannot estimate a model of all goods in the economy. Which goods should be included?  What are the consequences of limiting the analysis to a set of goods? Separability is often imposed by the data available. What about separability with respect to future consumption? Storage? Future prices? -->
<!-- \end{enumerate} -->

<!-- We will explore in this section empirical models of demand and discuss some specification issues. We will focus on the most commonly used models and their properties. The treatment of demand analysis in this course is not comprehensive but should give you a good basis for your future research or to understand the research of others. Good references include \textcite{Deaton1980} and \textcite{Johnson1984}. A recent summary of consumer demand analysis that I recommend you read is \textcite{Okrent2011}. -->

<!-- %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% -->
<!-- \subsection{Restrictions on demand imposed by the data} -->
<!-- \noindent -->
<!-- The availability of data often dictates restrictions on the type of model that an econometrician can estimate. What are the effects of these restrictions? Are the restrictions so strong that a system of demand does not yield consistent estimates? In this section, we explore the conditions under which demand theory is consistent with the restrictions imposed by the data. We will begin by looking at restrictions on the number of goods available and then we will look at restrictions from aggregation. -->

<!-- %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% -->
<!-- \subsubsection{Separability assumptions} -->
<!-- \noindent -->
<!-- Empirical analysis of demand focuses on a subset of goods that is limited by the data available or selected by the econometrician. In practice, consumers buy thousands of different goods and it would not be feasible for an economist to consider all of these goods within a system of demand. It is impossible to obtain data for all goods in the economy and to specify a demand system for all available products. -->

<!-- When is it possible to disentangle the demand for a subset of goods from the remaining goods? To determine this, we must look at where consumer's demand comes from. Recall that the consumer maximization problem is -->
<!-- \begin{equation*} -->
<!-- \arg \max_{x_1,...,x_N} U(x_1,...,x_N) \; \text{ s.t. } \; \sum_i p_i x_i \leq W, -->
<!-- \end{equation*} -->
<!-- where $x_i$ is the consumption of good $i$ and $p_i$ is the price of good $i$. The solution of the utility maximization problem yields the Marshallian demand $x_1^{\ast},...,x_N^{\ast}$. Typically, when estimating a demand system, we want to focus on a set of $k$ goods. Estimation of demand for a selected group of goods is theoretically correct only if certain restrictions hold. We will see that under some conditions on the utility function or on the price vector, that focusing on a subset of goods does not bias demand estimates. The separability conditions are most often not made explicit, are assumed to hold and not tested. See \textcite{Moschini1994} for some detail on how to test for the separability of the demand. -->

<!-- I will not discuss time separability. The models of demand that we will consider in this section are based on static economic theory. We will ignore issues related to expectation about future prices and to storage and impose that the demand in one period is independent of past and future consumption. -->

<!-- \paragraph{Hicksian separability} -->
<!-- \noindent -->
<!-- Hicksian separability, also referred to as the \emph{composite commodity theorem}, imposes a structure on prices and on the utility function. Instead of using $U(x_1,...,x_k,x_{k+1},...,x_N)$ in the maximization problem, we want to use $U^{H}(x_1,...,x_k,z)$ where $z$ is a composite good, and where the consumer maximization problem yields $x_1^{\ast},...,x_k^{\ast}$ under both utility specifications. Hicksian separability says that there is a price structure $p_{k+1},...,p_N$ such that -->
<!-- \begin{equation*} -->
<!-- \left( -->
<!--     \begin{array}{c} -->
<!--     p_{k+1}\\ -->
<!--     .\\ -->
<!--     .\\ -->
<!--     .\\ -->
<!--     p_N -->
<!--     \end{array} -->
<!-- \right) -->
<!-- = \pi -->
<!-- \left( -->
<!--     \begin{array}{c} -->
<!--     \tilde{p}_{k+1}\\ -->
<!--     .\\ -->
<!--     .\\ -->
<!--     .\\ -->
<!--     \tilde{p}_N -->
<!--     \end{array} -->
<!-- \right) -->
<!-- \end{equation*} -->
<!-- and that we can define a composite commodity $z=\sum_{l=k+1}^{N} \tilde{p}_l x_l$. Hicksian separability holds if and only if -->
<!-- \begin{equation*} -->
<!-- \arg \max_{x_1,...,x_N} U(x_1,...,x_k,x_{k+1},...,x_N) \; \text{ s.t. } \; \sum_i p_i x_i \leq W -->
<!-- \end{equation*} -->
<!-- and -->
<!-- \begin{equation*} -->
<!-- \arg \max_{x_1,...,x_k,z} U^{H}(x_1,...,x_k,z) \; \text{ s.t. } \; \sum_i^{k} p_i x_i + \pi z \leq W, -->
<!-- \end{equation*} -->
<!-- both yield $x_1^{\ast},...,x_k^{\ast}$. -->

<!-- \paragraph{Weak separability} -->
<!-- \noindent -->
<!-- Unlike Hicksian separability, weak separability imposes structure on the utility function only. Under weak separability, we can write the utility function such that -->
<!-- \begin{equation*} -->
<!-- U(x_1,...,x_N)=U(\upsilon(x_1,...,x_k),x_{k+1},...,x_N). -->
<!-- \end{equation*} -->
<!-- This implies that $MRS_{x_i,x_j\in(x_1,...,x_k)} \perp z \in (x_{k+1},...,x_N)$. If weak separability holds, we can think of the utility maximization problem in 2 stages: -->
<!-- \begin{enumerate} -->
<!--     \item $\max_{x_1,...,x_k} \upsilon(x_1,...,x_k) \; \text{ s.t. } \; \sum_i^{k} p_i x_i \leq m$ which yields $V(\mathbf{p},m)=V(x_1^{\ast},...,x_k^{\ast})$.    \item $\max_{m,x_{k+1},...,x_N} U(V(x_1^{\ast},...,x_k^{\ast}),x_{k+1},...,x_N) \; s.t. \; m+\sum_{k+1}^{N} p_i x_i \leq W$. -->
<!-- \end{enumerate} -->
<!-- The assumption of weak separability is almost invariably imposed. Thus, most often, models of demand focus on the group of goods in the first stage above and consider the expenditure over that group of goods rather than wealth. \textcite{Lafrance1993} shows that welfare measurement with weakly separable goods produces biases. -->

<!-- \paragraph{Strong separability} -->
<!-- \noindent -->
<!-- Strong separability imposes more structure on the utility function than weak separability. Strong separability assumes that -->
<!-- \begin{equation*} -->
<!-- U(x_1,...,x_N)=U(\upsilon_1(x_1),...,\upsilon_N(x_N)). -->
<!-- \end{equation*} -->
<!-- The assumption of strong separability is however stronger than we need for the material we will cover in this course. -->

<!-- \paragraph{Incomplete demand system} -->
<!-- \noindent -->
<!-- In an incomplete demand system, it is not required to include consumption of all goods within the system. A system is incomplete if the demand $x_1,...,x_k$ are observable but that demand $x_{k+1},...,x_N$, where $N>k+2$, are not. Although consumption of all goods are not observable, all prices are observed. Under some regularity conditions, the system can be treated as complete by augmenting the incomplete demand system with a composite num\'{e}raire and by deflating the price of the observable goods by a price index for the non observable good. See \textcite{Epstein1982} for detail. -->

<!-- \paragraph{Two-stage budgeting} -->
<!-- \noindent -->
<!-- Two-stage budgeting relates to weak separability. In two-stage budgeting, consumers allocate their budget among groups of goods. Thus, two-stage budgeting is not an outcome of a separability assumption, but the core assumption that allows for estimation considering a subset of goods. See \textcite{Okrent2011} for detail. -->

<!-- \subsubsection{Aggregation} -->
<!-- \noindent -->
<!-- Consumer theory assumes a single representative consumer but, in practice, a representative consumer does not exist. Consumers have heterogenous preferences and thus do not derive the same utility for the consumption of a good. Think for example the difference between the utility that a typical man and a typical woman derive from a nice pair of high-heel shoes. In addition, consumers do not have the same income, which, of course, affects consumption as well. -->

<!-- Consumption data are rarely disaggregated at the individual consumer level.\footnote{We will discuss microdata in section \ref{sec:microdata}.} Most often, data are available at a certain level of aggregation (e.g. county, state or country). For example, US meat consumption data (in fact, typically the disappearance of meat) often used in the literature are available at the country level. When is it valid to use these data? Microeconomic theory, that derives from the study of a representative consumer, does not always hold at the aggregate level. -->

<!-- To expose the problem of aggregation more precisely, we can write the aggregate demand as -->
<!-- \begin{equation*} -->
<!-- x(\mathbf{p}, W_1, W_2,...,W_M) = \Sigma_{\ell=1}^{M} x_{\ell}(\mathbf{p}, W_{\ell}), -->
<!-- \end{equation*} -->
<!-- where $\ell$ identifies consumers. Observe that all consumers face the same price vector. When is it correct to write -->
<!-- \begin{equation*} -->
<!--  \Sigma_{\ell=1}^{M} x_{\ell}(\mathbf{p}, W_{\ell}) =  x(\mathbf{p}, \Sigma_{\ell=1}^{M} W_{\ell})? -->
<!-- \end{equation*} -->
<!-- Alternatively, we can divide by $M$, the number of consumers, and ask instead whether the demand by a representative consumer exists. -->

<!-- The condition for the correct aggregation of consumer demand is that the distribution of wealth does not affect the aggregate demand. We can show that condition by taking the differential of the aggregate demand for a good $i$ -->
<!-- \begin{equation*} -->
<!--  \Sigma_{\ell=1}^{M} \frac{\p x_{i\ell}(\mathbf{p}, W_{\ell})}{\p W_{\ell}} d W_{\ell} = 0 \text{ } \forall i. -->
<!-- \end{equation*} -->
<!-- This can only be true for a redistribution of wealth that holds total wealth constant, i.e. $\Sigma_{\ell=1}^{M} d W_{\ell} = 0$, only if -->
<!-- \begin{equation*} -->
<!-- \frac{\p x_{i\ell}(\mathbf{p}, W_\ell)}{\p W_{\ell}} = \frac{\p x_{ik}(\mathbf{p}, W_k)}{\p W_k} \text{ } \forall \ell,k -->
<!-- \end{equation*} -->
<!-- This condition implies a linear wealth expansion path. In consequence, aggregation of consumer demand is possible under certain restrictions on the shape of Engel curve, a concept related to wealth expansion path. -->

<!-- One type of expenditure function that allows for exact linear consumer aggregation is the Gorman (polar) form -->
<!-- \begin{equation*} -->
<!-- e(\mathbf{p},u) = a(\mathbf{p}) + u b(\mathbf{p}). -->
<!-- \end{equation*} -->
<!-- You can derive from this expression using Roy's identity that the Engel curves are linear. Although it allows for exact aggregation, one problem with the linear Engel curves from the Gorman form is that they are not consistent with empirical evidence \autocite{Deaton1980a, Banks1997}. The PIGLOG (Price Independent Generalized Linear in Log) class of preferences yields Engel curves more consistent with empirical evidence and allows for exact nonlinear aggregation of consumers -->
<!-- \begin{equation*} -->
<!-- \ln{e(\mathbf{p},u)} = a(\mathbf{p}) + u b(\mathbf{p}). -->
<!-- \end{equation*} -->
<!-- where $u \in (0,1)$ with 0 meaning subsistence and 1 bliss. Demand derived from the expenditure function above yield log-linear Engel curves. As we will see below, many models of demand derive from PIGLOG class of preferences. -->

<!-- Under correct aggregation, it is possible to estimate models of demand considering a representative consumer. \textcite{Deaton1980a} provide detail on consumer aggregation. \textcite{MasColell1995} discuss exact linear aggregation. -->

<!-- %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% -->

<!-- \subsection{Empirical models of demand} -->
<!-- \noindent -->
<!-- In what follows, we will derive demand systems consistent with economic theory. The appendix to this chapter gives a brief summary of consumer theory with an emphasis on the properties of demand. -->

<!-- To satisfy economic theory, we will require that the following properties hold -->
<!-- \renewcommand\minalignsep{0pt} -->
<!-- \begin{align} -->
<!--     \text{Symmetry: } & \eta_{ij}^{H} s_i = \eta_{ji}^{H} s_j;\label{eq.Symmetry}\\ -->
<!--     \text{Homogeneity: } & \sum_j \eta_{ij} + \eta_{iW} = 0 \text{ or } \sum_j \eta_{ij}^{H} = 0;\label{eq.Homogeneity}\\ -->
<!--     \text{Engel aggregation: } & \sum_i s_i \eta_{iW} =1;\label{eq.Engel}\\ -->
<!--     \text{Cournot aggregation: } & s_j + \sum_i s_i \eta_{ij}=0, \label{eq.Cournot} -->
<!-- \end{align} -->
<!-- where, $\eta_{ij}^{H}$ is the Hicksian elasticity of demand for good $i$ with respect to the price of good $j$, $s_i$ is the expenditure share for good $i$, $\eta_{ij}$ is the demand elasticity of good $i$ with respect to the price of good $j$, $W$ is income and $\eta_{iW}$ is the income elasticity of good $i$. Another desirable property is the semi negativeness of the Slutsky matrix. Although that last condition is difficult (tedious) to impose, it is not difficult to verify. -->

<!-- A demand system is \emph{integrable} if it could have been derived from a utility function. That is, it is possible from the Hicksian demand to recover the cost function and then by inversion to obtain the utility function. A system of demand is integrable if it satisfies adding-up conditions (Engel aggregation and Cournot aggregation), homogeneity and symmetry of the Slutsky matrix. A demand system is \emph{rational} if it is integrable and the Slutsky matrix is semi-negative definite \autocite{Lewbel1996}. -->

<!-- We will see below several models of demand. This summary however covers only the most popular models. See \textcite{Okrent2011} for estimating equations and restrictions for many other models. -->

<!-- Note that we will use $m$ to denote per capita expenditure on the group of weakly separable goods such that $m+\sum_{k+1}^{N} p_i x_i=W$. With aggregated data, we use per capita expenditure values to neutralize the effect of population growth. -->

<!-- \subsubsection{Single-equation models} -->
<!-- \noindent -->
<!-- Early empirical models of demand were not derived specifically from consumer theory. These models, although they include some theoretical restrictions, are not fully consistent with economic theory. You can find detail about these models in \textcite{Deaton1980} or in \textcite{Johnson1984}. -->

<!-- I discuss the double-log model and a transformation of that model. \textcite{Okrent2011} discuss the Box-Cox model that nests the linear model, the semi-log model and the double-log model. -->

<!-- \paragraph{Double-log model} -->
<!-- \noindent -->
<!-- Recall that elasticities are defined as ratios of the percentage changes in two variables. A good approximation of a change in percentage is the change in logs, implying that a good approximation of the price elasticity of demand is $\eta_{ij} \approx d\log(x_i)/d\log(p_j)$. Thus, it seems natural to obtain elasticities of demand by estimating -->
<!-- \begin{equation}\label{eq.dlog} -->
<!-- \ln{x_i} = \alpha_i + \eta_{im} \ln{m} + \sum_j \eta_{ij} \ln{p_j} + u_i, -->
<!-- \end{equation} -->
<!-- where $u_i$ is an error term. The main advantages of the double-log model is that 1) it is easy to estimate and 2) it is possible to test theoretical restrictions. However, the double-log model is not integrable unless budget shares are constant \autocite{Johnson1984} as they are with Cobb-Douglas utility function. -->

<!-- \paragraph{Stone model} -->
<!-- \noindent -->
<!-- Richard Stone wished to use the double-log model in \eqref{eq.dlog} to estimate demand functions for 48 products with only 19 observations.\footnote{Richard Stone received the Nobel Memorial Prize in Economic Science for the development of national accounting systems. Still, Stone's most often cited work are his papers on consumer demand analysis.} One solution was to set cross-price elasticities to zero but Stone considered it too restrictive and not satisfying. Instead, Stone used the double-log model in \eqref{eq.dlog} and the Slutsky equation in \eqref{eq.Slutsky} to write that -->
<!-- \begin{equation}\label{eq.Stone} -->
<!-- \ln{x_i} = \alpha_i + \eta_{im} \ln{(\frac{m}{P})} + \sum_j \eta_{ij}^{H} \ln{p_j} + u_i, -->
<!-- \end{equation} -->
<!-- where $P=\prod_j p_j^{s_j}$ is the Stone price index and $s_j$ are the expenditure shares. The Stone model is a restatement of the double-log model that allows the direct estimation of Hicksian price elasticities. In his analysis, Stone uses the homogeneity restriction in \eqref{eq.Homogeneity} to limit the estimation of elasticities to close substitutes and complements \autocite[see][pages 61-64]{Deaton1980}. -->

<!-- \subsubsection{Maximization of utility function} -->
<!-- \noindent -->
<!-- An easy way to derive a model of demand that is consistent with economic theory is to begin with a functional form for the utility function and derive demand equations. Although appealing for its consistency with economic theory, the functional forms for the demand are not sufficiently flexible and rarely yield estimates consistent with empirical evidence. -->

<!-- \paragraph{Cobb-Douglas model} -->
<!-- \noindent -->
<!-- The Marshallian demand of a good $i$ for a consumer with a Cobb-Douglas utility function is given by -->
<!-- \begin{equation*} -->
<!-- x_i(p_i,m) = \frac{\alpha_i m}{p_i}, -->
<!-- \end{equation*} -->
<!-- where here $\alpha_i$ is the exponent associated to the consumption of good $i$ in the utility function. Taking logs on both sides, we can write that the stochastic version of the log of the demand as -->
<!-- \begin{equation*} -->
<!-- \ln{x_i(p_i,m)} = \beta_i + \beta_m \ln{m} - \beta_{p_i} \ln{p_i} + u_i. -->
<!-- \end{equation*} -->
<!-- If consumers have Cobb-Douglas utility functions, the coefficient for the income and the price should equal 1, $\beta_m=1$ and $\beta_{p_i}=1$, and the intercept should equal the log of the expenditure share, i.e. $\beta_i=\ln{\alpha_i}=\ln{s_i}$. This makes the Cobb-Douglas very restrictive: -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item Budget shares are constant. However, theory says that expenditure shares decline with respect to income for non-luxury goods $(\eta_{im}<1)$ like food (Try to prove that). -->
<!--     \item Constant elasticities: $\eta_{im}=1$, $\eta_{i}=1$ and $\eta_{ij}=0$, where the value of the cross-price elasticity implies that $\sigma_{ij}=1$. -->
<!-- \end{enumerate} -->
<!-- The Cobb-Douglas model is theoretically correct but not empirically plausible. Because of unit income elasticity, Engel's law cannot be satisfied.\footnote{Engel's law is not a law by definition but an empirical observation. The law states that as income rises, the expenditure share of food decreases even though the expenditure on food increases. This is because food is a normal good with its elasticity of income being between zero and one.} The Constant Elasticity of Substitution (CES) utility function allows for values of the elasticity of substitution other than 1 but maintains the other restrictions. -->

<!-- \paragraph{Linear expenditure system (LES)} -->
<!-- \noindent -->
<!-- Consider the \emph{Stone-Geary} utility function -->
<!-- \begin{equation*} -->
<!-- U(\mathbf{x}) = \prod_{i=1}^{N}(x_i - \gamma_i)^{\beta_i} -->
<!-- \end{equation*} -->
<!-- where the parameter $\gamma_i$ can be interpreted as a subsistence quantity for good $i$. The Cobb-Douglas utility function is a special case of the Stone-Geary utility function. From maximization of the utility function under a budget constraint, the Marshallian demand is given by -->
<!-- \begin{equation*} -->
<!-- x_i(\mathbf{p},m) = \gamma_i + \frac{\beta_i}{p_i}(m-\sum_{j \neq i} p_j \gamma_j). -->
<!-- \end{equation*} -->
<!-- Thus, by multiplying both sides by $p_i$, we find that expenditure on a good is a linear function of total expenditure and prices, as the name of the model suggests. Because of the subsistence quantity, the wealth expansion paths are not linear with respect to the origin (see figure \ref{fig.LES}) unlike in the Cobb-Douglas model. Note also that the expenditure shares are no longer constant -->
<!-- \begin{equation*} -->
<!-- s_i = \frac{p_i x_i(\mathbf{p},m) }{m} = \frac{p_i \gamma_i}{m} + \beta_i \left(1-\frac{\sum_j p_j \gamma_j}{m} \right). -->
<!-- \end{equation*} -->
<!-- The income elasticity is given by -->
<!-- \begin{equation*} -->
<!-- \eta_{im} = \frac{\beta_i m}{p_i x_i(\mathbf{p},m)} = \frac{\beta_i}{s_i}, -->
<!-- \end{equation*} -->
<!-- where $\beta_i>0$ such that there is no inferior good. The LES also rules out substitute goods \autocite{Johnson1984}. -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!--     \begin{picture}(240,240) -->
<!--         %Axises and labels -->
<!--         \thicklines -->
<!--         %\scriptsize -->
<!--         \put(0,0){\vector(1,0){240}} %x-axis -->
<!--         \put(0,0){\vector(0,1){220}} %y-axis -->
<!--         \put(215,-10){$x_1$} -->
<!--         \put(-15,210){$x_2$} -->
<!--         %Lines -->
<!--         \multiput(40,0)(0,10){22}{\line(0,1){5}}%Dashed line - vertical -->
<!--         \multiput(0,40)(10,0){22}{\line(1,0){5}}%Dashed line - vertical -->
<!--         %Utility function -->
<!--         \qbezier(20, 220)(50, 50)(220, 20)%U^0 -->
<!--         \qbezier(50, 220)(80, 80)(220, 50)%U^1 -->
<!--         %Budget lines -->
<!--         \put(0,78){\line(4,-1){220}} %x-axis -->
<!--         \put(0,104){\line(4,-1){220}} %x-axis -->
<!--         %dots -->
<!--         \put(152,40){\circle*{4}} -->
<!--         \put(208,52){\circle*{4}} -->
<!--         %Labels -->
<!--         \put(40,-10){$\gamma_1$} -->
<!--         \put(-15,40){$\gamma_2$} -->
<!--         %Income expansion path -->
<!--         %\thicklines -->
<!--         \linethickness{2pt} -->
<!--         \put(40,40){\line(1,0){143}} -->
<!--         \put(182,40){\line(26,12){38}} -->
<!--         \end{picture} -->
<!-- \vspace{0.1in} -->
<!-- \caption{Utility maximization with LES} \label{fig.LES} -->
<!-- \end{center} -->
<!-- \end{figure} -->

<!-- \subsubsection{Differential approximation of demand function} -->
<!-- \noindent -->
<!-- One way to derive an empirical equation for demand estimation is to shock a Marshallian demand and consider how small changes in each variable affect the demand. That is, we can take the differential of the demand function and then find an expression for the change in the demand, which becomes the estimating equation for the econometric model. Imposing the correct restrictions on that expression assures that the demand system conforms to economic theory. There are many systems of demand derived from a differential approximation of demand functions, see \textcite{Okrent2011} for some detail. Below, I present the Rotterdam model, the differential system of demand that I believe has been historically the most commonly used. The Barten's synthetic model of demand seems to have gained popularity recently. -->

<!-- \paragraph{Rotterdam model} -->
<!-- \noindent -->
<!-- The Rotterdam model has been around for a long time. It is based on the differential of a Marshallian demand. Consider the Marshallian demand for a good $i$ written as -->
<!-- \begin{equation*} -->
<!-- x_i = x_i(\mathbf{p},m). -->
<!-- \end{equation*} -->
<!-- Totally differentiating that expression yields -->
<!-- \begin{equation}\label{eq:dx} -->
<!-- d x_i = \frac{\p x_i(\mathbf{p},m)}{\p m} d m + \sum_j \frac{\p x_i(\mathbf{p},m)}{\p p_j} d p_j. -->
<!-- \end{equation} -->
<!-- Note that it is not too difficult to expand the previous expression by including other variables that affect demand. Dividing both sides of \eqref{eq:dx} by $x_i$ yields -->
<!-- \begin{align*} -->
<!-- & \frac{d x_i}{x_i} &= \frac{\p x_i(\mathbf{p},m)}{\p m} \frac{m}{x_i} \frac{d m}{m} + \sum_j \frac{\p x_i(\mathbf{p},W)}{\p p_j} \frac{p_j}{x_i} \frac{d p_j}{p_j} -->
<!-- &\approx d \ln{x_i} = \eta_{im} d \ln{m} + \sum_j \eta_{ij} d \ln{p_j}. -->
<!-- \end{align*} -->
<!-- Using the Slutsky equation in \eqref{eq.Slutsky}: -->
<!-- \begin{align*} -->
<!-- d \ln{x_i} &= \eta_{im} d \ln{m} + \sum_j (\eta_{ij}^{H} - s_j \eta_{im} ) d \ln{p_j}\\ -->
<!--             &= \eta_{im} (d \ln{m} - \sum_j s_j d \ln{p_j}) + \sum_j \eta_{ij}^{H} d \ln{p_j}, -->
<!-- \end{align*} -->
<!-- which is in fact the Stone model in differential form (recall that $\ln{P}=\sum_j s_j d \ln{p_j}$ is the log of the Stone price index). -->

<!-- Empirically, the Rotterdam model is specified by multiplying both sides by $s_i$ such that the model can satisfy symmetry: -->
<!-- \begin{equation*} -->
<!-- s_i d \ln{x_i} = \beta_i d \ln{M} + \sum_j \gamma_{ij} d\ln{p_j} + u_i, -->
<!-- \end{equation*} -->
<!-- where $d \ln{M} = d \ln{m} - \sum_j s_j d \ln{p_j}$, $\beta_i = s_i \eta_{im}= p_i \frac{\p x_i}{\p m}$ and $\gamma_{ij}=s_i \eta_{ij}^{H}$. Thus symmetry can be imposed by setting $\gamma_{ij}= \gamma_{ji}$ such that $s_i \eta_{ij}^{H} = s_j \eta_{ji}^{H}$. We can also impose the following theoretical constraints to the model -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=17mm,label=\roman*.] -->
<!--     \item Adding up constraints: $\sum_j \beta_j=1$; $\sum_j \gamma_{jk}=0$; -->
<!--     \item Homogeneity: $\sum_j \gamma_{kj}=0$; -->
<!--     \item Symmetry: $\gamma_{ij} = \gamma_{ji}$. -->
<!-- \end{enumerate} -->
<!-- \textcite{Johnson1984} note that for empirical applications of the Rotterdam model with discrete observations the $d \ln's$ should be replaced by $\Delta \ln's$ and $s_i$ should be replaced by $s_i^\ast = (1/2)(s_{it}+s_{it+1})$, where $t$ indicates time. -->

<!-- We can calculate elasticities from parameter estimates of the Rotterdam model using the following expressions -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item $\eta_{im}=\frac{\beta_i}{s_i}$; -->
<!--     \item $\eta_{ij}^{H}=\frac{\gamma_{ij}}{s_i}$; -->
<!--     \item $\eta_{ij}=\frac{(\gamma_{ij}-s_j \beta_i)}{s_i}$. -->
<!-- \end{enumerate} -->

<!-- \subsubsection{Application of Roy's identity} -->
<!-- \noindent -->
<!-- Many systems of demand are derived based on an expression for the indirect utility function. Demand systems derived using Roy's identity are integrable because it is possible to recover the utility function from which the system of demand equations is derived. Slutsky restrictions ensure that a demand system is integrable. I will assume a translog functional form for the indirect utility function. Other functional forms are of course possible. I will give more detail about flexible functional forms in chapter 2 when we will discuss the estimation of production functions. -->

<!-- \paragraph{Translog model} -->
<!-- \noindent -->
<!-- Translog stands for \emph{Transcendental logarithmic}, a flexible functional form proposed by \textcite{Christensen1975}. Consider the following indirect translog utility function: -->
<!-- \begin{equation*} -->
<!-- \ln{V(\mathbf{p},m)}=\alpha_0 + \sum_i \alpha_i \ln{(\frac{p_i}{m})} + \frac{1}{2} \sum_i \sum_j \beta_{ij} \ln{(\frac{p_i}{m})} \ln{(\frac{p_j}{m})}. -->
<!-- \end{equation*} -->
<!-- To derive the expression for the demand, we use Roy's identity in \eqref{eq.Roy} with a slight modification. In the translog indirect utility function, we have the log of the indirect utility function on the left-hand side. We therefore must consider Roy's identity in its log form -->
<!-- \begin{equation*} -->
<!-- s_i=\frac{p_i x_i}{m}= - \frac{\p V}{\p p_i}\frac{p_i}{V} \bigg/ \frac{\p V}{\p m}\frac{m}{V} \approx -\frac{\p \ln{V}}{\p \ln{p_i}} \bigg/ \frac{\p \ln{V}}{\p \ln{m}}. -->
<!-- \end{equation*} -->
<!-- Because $\frac{\p \ln{\frac{p_i}{m}}}{\p \ln{p_i}}=1$, we can write that -->
<!-- \begin{equation*} -->
<!-- s_i = -\frac{\p \ln{V}}{\p \ln{(\frac{p_i}{m})}} \bigg/ \frac{\p \ln{V}}{\p \ln{m}}. -->
<!-- \end{equation*} -->
<!-- Thus, from the indirect utility, after imposing symmetry by letting $\beta_{ij}=\beta_{ji}$, we find the following expression to estimate: -->
<!-- \begin{equation*} -->
<!-- s_i = \frac{\alpha_i + \sum_j \beta_{ij} \ln{(\frac{p_j}{m})}}{\sum_j \alpha_j + \sum_k \sum_j \beta_{kj} \ln{(\frac{p_j}{m})} \ln{(\frac{p_k}{m})} } + u_i. -->
<!-- \end{equation*} -->
<!-- The share equation is homogeneous of degree zero in prices and income. Not all parameters can be estimated and a convenient normalization is to set $\sum_j \alpha_j=1$. Another convenient normalization is to let $\sum_i \sum_j \beta_{ij} = 0$ such that the translog can be aggregated across consumers \autocite{Moschini1994}. Because of singularity, it is possible to estimate only $N-1$ equations, where $N$ is the number of goods in the system. Parameters of the equation that are deleted can be recovered from theoretical restrictions on demand. -->

<!-- The expressions for the elasticities for the translog model of demand are (to double check before using): -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item $\eta_{im} = 1+\frac{-\sum_{j}\beta_{ij} }{\alpha_i + \sum_j \beta_{ij} \ln{(\frac{p_j}{m})}}$; -->
<!--     \item $\eta_i = \frac{\beta_i}{\alpha_i + \sum_j \beta_{ij} \ln{(\frac{p_j}{m})}} - \frac{\sum_k \beta_{ki}}{1+\sum_k \sum_j \beta_{kj} \ln{(\frac{p_j}{m}})} - 1$; -->
<!--     \item $\eta_{ij} = \frac{\beta_{ij}}{\alpha_i + \sum_j \beta_{ij} \ln{(\frac{p_j}{m})}} - \frac{\sum_k \beta_{ki}}{1+\sum_k \sum_j \beta_{kj} \ln{(\frac{p_j}{m}})} $. -->
<!-- \end{enumerate} -->

<!-- \subsubsection{Application of Shephard's lemma} -->
<!-- \noindent -->
<!-- Maybe the most common method to derive a demand system is by specifying an expression for the cost function that is consistent with consumer aggregation. Using Shephard's lemma, it is then possible to derive expressions for a system of demand equations that is integrable and consistent with aggregation. I describe the AIDS model below. Many other systems of demand are derived using similar approach. -->

<!-- \paragraph{AIDS model} -->
<!-- \noindent -->
<!-- The \emph{Almost Ideal Demand System model} (AIDS) was proposed by \textcite{Deaton1980a}. The model is based on an expenditure function of the PIGLOG class of preferences -->
<!-- \begin{equation}\label{eq.cost} -->
<!-- \ln{e(\mathbf{p},u)} = a(\mathbf{p}) + u b(\mathbf{p}). -->
<!-- \end{equation} -->
<!-- where $u \in (0,1)$ with 0 meaning subsistence and 1 bliss. The PIGLOG expenditure function is related to the Gorman (polar) form of the expenditure function given by $e(\mathbf{p},u) = a(\mathbf{p}) + u b(\mathbf{p})$ that allows for consumer aggregation. The Gorman form yields linear Engel curves which, as mentioned before, is not consistent with empirical evidence. The PIGLOG allows for more general Engel curves while allowing for a model of demand derived from a representative consumer's perspective \autocite{Deaton1980a}. -->

<!-- \textcite{Deaton1980a} propose the following functional forms for $a(\mathbf{p})$ and $b(\mathbf{p})$ -->
<!-- \begin{align*} -->
<!-- a(\mathbf{p}) &= \alpha_0 + \sum_i \alpha_i \ln{p_i} + \frac{1}{2} \sum_i \sum_j \gamma_{ij}^\ast \ln{p_i} \ln{p_j}; \\ -->
<!-- b(\mathbf{p}) &= \beta_0 \prod_k p_k^{\beta_k}. -->
<!-- \end{align*} -->
<!-- We can derive other demand models by considering other functional forms for $a(\mathbf{p})$ and $b(\mathbf{p})$. The functional forms proposed by \textcite{Deaton1980a} imply a rank two for the Engel curve. \textcite{Lewbel1991} propose a test to select the correct rank. -->

<!-- From Shephard's lemma in logarithmic form $(\frac{\p \ln{e(\mathbf{p},u)}}{\p \ln{p_i}} = s_i)$ we find that the share equations are given by -->
<!-- \begin{equation*} -->
<!-- s_i = \alpha_i + \sum_j \gamma_{ij} \ln{p_j} + \beta_i \ln{(\frac{m}{P})}, -->
<!-- \end{equation*} -->
<!-- where $P$ is a price index defined as -->
<!-- \begin{equation*} -->
<!-- \ln{P} = \alpha_0 + \sum_j \alpha_j \ln{p_j} + \frac{1}{2} \sum_i \sum_j \gamma_{ij} \ln{p_j} \ln{p_i}, -->
<!-- \end{equation*} -->
<!-- where $\gamma_{ij}= \frac{1}{2} (\gamma_{ij}^\ast + \gamma_{ji}^\ast) = \gamma_{ji}$. Note that $\alpha_0$ is quite difficult to estimate and is often set equal to zero. -->

<!-- Theoretical restrictions such that the AIDS model is consistent with economics theory are the following -->
<!--  \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=17mm,label=\roman*.] -->
<!--      \item Adding up constraints: $\sum_i \alpha_i=1; \sum_i \beta_i=0; \sum_i \gamma_{ij}=0$; -->
<!--      \item Homogeneity: $\sum_j \gamma_{ij}=0$; -->
<!--      \item Symmetry: $\gamma_{ij} = \gamma_{ji}$. -->
<!--  \end{enumerate} -->
<!-- Note also that these expressions do not hold when the demand model includes other shifters. \textcite{Alston2001} shows a solution to correctly include demand shifters in an AIDS model. -->

<!-- The expressions for the demand elasticities for the AIDS model are given by the following expressions -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item $\eta_{im} = 1+\frac{\beta_i}{s_i}$; -->
<!--     \item $\eta_i = -1 + \frac{\gamma_{ii}-\beta_i(\alpha_i - \sum_j \gamma_{ij} \ln{p_j})}{s_i}$; -->
<!--     \item $\eta_{ij} = \frac{\gamma_{ij}-\beta_j(\alpha_j - \sum_j \gamma_{ij} \ln{p_j})}{s_i}$. -->
<!-- \end{enumerate} -->

<!-- The AIDS model has often been estimated using a linear version of the price index by using instead the Stone price index: -->
<!-- \begin{equation*} -->
<!-- \ln{P} \approx \ln{P^\ast} = \sum_k s_k \ln{P_k}. -->
<!-- \end{equation*} -->
<!-- The model with the linear approximation of the price index is referred to as the LA/AIDS model. That model is easier to estimate and helps solve a multi-collinearity problem in the price index $\ln{P}$. There are, however, some important problems with the linear approximation. The Stone price index is not invariant to the choice of unit of measurement and \textcite{Moschini1995} shows that this can be a significant problem. Solutions include using mean deflated prices or other price index such Tornquist, Paasche or Laspeyres. -->

<!-- Another problem is that the LA/AIDS is not integrable under the restrictions that are imposed under the AIDS model. That is, under the restrictions for the AIDS model, there is no utility function that yields a system of demand equations as in the LA/AIDS. \textcite{LaFrance2004} shows the parametric restrictions that make the LA/AIDS integrable. -->

<!-- From \textcite{Chalfant1987}, the expressions for the demand elasticities for the LA/AIDS model are given by -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item $\eta_{im} = 1+\frac{\beta_i}{s_i}$; -->
<!--     \item $\eta_i = -1 + \frac{\gamma_{ii}}{s_i} - \beta_i$; -->
<!--     \item $\eta_{ij} = \frac{\gamma_{ij}}{s_i}-\frac{\beta_i s_j}{s_i}$. -->
<!-- \end{enumerate} -->
<!-- These expressions for the elasticities are not exact but yield results that are closed to those of the AIDS model. See \textcite{Green1990} for exact expression of elasticities under the LA/AIDS model. -->

<!-- There are many variations of the AIDS model. These include \textcite{Banks1997} who introduce the Quadratic AIDS (QAIDS) and \textcite{Moschini1998} who propose a semi-flexible AIDS. -->

<!-- \subsubsection{Inverse demand system} -->
<!-- \noindent -->
<!-- So far, the models we have discussed use prices on the right-hand-side. It is however possible to estimate models using quantities on the right-hand-side. Prices tend to be highly correlated which makes it more difficult to identify parameters. On the opposite, consumption quantities tend to be less correlated. A second motive for using quantities as independent variables is the issue of endogeneity. For some commodities, assuming that prices are predetermined is reasonable, while for other commodities the assumption that quantities are predetermined is more acceptable. Section \ref{sec.endo} discusses endogeneity in demand models. -->

<!-- Some literature has proposed using quantities as the dependant variables. We will cover below the work of \textcite{Eales1994} and \textcite{Moschini1992}, who describe similar methods. Other work on inverse demand systems include \textcite{Christensen1977}. -->

<!-- Recall that the derivation of the AIDS model begins with the specification of an expenditure function that depends on prices and utility. Here, we will use an alternative representation of preference called the \emph{distance function}. The distance function $D(u,\mathbf{x})$ is defined implicitly by $U(\mathbf{x}/D(u,\mathbf{x}))=u$ \autocite{Deaton1979}. Figure \ref{fig.Distance} shows a graphical representation of a distance function. The distance function scales an arbitrary vector of quantity $\mathbf{x}$ such that utility equals an arbitrary level $u$. In figure \ref{fig.Distance}, the distance function is geometrically given by $D(u,\mathbf{x}) = 0A/0\mathbf{x}$. -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!--     \begin{picture}(240,240) -->
<!--         %Axises and labels -->
<!--         \scriptsize -->
<!--         \put(0,0){\vector(1,0){220}} %x-axis -->
<!--         \put(0,0){\vector(0,1){220}} %y-axis -->
<!--         \put(215,-10){$x_1$} -->
<!--         \put(-5,210){\makebox(0,0){$x_2$}} -->
<!--         %Utility function -->
<!--         \thicklines -->
<!--         \qbezier(20, 220)(40, 40)(220, 20)%U^0 -->
<!--         %Distance function -->
<!--         \thicklines -->
<!--         \put(0,0){\line(1,1){200}} -->
<!--         %dots -->
<!--         \put(80,80){\circle*{4}} -->
<!--         \put(180,180){\circle*{4}} -->
<!--         %Labels -->
<!--         \put(-5,-5){$0$} -->
<!--         \put(85,80){$A$} -->
<!--         \put(185,180){$\mathbf{x}$} -->
<!--         \put(225,20){$u$} -->
<!--         \end{picture} -->
<!-- \vspace{0.1in} -->
<!-- \caption{Distance function} \label{fig.Distance} -->
<!-- \end{center} -->
<!-- \end{figure} -->

<!-- The distance function has properties analogous to the cost function: homogeneous of degree one, concave, non-decreasing in quantities and decreasing in utility. Thus, one can specify a distance function in a form analogous to \eqref{eq.cost} as in \textcite{Moschini1992}: -->
<!-- \begin{equation}\label{eq.distance} -->
<!-- \ln D(u,\mathbf{x}) = a(\mathbf{x}) - u b(\mathbf{x}), -->
<!-- \end{equation} -->
<!-- where -->
<!-- \begin{align*} -->
<!-- a(\mathbf{x}) &= \alpha_0 + \sum_i \alpha_i \ln{x_i} + \frac{1}{2} \sum_i \sum_j \gamma_{ij}^\ast \ln{x_i} \ln{x_j}; \\ -->
<!-- b(\mathbf{x}) &= \beta_0 \prod_k x_k^{\beta_k}. -->
<!-- \end{align*} -->

<!-- Following \textcite{Deaton1979}, the log derivative of the distance function yields the compensated inverse demand (expenditure share): -->
<!-- \begin{equation*} -->
<!-- s_i = \alpha_i + \sum_j \gamma_{ij} \ln{x_j} + \beta_i u b(\mathbf{x}), -->
<!-- \end{equation*} -->
<!-- where $\gamma_{ij}= \frac{1}{2} (\gamma_{ij}^\ast + \gamma_{ji}^\ast) = \gamma_{ji}$. At $D(u,\mathbf{x})=1$, the distance function in \eqref{eq.distance} implicitly defines the direct utility function (utility is ordinal) such that we can write -->
<!-- \begin{equation*} -->
<!-- u=U(\mathbf{x})= \frac{a(\mathbf{x})}{b(\mathbf{x})}. -->
<!-- \end{equation*} -->
<!-- Thus, we can simplify the expression for the share and find -->
<!-- \begin{equation}\label{eq.IAIDS} -->
<!-- s_i = \alpha_i + \sum_j \gamma_{ij} \ln{x_j} + \beta_i \ln(\mathbf{X}), -->
<!-- \end{equation} -->
<!-- where -->
<!-- \begin{equation*} -->
<!-- \ln(\mathbf{X}) = \alpha_0 + \sum_i \alpha_i \ln{x_i} + \frac{1}{2} \sum_i \sum_j \gamma_{ij} \ln{x_i} \ln{x_j} -->
<!-- \end{equation*} -->
<!-- is a quantity index. Thus, the estimating equation is analogous to the estimating equation for the AIDS model. \textcite{Eales1994} refer to this model as the Inverse Almost Ideal Demand System (IAIDS) while \textcite{Moschini1992} prefer to call it Linear Inverse Demand System (LIDS). Both \textcite{Eales1994} and \textcite{Moschini1992} propose to replace the quantity index by a linear approximation $\ln(\mathbf{x^\ast}) = \sum_i s_i \ln x_i$. Note that the same caveat as in \textcite{Moschini1995} applies to this index. -->

<!-- Theoretical restrictions such that the estimated model is consistent with economics theory are the following: -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=17mm,label=\roman*.] -->
<!--     \item Adding up constraints: $\sum_i \alpha_i=1; \sum_i \beta_i=0; \sum_i \gamma_{ij}=0$; -->
<!--     \item Homogeneity: $\sum_j \gamma_{ij}=0$; -->
<!--     \item Symmetry: $\gamma_{ij} = \gamma_{ji}$. -->
<!-- \end{enumerate} -->
<!-- Those restriction are very similar to the AIDS model. -->

<!-- Estimation of an inverse demand system does not yield elasticities but rather flexibilities defined as $\upsilon_{ij} = \p \ln p_i / \p \ln x_j$. Note that there is no such thing as income flexibility for the inverse demand systems in \eqref{eq.IAIDS}. Rather, \textcite{Eales1994} use the concept of scale flexibility. Expressions for flexibilities are approximately -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item $\upsilon_{im} = -1 + \frac{\beta_i}{s_i}$; -->
<!--     \item $\upsilon_i = -1 + \frac{\gamma_{ii} + \beta_i(\alpha_i + \sum_k \gamma_{ik} \ln{x_k})}{s_i}$; -->
<!--     \item $\upsilon_{ij} = \frac{\gamma_{ij} + \beta_i(\alpha_ j + \sum_k \gamma_{ik} \ln{x_k})}{s_i}$. -->
<!-- \end{enumerate} -->
<!-- \textcite{Houck1965} shows the relationship between flexibilities and elasticities. -->

<!-- Inverse demand systems are rarely used for a few reasons. First, the interpretation of the results is not as straightforward as are the results from estimating a demand system. Second, in most cases, assuming that prices are exogenous seems more appropriate than assuming that quantities are exogenous. We will discuss this in section \ref{sec.endo}. -->

<!-- \subsubsection{Nesting of parametric models} -->
<!-- \noindent -->
<!-- Some literature developed models that nest many models within one. This sort of specification uses functional forms that are less restrictive but more difficult to estimate because of nonlinearity and an increased number of parameters. One example is \textcite{Piggott2003} who develops a model that nests many models of demand. -->

<!-- \subsection{Endogeneity of demand}\label{sec.endo} -->
<!-- \noindent -->
<!-- Consumer theory considers a representative consumer who takes prices as given. Therefore, if the theory holds, the price variable is exogenous and coefficient estimates should not be biased. Empirically, it may not be true that prices are exogenous. -->

<!-- We can question, for several reasons, whether price or quantity should be the dependant variable. According to \textcite{Thurman1987}, quantity may be predetermined in the demand for an agricultural commodity because of fixed biological lags or seasonality. That is, production is not determined by current prices but by prices observed at time of production. For nonstorable commodities, this implies that supply is perfectly inelastic, the price clears the market and absorbs any demand shock. Quantity demanded may also be considered the appropriate variable if prices are predetermined because of short-run fixity. For instance, changing prices at retail is costly and occurs only at discreet time periods. -->

<!-- What if we are concerned about endogeneity? \textcite{Thurman1987} shows how to use the Wu-Haussman test (also known as the Durbin-Wu-Haussman test or simply the Haussman test) to test for exogeneity of prices in demand for poultry in a double log model. \textcite{Thurman1987} finds that prices for poultry are predetermined by constant marginal cost of production and that quantity is determined by demand. -->

<!-- The problem of endogeneity in demand (or supply) was first observed out by \textcite{Working1927}. As the price and the quantity are determined by the intersection of the demand curve and the supply curve, ignoring one or the other obviously introduces biases. -->

<!-- Note that there might be an endogeneity problem even though data about individual consumers are available. The endogeneity problem arises because changes in consumer demands are likely correlated. That is, if the demand of one consumer changes, then the demand of other consumers is likely to change contemporaneously in the same direction. Thus, price is endogenous for the purpose of estimation although it is exogenous from the point of view of individual consumers \autocite{Rasmussen2011}. -->

<!-- What can we do if we find that the price is endogenous? We can use a structural model of the industry where the supply side is also modeled. I write a little bit about on page \pageref{sec:demand_IO}. -->

<!-- \subsection{Analysis of demand with microdata}\label{sec:microdata} -->
<!-- \noindent -->
<!-- One solution to the problem of endogeneity, although not always satisfactory, is to use microdata. Unlike aggregated data, which have been the focus of this chapter so far, microdata detail the purchases by individual consumers or households. Thus, as the unit of consumption is very small, there should be no issue regarding the endogeneity of prices or quantities. Another advantage of microdata is that they allow for the estimation of the effects of socio-demographic characteristics (e.g. age, race, education or gender) on demand. However, the use of microdata has its downside. In particular, it requires a more elaborated econometric model. -->

<!-- In a typical set of microdata, households report all their purchases in a given week. In some surveys, a panel of households will report their purchases for multiple weeks. An econometric challenge in estimating demand from microdata is how to deal with zeroes. That is, a household does not buy in a given week the whole universe of products. There are two issues with zero consumption. -->

<!-- The first issue is that the price of a product is not observable when consumption is zero. Microdata typically do not report prices but instead report quantities and expenditures, from which we can calculate unit value, a close approximation of the price. For some datasets, expenditures or prices are not reported at all. One solution is to use an available Consumer Price Index (CPI) and use Stone-Lewbel price indices to introduce variability in prices \autocite{Lewbel1989}. Prices or unit values are never available for zero consumption. A common practice is to use an average price calculated from observations in the nearby geographic area of a household. -->

<!-- The second issue is how to deal with zeroes in the econometric model. Consumption and expenditure in microdata are censored data as they are observed only when positive. It is possible to estimate any of the demand models that we have covered before by simply including or removing the observations with zero consumption. It is well known however that such approaches with censored data introduces a bias that becomes important when the number of zeroes is large. There are econometric models that explain the existence of zeroes and therefore, remove or alleviate the bias from the censoring. -->

<!-- The approach is to run a two-stage regression model. The first stage explains the existence of zero using a logit or a probit model. The second stage is a regression of consumption as the dependent variable that corrects censoring using information from the first stage. This is known in econometric as a Tobit model. The estimation of demand systems using microdata was first described by \textcite{Heien1990}. I describe below the method in \textcite{Shonkwiler1999} and \textcite{Yen2002}. Other papers using similar two-stage methods include \textcite{Meyerhoefer2005}, \textcite{Yen2006} and \textcite{Lambert2006}. -->

<!-- Denote by $i$ a product type and $j$ a household. The censoring responds to a stochastic process such that the expenditure share can be written as -->
<!-- \begin{align}%\label{eq:censoring} -->
<!-- s_{ji} &= f_{ji}(\mathbf{p}_j,m_j;\theta) + \epsilon_{ji} & & \text{if } \mathbf{z'_{ji}} \mathbf{\tau_i} + \nu_{ij}>0 \notag \\ -->
<!--        &= 0                     & & \text{Otherwise}, \notag -->
<!-- \end{align} -->
<!-- where  $f_{ji}(p_j,m_i;\theta)$ is deterministic model of expenditure share, such as those that we have covered before, $\mathbf{z'_{ji}}$ is a vector of exogenous variables, $\mathbf{\tau_i}$ is a parameter vector and $\epsilon_{ji}$ and $\nu_{ij}$ are random errors. Observe that the price vector $\mathbf{p}_j$ is specific to the household. -->

<!-- \textcite{Shonkwiler1999} and \textcite{Yen2002} assume that $u_j=(\epsilon_{j}', \nu_{i}')'$ is multivariate normal with -->
<!-- \begin{align}\label{eq:sigmas} -->
<!--  E[u_j,u_l] &= -->
<!--  \begin{bmatrix} -->
<!--      \Sigma_{\epsilon \epsilon} &  \Sigma_{\epsilon \nu} \\ -->
<!--      \Sigma_{\epsilon \nu} &  I_{n} -->
<!--   \end{bmatrix} -->
<!--   & & \text{if } j=l \\ -->
<!--        &= 0                     & & \text{Otherwise}, \notag -->
<!-- \end{align} -->
<!-- where $\Sigma_{\epsilon \epsilon} = E[\epsilon_j \epsilon_j'] = [\sigma_{ik}]$ -->
<!-- and $\Sigma_{\epsilon \nu} = E[\epsilon_j \nu_j'] = diag[\delta_1, \delta_2,..., \delta_n]$. Using \eqref{eq:sigmas} and the assumption of normality, the conditional mean of the expenditure share is -->
<!-- \begin{equation*} -->
<!-- E[s_{ji}|\nu_{ji}>-\mathbf{z'_{ji}} \mathbf{\tau_i}] = f_{ji}(\mathbf{p_j},m_j;\theta) + \delta_j \frac{\phi(\mathbf{z'_{ji}}  \mathbf{\tau_i})}{\Phi(\mathbf{z'_{ji}}  \mathbf{\tau_i})}, -->
<!-- \end{equation*} -->
<!-- where $\phi$ is the standard normal density function and $\Phi$ is the standard normal probability function. Because $E(s_{ji}|\nu_{ji}<-\mathbf{z'_{ji}} \mathbf{\tau_i}) =0 $ the unconditional mean of the expenditure share is -->
<!-- \begin{equation} \label{eq:Eshare} -->
<!-- E[s_{ji}] = \Phi(\mathbf{z'_{ji}}  \mathbf{\tau_i}) f_{ji}(\mathbf{p_j},m_j;\theta) + \delta_i \phi(\mathbf{z'_{ji}}  \mathbf{\tau_i}), -->
<!-- \end{equation} -->
<!-- Thus, from \eqref{eq:Eshare}, the system of share equations can be written as -->
<!-- \begin{equation*} -->
<!-- s_{ji} = \Phi(\mathbf{z'_{ji}}  \mathbf{\tau_i}) f_{ji}(\mathbf{p_j},m_j;\theta) + \delta_i \phi(\mathbf{z'_{ji}}  \mathbf{\tau_i}) + \xi_{ji}, -->
<!-- \end{equation*} -->
<!-- where $\xi_{ji} = s_{ji} - E(s_{ji})$. Clearly, $E(\xi_{ji})=0$ but is heteroscedastic. (Can you tell me why? See \textcite{Shonkwiler1999} for the answer.) \textcite{Yen2002} show an adjustment to the covariance matrix to correct for heteroscedasticity. \textcite{Meyerhoefer2005} instead model the heteroscedasticity of the errors term. -->

<!-- The procedure proposed by \textcite{Shonkwiler1999} and \textcite{Yen2002} is: -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=17mm,label=\roman*)] -->
<!--     \item Obtain probit estimates $\hat{\tau}_{ji}$ by maximum-likelihood; -->
<!--     \item Calculate $\phi(\mathbf{z'_{ji}}  \mathbf{\hat{\tau}_i})$ and $\Phi(\mathbf{z'_{ji}}  \mathbf{\hat{\tau}_i})$ for all $i$ and then estimate other parameters of the model in -->
<!--          \begin{equation}\label{eq:demand_tobit} -->
<!--          s_{ji} = \Phi(\mathbf{z'_{ji}}  \mathbf{\hat{\tau}_i}) f_{ji}(\mathbf{p_j},m_j;\theta) + \delta_i \phi(\mathbf{z'_{ji}}  \mathbf{\hat{\tau_i}}) + \epsilon_{ji} -->
<!--          \end{equation} -->
<!--         by maximum-likelihood or seemingly unrelated regressions. -->
<!-- \end{enumerate} -->
<!-- Note that unlike other systems of demand with the expenditure share as dependant variable, the right-hand-side of \eqref{eq:demand_tobit} does not sum to one. This means that there is no need to drop one equation and that an adding-up restriction cannot be imposed. -->

<!-- A few final notes to this section. Theoretical restrictions on the demand system are the same when estimating demand using microdata. The number of products is often very large in microdata and therefore to keep estimation feasible, one must restrict the number of products and thus rely on an assumption of separability. Even with microdata, the data are aggregated to a certain extent. For one product in a system of demand, say for example beef, microdata may report purchases of many cuts from many brands. To limit the number of products, these cuts and brands are usually aggregated together into a single product for beef. -->

<!-- Microdata are more difficult (costly) to obtain as they are often proprietary. However, very recently, the Bureau of Labor Statistics made publicly available the \emph{Consumer Expenditure Survey}. You can access the data at \url{http://www.bls.gov/cex/pumdhome.htm}. -->

<!-- \subsection{Analysis of demand in industrial organization}\label{sec:demand_IO} -->
<!-- \noindent -->
<!-- The field of industrial organization in economics has paid particular attention to estimation of demand in the last couple of decades. Why are industrial organization economists interested in estimating demand? Good estimates of demand are crucial to test theories in industrial organization. For example, to test whether firms second-degree price discriminate, a good estimate of demand is paramount as the ability of a firm to discriminate depends on the shape of the demand it perceives. -->

<!-- I will not explain structural models typically used in industrial organization. These models are quite complicated and understanding them well requires much involvement. For good summaries of these models, I refer you to \textcite{Nevo2000a} and \textcite{Rasmussen2011}. Notable papers that use structural models of demand include \textcite{Berry1995} and \textcite{Nevo2000}. In reference to \textcite{Berry1995}, these models are often referred to as BLP models. -->

<!-- \subsection{Nonparametric Analysis of Demand}\label{sec.nonpar} -->
<!-- \noindent -->
<!-- So far, the models that we have covered were based on the classical axiomatic theory of demand. In this section, we will approach demand analysis considering revealed preference. See \textcite{Varian1992} and \textcite{jehle2001} for more complete treatments of the theory that we will cover below. The nonparametric analysis of demand is based on revealed preference theory that was introduced by Paul Samuelson and then further developed by Sydney Afriat in the 60s, Erwin Diewert in the 70s and then Hal R. Varian in a series of paper in the early 80s \autocite{Vermeulen2012}. -->

<!-- Nonparametric analysis of demand does not refer to estimating a demand system without imposing functional forms like we usually mean in econometrics. Rather, nonparametric analysis of demand verifies that the data are consistent with utility maximization by testing for consistency with revealed preference axioms. This is important because any hypothesis of interest regarding the theory of demand is confounded with hypothesis about functional form in a typical empirical study of demand. Nonparametric analysis asks: -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=17mm,label=\roman*.] -->
<!--     \item Could the data have been generated by utility maximization? -->
<!--     \item Can we find a violation of consistency of data with revealed preference? -->
<!-- \end{enumerate} -->

<!-- Before turning to axioms of revealed preference, consider the following definitions from \textcite{Varian1992}: -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item \textbf{Directly revealed preferred}: If $\mathbf{p}^{0} \cdot\mathbf{x}^0 \ge \mathbf{p}^0 \cdot\mathbf{x}^1$, then it must be the case that $U(\mathbf{x}^0) \ge U(\mathbf{x}^1)$. In this case, we say that $\mathbf{x}^0$ is \emph{directly revealed preferred} to $\mathbf{x}^1$ and write $\mathbf{x}^0 R^D \mathbf{x}^1$. -->
<!--     \item \textbf{Strictly directly revealed preferred}:  If $\mathbf{p}^{0} \cdot\mathbf{x}^0 > \mathbf{p}^0 \cdot\mathbf{x}^1$, then it must be the case that $U(\mathbf{x}^0) > U(\mathbf{x}^1)$. In this case, we say that $\mathbf{x}^0$ is \emph{strictly directly revealed preferred} to $\mathbf{x}^1$ and write $\mathbf{x}^0 P^D \mathbf{x}^1$. -->
<!--     \item \textbf{Revealed preferred}: Consider that the following sequence holds: $\mathbf{p}^{0} \cdot\mathbf{x}^0 \ge \mathbf{p}^0 \cdot\mathbf{x}^1, \mathbf{p}^{1} \cdot\mathbf{x}^1 \ge \mathbf{p}^1 \cdot\mathbf{x}^2,..., \mathbf{p}^{n-1} \cdot\mathbf{x}^{n-1} \ge \mathbf{p}^{n-1} \cdot\mathbf{x}^n$. Then, we will say that $\mathbf{x}^0$ is \emph{revealed preferred} to $\mathbf{x}^n$ and write that $\mathbf{x}^0 R \mathbf{x}^n$ -->
<!-- \end{enumerate} -->

<!-- \subsubsection{Weak axiom of revealed preference (WARP)} -->
<!-- \noindent -->
<!-- The weak axiom of revealed preference states that -->
<!-- \begin{equation*} -->
<!-- \text{If } \mathbf{x}^0 R^D \mathbf{x}^1 \text{ and } \mathbf{x}^0 \text{ is not equal to } \mathbf{x}^1, \text{ then it is not the case that } \mathbf{x}^1 R^D \mathbf{x}^0. -->
<!-- \end{equation*} -->
<!-- This implies that the data should reveal that if $\mathbf{x}^0 R^D \mathbf{x}^1$ then $\mathbf{p}^{1} \cdot\mathbf{x}^1 < \mathbf{p}^1 \cdot\mathbf{x}^0$. This can be seen graphically in figure \ref{fig.WARP}. -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!--     \begin{picture}(240,240) -->
<!--         %Axises and labels -->
<!--         %\scriptsize -->
<!--         \put(0,0){\vector(1,0){240}} %x-axis -->
<!--         \put(0,0){\vector(0,1){220}} %y-axis -->
<!--         \put(215,-10){$x_1$} -->
<!--         \put(-15,210){$x_2$} -->
<!--         %Lines -->
<!--         \thicklines -->
<!--         \put(0,200){\line(1,-2){100}} -->
<!--         \put(0,100){\line(2,-1){200}} -->
<!--         %dots -->
<!--         \put(40,80){\circle*{4}} -->
<!--         \put(120,40){\circle*{4}} -->
<!--         \put(80,40){\circle*{4}} -->
<!--         %Labels -->
<!--         \put(33,65){$\mathbf{x^2}$} -->
<!--         \put(122,45){$\mathbf{x^0}$} -->
<!--         \put(65,33){$\mathbf{x^1}$} -->
<!--         \put(102,5){$\mathbf{p^1}$} -->
<!--         \put(202,5){$\mathbf{p^0}$} -->
<!--         \end{picture} -->
<!-- \vspace{-0.15in} -->
<!-- \end{center} -->
<!-- \begin{alignat*}{2} -->
<!-- \text{Notes: } & \bullet  \text{WARP: } && \mathbf{p}^{0} \cdot\mathbf{x}^0 > \mathbf{p}^0 \cdot\mathbf{x}^1 \text{ and } \mathbf{p}^1 \cdot\mathbf{x}^0 > \mathbf{p}^1 \cdot\mathbf{x}^1 \Rightarrow x^0 R^D x^1;\\ -->
<!--  & \bullet \text{SARP: } &&  \mathbf{p}^0 \cdot\mathbf{x}^0 \geq \mathbf{p}^0 \cdot\mathbf{x}^1 \text{ and } \mathbf{p}^1 \cdot\mathbf{x}^1 \geq \mathbf{p}^1 \cdot\mathbf{x}^2 \Rightarrow x^0 R x^2. -->
<!-- \end{alignat*} -->
<!-- \caption{Weak and Strong axiom of revealed preferred} \label{fig.WARP} -->
<!-- \end{figure} -->


<!-- \subsubsection{Strong axiom of revealed preference (SARP)} -->
<!-- \noindent -->
<!-- The strong axiom of revealed preference states that -->
<!-- \begin{equation*} -->
<!-- \text{If } \mathbf{x}^0 R \mathbf{x}^1 \text{ and } \mathbf{x}^0 \text{ is not equal to } \mathbf{x}^1, \text{ then it is not the case that } \mathbf{x}^1 R \mathbf{x}^0. -->
<!-- \end{equation*} -->
<!-- The SARP rules out intransitive preferences. Figure \ref{fig.WARP} illustrates. -->

<!-- \subsubsection{Generalized axiom of revealed preference (GARP)} -->
<!-- \noindent -->
<!-- WARP and SARP are not well-suited for empirical work because they are concerned with existence of utility function. In testing the data, we are concerned with whether the data are consistent with utility maximization. \textcite{Varian1982} recognized this and proposed to use the GARP, which states that -->
<!-- \begin{equation*} -->
<!-- \mathbf{x}^0 R \mathbf{x}^1 \text{ implies not } \mathbf{x}^1 P^D \mathbf{x}^0. -->
<!-- \end{equation*} -->
<!-- Thus, if the data are consistent with GARP, they should reveal that if $\mathbf{x}^0 R \mathbf{x}^2$ then it implies that $\mathbf{p}^{2} \cdot\mathbf{x}^2 < \mathbf{p}^2 \cdot\mathbf{x}^0$. -->
<!-- GARP is a generalization of SARP by allowing multivalued demand functions and flat indifference curves. If GARP holds, it implies following Afriat's theorem the existence of a utility function. Thus, if we find no violations of GARP in the data, it means that the data are consistent with the maximization of a well-behaved utility function. That is, there exists a parametric representation of the demand equations that rationalizes the data. -->

<!-- \subsubsection{Testing data for WARP} -->
<!-- \noindent -->
<!-- With a proper algorithm, it is not difficult to test the data for consistency with GARP on a computer. The algorithm must verify the consistency with GARP for every $\mathbf{x}^i$ and $\mathbf{x}^j$. -->

<!-- The algorithm for testing for WARP is quite simple. Recall that the WARP states that -->
<!-- \begin{equation*} -->
<!-- \mathbf{x}^0 R^D \mathbf{x}^1 \text{ if } \mathbf{p}^{0} \cdot \mathbf{x}^0 \geq \mathbf{p}^0 \cdot\mathbf{x}^1 \text{ and } \mathbf{p}^1 \cdot\mathbf{x}^0 > \mathbf{p}^1 \cdot\mathbf{x}^1. -->
<!-- \end{equation*} -->
<!-- This can be rewritten as -->
<!-- \begin{equation*} -->
<!-- \mathbf{x}^0 R^D \mathbf{x}^1 \text{ if } 1 \geq \frac{\mathbf{p}^0 \cdot\mathbf{x}^1}{m^0} \text{ and } \frac{\mathbf{p}^1 \cdot\mathbf{x}^0}{m^1} > 1. -->
<!-- \end{equation*} -->
<!-- Empirically, the strategy to test WARP is to first build the following matrix: -->
<!-- \begin{equation*} -->
<!-- \left( -->
<!--   \begin{array}{ccc} -->
<!--      \mathbf{p}^{0} \cdot \mathbf{x}^0 &  \mathbf{p}^{0} \cdot \mathbf{x}^1 &  \mathbf{p}^{0} \cdot \mathbf{x}^2 \\ -->
<!--      \mathbf{p}^{1} \cdot \mathbf{x}^0 &  \mathbf{p}^{1} \cdot \mathbf{x}^1 &  \mathbf{p}^{1} \cdot \mathbf{x}^2 \\ -->
<!--      \mathbf{p}^{2} \cdot \mathbf{x}^0 &  \mathbf{p}^{2} \cdot \mathbf{x}^1 &  \mathbf{p}^{2} \cdot \mathbf{x}^2 \\ -->
<!--   \end{array} -->
<!-- \right). -->
<!-- \end{equation*} -->
<!-- Then dividing each row of the matrix by the expenditure given on the diagonal we can write: -->
<!-- \begin{equation}\label{eq.matWARP} -->
<!-- \left( -->
<!--   \begin{array}{ccc} -->
<!--      1 &  \frac{\mathbf{p}^{0} \cdot \mathbf{x}^1}{m^0} &  \frac{\mathbf{p}^{0} \cdot \mathbf{x}^2}{m^0} \\ -->
<!--      \frac{\mathbf{p}^{1} \cdot \mathbf{x}^0}{m^1} &  1 &  \frac{\mathbf{p}^{1} \cdot \mathbf{x}^2}{m^1} \\ -->
<!--      \frac{\mathbf{p}^{2} \cdot \mathbf{x}^0}{m^2} &  \frac{\mathbf{p}^{2} \cdot \mathbf{x}^1}{m^2} &  1 \\ -->
<!--   \end{array} -->
<!-- \right). -->
<!-- \end{equation} -->
<!-- We can test WARP by comparing the values of pairs in \eqref{eq.matWARP} to 1. Consider the bundles $k$ and $l$. We know that WARP hold if  $1 \geq \frac{\mathbf{p}^k \cdot\mathbf{x}^l}{m^k}$ and $\frac{\mathbf{p}^l \cdot\mathbf{x}^k}{m^l} > 1$. So we say that WARP does not hold whenever we find a case where these inequalities do not hold. -->

<!-- There are, however, some problems with testing for WARP or other axioms of preference. What do we do if we find violations? Do we reject economic theory? With time series data the budget constraint shifts out and therefore it is difficult to find violations. What is the power of testing dating for violations in WARP? -->

<!-- Results of revealed preference tests are reported using the number of successes. This is not a statistic and therefore it is difficult to understand the meaning of the test. Given that the test is exact, a single violation should be sufficient to reject consistency. As such, the size of the test on revealed preferences is zero \autocite{Moschini1996}. The power of the test, the capacity of detecting violations when there are in fact violations, is unknown. Evidence suggests that the power of test on revealed preferences is small. One reason is the shift in the budget line as the next section covers. -->

<!-- \subsubsection{How demanding is revealed preference?} -->
<!-- \noindent -->
<!-- Figure \ref{fig.WARP2} shows two budget lines, typical of what may be observed in a dataset. That is, relative prices are quite stable over time while income increases. This means that the budget line shifts out but that its slope does not change by much. Thus, as budget line do not cross, it is almost impossible to observe violation of revealed preference. -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!--     \begin{picture}(240,240) -->
<!--         %Axises and labels -->
<!--         %\scriptsize -->
<!--         \put(0,0){\vector(1,0){220}} %x-axis -->
<!--         \put(0,0){\vector(0,1){240}} %y-axis -->
<!--         \put(215,-10){$x_1$} -->
<!--         \put(-15,210){$x_2$} -->
<!--         %Lines -->
<!--         \thicklines -->
<!--         \put(0,200){\line(1,-1.5){133}} -->
<!--         \put(0,100){\line(1,-1){100}} -->
<!--         %dots -->
<!--         \put(50,50){\circle*{4}} -->
<!--         \put(80,80){\circle*{4}} -->
<!--         %Labels -->
<!--         \put(136,5){$\mathbf{p^1}$} -->
<!--         \put(102,5){$\mathbf{p^0}$} -->
<!--         \put(52,50){$\mathbf{x^0}$} -->
<!--         \put(82,80){$\mathbf{x^1}$} -->
<!--         \end{picture} -->
<!-- \vspace{0.1in} -->
<!-- \caption{Inability to detect violations} \label{fig.WARP2} -->
<!-- \end{center} -->
<!-- \end{figure} -->

<!-- Empirically, almost no violations of GARP are found, i.e. the pass rate is usually near 100\%. Thus, as figure \ref{fig.WARP2} shows, empirically the conditions from WARP to fail may be too undemanding. Some literature proposes corrections to account for the shift in the budget but these are not always convincing. Recently, \textcite{Beatty2011} propose a correction based on restrictions on choices implied by GARP. The authors use the restrictions on budget share to penalize the pass rate. The less restrictive GARP is, the more penalty is imposed on the measure of success. -->

<!-- \subsection{Applications of demand analysis: structural change in the demand for meat} -->
<!-- \noindent -->
<!-- During the 1980s, economists noticed that American consumers had been consuming less red meat and more white meat. Figure \ref{fig.quantities} shows the consumptions of meat per capita of US consumers between 1975 and 2000. Notice the sharp decrease in the consumption of beef and the increase in the consumption of poultry. What explains these changes? Health concerns? Change in tastes? Change in relative prices? -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!-- \includegraphics[width=0.9\textwidth,keepaspectratio]{quantities.PNG} -->
<!-- \caption{US per capita meat consumption in lb.} \label{fig.quantities} -->
<!-- \end{center} -->
<!-- \end{figure} -->

<!-- According to \textcite{Stigler1977} tastes do not change. Constant taste is a tautology with respect to fundamental goods. Taste may seem to change when incorporating only market goods in empirical analysis. Not every economists agree with that statement. Taste may also seem to change because product quality changes over time but that is not captured by the data. For example, chicken used to be offered as whole, almost exclusively, and now it is offered by parts. -->

<!-- Here, we will explore two papers that investigate whether tastes for meat have changed. There is an important literature on that topic and some other significant contributions include \textcite{Chavas1983} and \textcite{Eales1988}. -->

<!-- \subsubsection{\textcite{Moschini1989}} -->
<!-- \noindent -->
<!-- \textcite{Moschini1989} test for a structural change in the demand for meat. The authors do not search for a structural change of any specific nature but for a change in demand not explained by relative prices and income. \textcite{Moschini1989} assume that structural change occurs following a path $h_t$.\footnote{Since then, the literature on structural change has very much progressed. Recent contributions estimates of structural changes at unknown date \cite[e.g.][]{Gregory1996, Hansen2001, Bai2003}.} The LA/AIDS model estimated is given by -->
<!-- \begin{equation*} -->
<!-- s_{it} = \alpha_i + \gamma_i h_t + \sum_j (\beta_{ij} +\delta_{ij} h_t)\ln{p_{jt}} + (\beta_i + \delta_{i} h_t) \ln{(\frac{m}{P})} + \sum_k (\alpha_{ik} + \gamma_{ik} h_t) D_k + e_{it}, -->
<!-- \end{equation*} -->
<!-- where $D$ are seasonal dummies. \textcite{Moschini1989} test whether $\gamma=0$ and $\delta=0$. -->

<!-- Figure \ref{fig.path} shows how the time path is constructed. The bounds $\tau_1$ and $\tau_2$ are parameters to be estimated. If $\tau_2=\tau_1+1$, the structural change is abrupt (Chow test). However, if $\tau_2=T$ and $\tau_1=0$, the structural change occurs very slowly. The values for $\tau_1$ and $\tau_2$ are found by maximizing the likelihood function. -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!--     \begin{picture}(340,100) -->
<!--         %Axises and labels -->
<!--         %\scriptsize -->
<!--         \put(0,0){\vector(1,0){330}} %x-axis -->
<!--         \put(115,-10){$\tau_1$} -->
<!--         \put(215,-10){$\tau_2$} -->
<!--         \put(305,-10){$T$} -->
<!--         %Lines -->
<!--         \thicklines -->
<!--         \put(0,0){\line(1,0){115}} -->
<!--         \put(115,0){\line(4,3){100}} -->
<!--         \put(215,75){\line(1,0){90}} -->
<!--         \thinlines -->
<!--         \multiput(215,75)(0,-5){15}{\line(0,-1){2.5}}%Dashed line - vertical -->
<!--         \end{picture} -->
<!-- \vspace{0.1in} -->
<!-- \caption{Time path in \textcite{Moschini1989}} \label{fig.path} -->
<!-- \end{center} -->
<!-- \end{figure} -->

<!-- \begin{figure}[htbp] -->
<!-- \begin{center} -->
<!-- \includegraphics[width=4in]{Confidence.JPG} -->
<!-- \end{center} -->
<!-- \caption{Confidence regions for structural change parameters: figure 2 in \textcite{Moschini1989}} \label{fig.region} -->
<!-- \end{figure} -->

<!-- Figure \ref{fig.region} shows the confidence region for the structural changes in the model's parameters. It suggests a structural change in the mid 70s. \textcite{Moschini1989} conclude that: -->
<!-- \begin{enumerate}[topsep=0mm,leftmargin=15mm,noitemsep,label=\roman*)] -->
<!--     \item Observed meat consumption patterns cannot be fully explained by the dynamics of prices and income; -->
<!--     \item Constant parameters are rejected by the AIDS model. -->
<!-- \end{enumerate} -->
<!-- Note that \textcite{Moschini1989} never mention that tastes have changed. The conclusions are that a structural change has affected the demand for meat. However, \textcite{Moschini1989} do not explain what is that structural change. -->

<!-- \subsubsection{\textcite{Chalfant1988}} -->
<!-- \noindent -->
<!-- Mispecification of parametric models may yield the rejection of stable preference. \textcite{Chalfant1988} ``test'' stability of preferences for meat consumption data nonparametrically in order to impose a minimum of joint hypotheses (i.e. functional forms and structural change). -->

<!-- The authors test for violations in GARP using data on meat consumption in the US and Australia. They explain that possible violations may be due to: 1) Dynamics; 2) Change in taste; 3) Inappropriate aggregation; 4) Inappropriate separability; 5) Demographic change; 6) Quality change; 7) Change in household production technology; and 8) Uncertainty, risk. \textcite{Chalfant1988} find minor violations of GARP in Australian data (mutton) but no violations in US data. From this, the authors conclude that the data were generated by a system of stable, well-behaved, weakly separable, per capita demand equations. The authors also find that adjusting expenditure for income growth, assuming that income elasticities equal one, did not result in any violations. Their final conclusion is that the data do not indicate changes in preferences and that relative prices alone can account for observed shifts in consumption patterns. -->

<!-- As mentioned in section \ref{sec.nonpar}, there are a number of limitations to nonparametric analysis of demand. In this particular case, an important one is the power of the test performed by \textcite{Chalfant1988}. The section on the power of nonparametric test is puzzling. \textcite{Moschini1996} finds it surprising that there are no violations in the data given seasonality in quarterly data. -->

<!-- %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% -->

<!-- \renewcommand{\thesection}{A.\arabic{section}} -->
<!-- \renewcommand{\theHsection}{A.\arabic{section}} -->

<!-- \setcounter{secnumdepth}{0} -->
<!-- \subsection{Appendix A: Brief review of consumer theory} -->
<!-- \setcounter{secnumdepth}{2} -->
<!-- \setcounter{equation}{0} -->

<!-- \noindent -->
<!-- The treatment of consumer theory in this section is far from being complete but you should find the following summary useful for the material that we cover in this section and later in class. Here, I present consumer theory like a list, without going into the detail as this section is meant as a reminder for you. When giving properties of functions, the lists are not always complete. For much more exhaustive treatments of consumer theory, I refer you to \textcite{Varian1992}, \textcite{MasColell1995} or \textcite{jehle2001}. -->

<!-- \subsubsection{Properties of utility function} -->
<!-- \noindent -->
<!-- If preference ordering is complete, transitive, monotone, convex and continuous, then there exists a utility function that represents preferences. -->
<!-- \begin{enumerate}[topsep=0mm,leftmargin=15mm,noitemsep,label=\roman*)] -->
<!--   \item $U(\mathbf{x})$ is increasing; -->
<!--   \item $U(\mathbf{x})$ is (strictly) quasiconcave if $\succeq$ is (strictly) convex. -->
<!-- \end{enumerate} -->

<!-- \subsubsection{Consumer's problem} -->
<!-- \noindent -->
<!-- Marshallian(Walrasian) demand: $\mathbf{x}(\mathbf{p},W)=\arg \max U(\mathbf{x}) \text{ s.t. } \mathbf{p}\cdot\mathbf{x} \leq W$.\\ -->
<!-- \noindent -->
<!-- \begin{tabular}{ll} -->
<!-- Properties: & i) Homogeneous of degree zero in price and wealth (no money illusion);\\ -->
<!--             & ii) Walras's law, i.e. $\mathbf{p}\cdot\mathbf{x} = W$;\\ -->
<!--             & iii) Convex. -->
<!-- \end{tabular} -->

<!-- \subsubsection{Indirect utility function} -->
<!-- \noindent -->
<!-- \begin{equation*} -->
<!-- V(\mathbf{p},W) = \max U(\mathbf{x}) \text{ s.t. } \mathbf{p}\cdot\mathbf{x} \leq W. -->
<!-- \end{equation*} -->
<!-- \noindent -->
<!-- \begin{tabular}{ll} -->
<!-- Properties: & i) Homogeneous of degree zero;\\ -->
<!--             & ii) Increasing in $W$, nonincreasing in $p$;\\ -->
<!--             & iii) Quasiconvex.\\ -->
<!--             & iv) Continuous. -->
<!-- \end{tabular} -->

<!-- Roy's identity: -->
<!-- \begin{equation}\label{eq.Roy} -->
<!-- x_i(\mathbf{p},W)=-\frac{\p V(\mathbf{p},W)}{\p p_i}/\frac{\p V(\mathbf{p},W)}{\p W}. -->
<!-- \end{equation} -->

<!-- \subsubsection{Hicksian demand} -->
<!-- \noindent -->
<!-- \begin{equation*} -->
<!-- \mathbf{h}(\mathbf{p},u)=\arg \min \mathbf{p}\cdot\mathbf{x} \text{ s.t. } U(\mathbf{x}) \ge u. -->
<!-- \end{equation*} -->
<!-- \noindent -->
<!-- \begin{tabular}{ll} -->
<!-- Properties: & i) Homogeneous of degree zero;\\ -->
<!--             & ii) No excess utility: $\mathbf{x}=\mathbf{h}(\mathbf{p},u)$, $U(\mathbf{x})=u$;\\ -->
<!--             & iii) Convex. -->
<!-- \end{tabular} -->

<!-- \subsubsection{Expenditure minimization problem} -->
<!-- \noindent -->
<!-- \begin{equation*} -->
<!-- e(\mathbf{p},u)=\min \mathbf{p}\cdot\mathbf{x} \text{ s.t. } U(\mathbf{x}) \ge u. -->
<!-- \end{equation*} -->
<!-- \noindent -->
<!-- \begin{tabular}{ll} -->
<!-- Properties: & i) Homogeneous of degree one in $\mathbf{p}$;\\ -->
<!--             & ii) Increasing in $\mathbf{p}$, nondecreasing in u;\\ -->
<!--             & iii) Concave in $\mathbf{p}$;\\ -->
<!--             & iv) Continuous. -->
<!-- \end{tabular} -->

<!-- Shephard's lemma: -->
<!-- \begin{equation}\label{eq.Shephard} -->
<!-- \frac{\p e(\mathbf{p},u)}{\p p_i}= h_i(\mathbf{p},u). -->
<!-- \end{equation} -->

<!-- \subsubsection{Important relationships (Duality)} -->
<!-- \begin{enumerate}[noitemsep, topsep=0mm, leftmargin=10mm,label=\textbullet] -->
<!--     \item $e(\mathbf{p},u)=W$; -->
<!--     \item $V(\mathbf{p},W)=u$; -->
<!--     \item $\mathbf{x}(\mathbf{p},W)=\mathbf{h}(\mathbf{p},V(\mathbf{p},W))$; -->
<!--     \item $\mathbf{h}(\mathbf{p},u)=\mathbf{x}(\mathbf{p},e(\mathbf{p},u))$. -->
<!-- \end{enumerate} -->

<!-- \subsubsection{Engel aggregation} -->
<!-- \noindent -->
<!-- By Walras law we know that -->
<!-- \begin{equation*} -->
<!-- \sum_i p_i x_i(\mathbf{p},W)=W. -->
<!-- \end{equation*} -->
<!-- Partially differentiating both sides with respect to W yields -->
<!-- \begin{equation*} -->
<!-- \sum_i p_i\frac{\p  x_i(\mathbf{p},W)}{\p W}=1. -->
<!-- \end{equation*} -->
<!-- Simplifying we find -->
<!-- \begin{align*} -->
<!-- \sum_i \frac{p_i x_i(\mathbf{p},W)}{W} \frac{\p  x_i(\mathbf{p},W)}{\p W}\frac{W}{x_i(\mathbf{p},W)} &=1\\ -->
<!-- \sum_i s_i \eta_{iW} &=1, -->
<!-- \end{align*} -->
<!-- where $s_i$ is the expenditure share and $\eta_{iW}$ is the income elasticity of demand for good $i$. -->

<!-- \subsubsection{Cournot aggregation} -->
<!-- \noindent -->
<!-- Again, by Walras law we know that -->
<!-- \begin{equation*} -->
<!-- \sum_i p_i x_i(\mathbf{p},W)=W. -->
<!-- \end{equation*} -->
<!-- This time, partially differentiating both side with respect to $p_j$ we find -->
<!-- \begin{equation*} -->
<!-- x_j(\mathbf{p},W)+\sum_i p_i\frac{\p  x_i(\mathbf{p},W)}{\p p_j}=0. -->
<!-- \end{equation*} -->
<!-- A few manipulations and simplifications yield -->
<!-- \begin{align*} -->
<!-- -\frac{p_j x_j(\mathbf{p},W)}{W} &= \sum_i \frac{p_i x_i(\mathbf{p},W)}{W} \frac{\p  x_i(\mathbf{p},W)}{\p p_j} \frac{p_j}{x_i(\mathbf{p},W)}\\ -->
<!-- -s_j &= \sum_i s_i \eta_{ij}, -->
<!-- \end{align*} -->
<!-- where $\eta_{ij}$ is the cross-price elasticity. -->

<!-- \subsubsection{Slutsky equation} -->
<!-- \noindent -->
<!-- We know that the the Marshallian demand equals the Hicksian demand -->
<!-- \begin{equation*} -->
<!-- h_i(\mathbf{p},u)=x_i(\mathbf{p},W). -->
<!-- \end{equation*} -->
<!-- Partially differentiating both sides with respect $p_j$ and using Shephard's lemma in \eqref{eq.Shephard} -->
<!-- \begin{equation*} -->
<!-- \frac{\p h_i(\mathbf{p},u)}{\p p_j}=\frac{\p x_i(\mathbf{p},W)}{\p p_j} + \frac{\p x_i(\mathbf{p},W)}{\p W}\frac{\p e(\mathbf{p},u)}{\p p_j} =\frac{x_i(\mathbf{p},W)}{\p p_j} + \frac{\p x_i(\mathbf{p},W)}{\p W} x_j(\mathbf{p},W). -->
<!-- \end{equation*} -->
<!-- Multiplying both sides by $p_j$ and dividing both sides by $h_i(\mathbf{p},u)=x_i(\mathbf{p},W)$ yields -->
<!-- \begin{equation*} -->
<!-- \frac{\p h_i(\mathbf{p},u)}{\p p_j} \frac{p_j}{h_i(\mathbf{p},u)} = \frac{\p x_i(\mathbf{p},W)}{\p p_j} \frac{p_j}{x_i(\mathbf{p},W)} + \frac{\p x_i(\mathbf{p},W)}{\p W} \frac{W}{x_i(\mathbf{p},W)} \frac{p_j x_j(\mathbf{p},W)}{W}. -->
<!-- \end{equation*} -->
<!-- Thus we can write the Slutsky equation in terms of elasticities is -->
<!-- \begin{equation}\label{eq.Slutsky} -->
<!-- \eta_{ij}^{H} = \eta_{ij} + s_j \eta_{iW}, -->
<!-- \end{equation} -->
<!-- where $\eta_{ij}^{H}$ denotes the Hicksian (compensated) elasticity of demand. We can do the same derivation in matrix form and obtain the Slutsky matrix, which is symmetric (Young's theorem) and negative semidefinite. -->

<!-- Symmetry of the Slutsky matrix implies that -->
<!-- \begin{align*} -->
<!-- \frac{\p h_i(\mathbf{p},u)}{\p p_j} &= \frac{\p h_j(\mathbf{p},u)}{\p p_i} \\ -->
<!-- \frac{\p h_i(\mathbf{p},u)}{\p p_j} \frac{p_j}{h_i(\mathbf{p},u)} \frac{p_i h_i(\mathbf{p},u)}{W}&= \frac{\p h_j(\mathbf{p},u)}{\p p_i} \frac{p_i}{h_j(\mathbf{p},u)} \frac{p_j h_j(\mathbf{p},u)}{W}\\ -->
<!-- \eta_{ij}^{H} s_i &= \eta_{ji}^{H} s_j. -->
<!-- \end{align*} -->
<!-- This also implies that we find for the Allen elasticity of substitution that $\sigma_{ij}=\sigma_{ji}$. We will come back to that elasticity later. -->

<!-- \subsubsection{Homogeneity} -->
<!-- \noindent -->
<!-- Homogeneity of the Marshallian demand implies that we can write -->
<!-- \begin{equation*} -->
<!-- x_i(\mathbf{p},W) = x_i(\alpha\mathbf{p},\alpha W), -->
<!-- \end{equation*} -->
<!-- where $\alpha>0$. Differentiating the Marshallian demand yields -->
<!-- \begin{equation*} -->
<!-- dx_i(\mathbf{p},W) = \sum_j \frac{\p x_i(\mathbf{p},W)}{\p p_j} d p_j + \frac{\p x_i(\mathbf{p},W)}{\p W} d W. -->
<!-- \end{equation*} -->
<!-- Dividing by $x_i$ on both sides -->
<!-- \begin{equation*} -->
<!-- \frac{d x_i(\mathbf{p},W)}{x_i} = \sum_j \frac{\p x_i(\mathbf{p},W)}{\p p_j} \frac{p_j}{x_i(\mathbf{p},W)} \frac{d p_j}{p_j} + \frac{\p x_i(\mathbf{p},W)}{\p W} \frac{W}{x_i(\mathbf{p},W)} \frac{d W}{W}. -->
<!-- \end{equation*} -->
<!-- Using $E$ as an operator to denote a change in percentage, we can write -->
<!-- \begin{equation*} -->
<!-- E x_i(\mathbf{p},W) = \sum_j \eta_{ij} E p_j + \eta_{iW} E W. -->
<!-- \end{equation*} -->
<!-- Let $E p_j = E W = \alpha$. Because the demand is homogeneous of degree 0, this implies that $E x_i(\mathbf{p},W)=0$. Thus we find that -->
<!-- \begin{equation*} -->
<!-- \sum_j \eta_{ij} + \eta_{iW} = 0. -->
<!-- \end{equation*} -->
<!-- Using Slutsky equation in \eqref{eq.Slutsky} we can write -->
<!-- \begin{equation*} -->
<!-- \sum_j \eta_{ij}^{H} - \eta_{iW} \sum_j s_j + \eta_{iW} = 0. -->
<!-- \end{equation*} -->
<!-- Because the expenditure shares sum to 1, we can write -->
<!-- \begin{equation*} -->
<!-- \sum_j \eta_{ij}^{H} = 0. -->
<!-- \end{equation*} -->



