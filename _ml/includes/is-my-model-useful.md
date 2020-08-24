\ifndef{isMyModelUseful}
\define{isMyModelUseful}

\editme

\subsection{Is my Model Useful?}

> All models are wrong, but some are useful
>
> @Box:science76

\notes{This important quote has become worn by overuse (like a favorite
sweater). Worse still it is almost being bandied around to mean that
*because* my model is wrong it *might* be useful. It seems that people
almost equate the statement to meaning probability of my model being
wrong given that its useful is = 1. Which would be an incorrect model
but seems to be useful in practice when trying to justify poor
assumptions.}

\notes{Perhaps we should be more focusing on the quote from the same paper

> the scientist must be alert to what is importantly wrong. It is inappropriate to be concerned about mice when there are tigers abroad. 
>
> @Box:science76

First highlighted to me by Richard Wilkinson. Let's have a think about
where the tigers might be in the domain of big data. To consider this,
let's first see what we can write down about our data that isn't
implicitly wrong. If we are interested in multivariate data we could
first write down our data in the following form.}
$$
\text{data} = \mathbf{\dataMatrix} \in \Re^{\numData\times \dataDim},
$$
where here we are assuming we have $\numData$ data points and $\dataDim$
features. As soon as we write down our data in this form it
invites particular assumptions about the data that may have been valid
in the 1930s, when there was more focus on survey data. Experimental designs 
stipulated a table of data with a specific set of hypotheses in mind. The data
naturally sat in a matrix. 

As soon as we write down our data in a
matrix form, $\dataMatrix\in \Re^{\numData\times \dataDim}$ it almost second nature 
to begin making factorization assumptions. In particular, an independence assumption across
the $\numData$ data points.}
\begin{align*}
p(\dataMatrix|\parameterVector) = \prod_{i=1}^\numData p(\dataVector_{i, :} | \boldsymbol{\theta})
\end{align*}
\notes{This factorization gives several advantages. It has a theoretical framing, that easily allows us
to show that by optimizing the resulting lieklihood, we are minimizing a sample based approximation to a
Kullback-Leibler divergence between our model and the true data generating density (see e.g. @Wasserman:all03). 
\begin{align*}
\log p(\dataMatrix|\parameterVector) =& \sum_{i=1}^\numData \log p(\dataVector_{i, :} | \boldsymbol{\theta}) + \text{const}
\approx & \int \Pr(\dataMatrix) \log \frac{p(\dataMatrix|\parameterVector)}{\Pr(\dataMatrix)}
\end{align*}
where \Pr(\dataMatrix) is the true data generating distribution.

From pragmatist's perspective, the assumption allows us to easily make predictions about new data
points given a parameter vector that is derived from the training data.
This assumption will generally be wrong, and also leads to concerns
about the parameters when $\numData<<\dataDim$, the so called \`large
$\dataDim$, small $\numData$' domain.}

\notes{I think that this is a wrongheaded way of thinking about modern data,
because in practice, $\dataDim$, doesn't really exist, at least not in
the sense that the above model implies we should treat it. It doesn't
exist as a static view of the data: $\dataDim$ is much more fluid than
the model above implies. Indeed, I'll argue below that rather than
increasing $\dataDim$ when we obtain a new feature about a data point,
we should be increasing $\numData$. That adding writing down our data in
matrix form, $\dataMatrix$, may even be constraining our thinking to
these factorized models. And the fact that the factorization is strong:
i.e. it assumes that all becomes independent given the parameters, it is
very often wrong. That is not to say that these factorization
assumptions are not useful, indeed we will make use of them below, but
they should *not* be the first thing we write down.}

\endif